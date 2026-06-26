---
tipo: aprofundamento
nivel: 4
fluxo: Estratégia & Visão
conceito_pai: Era dos evals — o eval é o PRD do modelo
autores: [Brendan Foody, Hamel Husain, Shreya Shankar]
---
# 📜 Era dos evals — Evidências
**↑ Card:** [[Era dos evals — o eval é o PRD do modelo]] · **Tema:** [[Estratégia — Estratégia de produto]] · **Camada:** L4
**Fontes:** [[Brendan Foody]] (1:07:08) · [[Hamel Husain]] (1:46:33) · [[Shreya Shankar]] (1:46:33)

---

## Por que evals são o PRD do modelo (Brendan Foody)

Brendan Foody — fundador de empresa especializada em evals para labs de IA — articula a tese estrutural: o gargalo primário para melhorar qualquer modelo de IA não é dados de pré-treino, é a **capacidade de definir o que é sucesso**.

> "Se o modelo é o produto, o eval é o PRD — mas também o material de vendas. Os labs usam evals para demonstrar as capacidades dos seus modelos."

> "O gargalo primário dos labs para melhorar modelos é como eles podem medir efetivamente o que parece sucesso para o modelo."

> "A barreira para aplicar agentes em toda a economia para automatizar qualquer workflow é: como medimos sucesso? Como fazemos o eval?"

> "Os modelos são apenas tão bons quanto seus evals."

O mercado de evals como negócio criou uma nova categoria de trabalho especializado — mais bem-paga que crowdsourcing comum porque requer expertise de domínio. Os top 10% dos contribuidores geram a maioria das melhorias de modelo — mesma lei de potência que se vê em organizações de alto desempenho.

A mecânica: o eval define uma rubrica; o modelo aprende via RL (RLAIF) a atingir o critério. Empresas que criam evals para seus workflows próprios acumulam vantagem competitiva porque provam (para si e para parceiros) o que os modelos sabem fazer no seu domínio específico.

---

## Evals como processo prático para times de produto (Hamel Husain)

Hamel traz a perspectiva do consultor que implementou evals em dezenas de produtos de IA. A tese operacional: evals é data analytics, não rocket science.

**O processo em três fases:**

**Fase 1 — Error Analysis (Open Coding)**
Abrir a ferramenta de observabilidade, revisar traces individuais e anotar livremente. Não é preciso categorizar ainda — só descrever o problema mais upstream em cada trace.

> "Você aprende uma quantidade absurda quando faz isso. Toda pessoa que faz isso fica viciada imediatamente. Quando você está construindo um app de IA, você simplesmente aprende muito."

> "Para a maioria dos problemas, você vê os olhos das pessoas abrirem quando eu digo 'vamos olhar seus traces agora'. Eles ficam surpresos que eu vou olhar traces individuais — e 100% das vezes aprendemos muito e descobrimos o problema."

> "A contagem básica é a técnica analítica mais poderosa em ciência de dados porque é simples e acessível a todos."

**Fase 2 — Axial Coding com LLM**
Exportar os open codes para uma planilha e pedir a um LLM para agrupar em categorias de falha acionáveis. O LLM é excelente nessa tarefa de síntese — mas a revisão e renomeação é humana.

> "Use as palavras 'open codes' e 'axial codes' no prompt — o LLM conhece esses termos das ciências sociais e sabe o que fazer. Isso é um atalho poderoso."

**Fase 3 — LLM como Juiz**
Para cada categoria de falha prioritária, criar um prompt de avaliação binário (true/false). Validar contra labels humanos antes de publicar. Implantar em CI e em monitoramento de produção.

> "Quando você reporta métricas, ninguém sabe o que 3.2 versus 3.7 significa. A decisão tem de ser sim ou não. Pode ser doloroso definir isso, mas você absolutamente deve — caso contrário, o processo vira intratável."

> "Antes de publicar o judge, verifique se ele concorda com o seu julgamento humano. Use a matriz de confusão, não só a taxa de concordância global — 90% pode ser enganoso quando o erro é raro."

**Timing e ROI:**

> "É a atividade de maior ROI que você pode fazer. Para a maioria dos produtos, você faz esse processo uma vez e depois constrói sobre ele."

> "Para um app de IA que envia emails, as empresas que fazem isso bem têm um senso muito aguçado de como a aplicação está performando. As pessoas não falam sobre isso porque é seu moat."

---

## Criteria Drift e a Ciência dos Evals (Shreya Shankar)

Shreya Shankar combina perspectiva de pesquisadora (paper "Who Validates the Validators?") com experiência prática em dezenas de pipelines de LLM.

**O problema central — criteria drift:**
No software tradicional, os requisitos são definidos antes da implementação. Em produtos de IA, os critérios de qualidade **mudam conforme você vê os outputs reais**.

> "O que descobrimos no estudo foi que as pessoas não conseguem definir seus critérios upfront. As opiniões sobre o que é bom ou ruim mudam à medida que revisam mais outputs. Eles descobrem modos de falha apenas depois de ver 10 outputs que nunca teriam sonhado em primeiro lugar — e isso vale para especialistas."

Esse fenômeno explica por que pular direto para escrever prompts de judge (sem olhar dados primeiro) é uma armadilha: você vai escrever critérios para falhas que imaginou, não para as falhas reais do produto.

**Saturação teórica:**
> "Quando você deixar de descobrir novos tipos de problema, é hora de parar. Isso é saturação teórica — um conceito que vem da análise qualitativa. Alguns precisam de 100 traces, outros de 40, outros de 15. Depende da complexidade do produto e da sua experiência em análise de erros."

**Evals como especificação viva:**
> "O eval vai mudar sua PRD. Você vai descobrir expectativas que não existiam no documento original — e isso é uma feature, não um bug. Você nunca sabe exatamente o que quer até ver o que o LLM faz."

**Número de judges necessários:**
> "Entre quatro e sete. Não é muito, porque muitos modos de falha se resolvem apenas ajustando o prompt. Você não deve criar um eval para tudo — priorize os que são persistentes mesmo após descrever o comportamento ideal no prompt do agente."

**Escala e custo:**
> "Depois de criar os judges, o custo recorrente é baixo: cron job semanal, 30 minutos de revisão. O custo upfront de 3-4 dias de error analysis é investimento pontual. O moat vem de acumular esse conhecimento sobre seu produto que nenhum concorrente tem — porque ninguém está fazendo isso sistematicamente."

---

## Padrão convergente: evals como moat operacional

Os três autores convergem num insight comum: evals não são apenas uma prática de engenharia — são **vantagem competitiva acumulada**. A empresa que sabe exatamente onde seu produto de IA falha, e tem sistemas para detectar e corrigir isso em tempo real, opera num plano diferente. Esse conhecimento não é transferível via benchmarks públicos — está embutido nos dados de produção e nos critérios específicos do domínio.

Brendan enquadra isso em nível de modelo (labs competindo via evals); Hamel e Shreya em nível de produto (times que conhecem suas falhas antes dos usuários). O princípio é o mesmo: **medir com precisão é o que separa quem melhora de quem acha que melhorou**.
