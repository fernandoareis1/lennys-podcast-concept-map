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

## [[Brendan Foody]] — A camada de negócio dos evals (2025-09-18)

> "Se o modelo é o produto, o eval é o PRD — mas também é o material de vendas. Os labs usam evals para demonstrar as capacidades dos seus modelos."

> "O gargalo primário dos labs para melhorar modelos é como eles podem medir efetivamente o que parece sucesso para o modelo. Toda capacidade que você quer que o modelo execute precisa de um eval primeiro."

> "A barreira para aplicar agentes em toda a economia para automatizar qualquer workflow é: como medimos sucesso? Como fazemos o eval?"

> "Os modelos são apenas tão bons quanto seus evals. Toda a economia vai provavelmente se tornar uma máquina de ambiente de evals, construindo mundos e contextos para que haja rubrics ou verificadores."

**Mecanismo:** Evals funcionam como "rubricas" que permitem ao modelo ser avaliado de forma objetiva — análogo a uma prova com gabarito. Sem eval, não há como recompensar os comportamentos certos no RL, nem validar que uma capacidade foi adquirida. Isso torna evals o ativo estratégico central de qualquer lab ou empresa construindo em cima de IA.

**Mercado:** Há uma nova categoria de trabalho humano especializado em escrever evals — mais bem-paga que crowdsourcing tradicional porque requer expertise real. Top 10% dos contribuidores geram maioria do impacto de melhoria de modelos.

🎧 [Why experts writing AI evals is creating the fastest-growing companies in history | Brendan Foody (1:07:08)](https://www.youtube.com/watch?v=ja6fWTDPQl4) · 2025-09-18

---

## [[Hamel Husain]] & [[Shreya Shankar]] — A metodologia prática de evals para builders (2025-09-25)

> "Evals é uma forma de medir e melhorar sistematicamente uma aplicação de IA. No fundo é análise de dados do seu aplicativo de LLM — data analytics — com uma forma sistemática de olhar esses dados, criar métricas e iterar com confiança." — Hamel

> "Evals é um grande espectro de formas de medir a qualidade da aplicação. Unit tests são só uma pequena parte desse grande quebra-cabeça." — Shreya

**O processo completo (demonstrado ao vivo com caso real da Nurture Boss):**

### Fase 1 — Error Analysis / Open Coding
Amostrar ~100 traces (logs de interação), anotar o primeiro erro visível em cada um de forma livre e descritiva. Não tentar categorizar ainda — apenas capturar. O objetivo é desenvolvimento de intuição sobre o que está errado.

> "Quando as pessoas fazem esse processo de olhar os dados, ficam imediatamente viciadas. Você aprende muito sobre sua aplicação em muito pouco tempo." — Hamel

> "Não há nenhum LLM que consiga fazer essa parte da análise pelo humano. Eu apostaria dinheiro nisso. Se você colocar uma alucinação sobre tour virtual no ChatGPT e perguntar 'tem algum erro?', ele vai dizer 'não, fez ótimo trabalho'. Mas Hamel tinha o contexto de que a empresa não oferece tour virtual." — Shreya

**Conceito do "benevolent dictator":** Não use um comitê para decidir o que é erro. Designe uma pessoa com expertise de domínio como a "ditadora benevolente" — ela define o que é certo e errado. Processo por comitê torna o eval caro demais para manter.

### Fase 2 — Axial Coding (LLM para organizar)
Exportar as notas como CSV e pedir a um LLM para agrupar em categorias de falha (axial codes). Revisar as categorias e torná-las específicas e acionáveis (não genéricas como "capability limitations").

> "O que as pessoas geralmente fazem é pular direto para os testes. Isso é onde as coisas saem dos trilhos. Você precisa primeiro fazer análise de dados para saber o que realmente merece um eval." — Hamel

> "Os termos open coding e axial coding vêm das ciências sociais — não é algo que inventamos. Se alguém te traz uma forma de fazer algo inteiramente nova sem embasamento em centenas de anos de teoria, você devia ser um pouco cético." — Shreya

### Fase 3 — Contagem (pivot table)
Usar a planilha para contar frequência de cada categoria de falha. A técnica de contagem simples é subestimada — é poderosa porque vai do caos a prioridades claras em minutos.

> "Basic counting is the most powerful analytical technique in data science because it's so simple and it's undervalued." — Hamel

### Fase 4 — LLM como Juiz (para falhas subjetivas)
Para modos de falha que não são capturáveis com código simples (ex.: "deveria ter transferido para um humano?"), criar um LLM judge com output binário true/false. Validar o juiz contra as anotações humanas via **matriz de confusão** — não apenas % de concordância.

> "Você não quer escrever um eval com escala de 1 a 5. Isso é uma forma covarde de não tomar uma decisão. Você precisa decidir: isso é bom o suficiente ou não? Quando você reporta as métricas, ninguém sabe o que 3.2 versus 3.7 significa." — Hamel

> "Quando as pessoas perdem confiança nos seus evals, perdem confiança em você. É crítico que você valide seu juiz." — Hamel

**Erros comuns identificados:**
- Criar o prompt de juiz e confiar nele sem validar contra humano.
- Usar apenas % de concordância (enganoso quando erros são raros).
- Escala Likert ao invés de binário.
- Pular a análise de erros e ir direto para os testes.

**Sobre o debate "evals vs. vibe checks":**
> "Dogfooding é perigoso só porque muitas pessoas dizem que estão dogfooding mas não estão de verdade — não estão com aquela viscosidade necessária para fechar o loop de feedback." — Hamel

> "Coding agents como Claude Code estão de pé nos ombros dos evals que os colegas fizeram para os modelos de coding. Não existe mundo em que eles estão sendo como, 'fiz o Claude Code, nunca vou olhar nada'." — Shreya

**Sobre o debate "evals vs. A/B tests":**
> "A/B tests são mais uma forma de eval — você tem uma métrica que quantifica sucesso de algo e está comparando. Não dá para fazer A/B test sem um eval para comparar. Talvez só tenhamos um jeito diferente de ver isso." — Shreya

**Tempo investido:**
- Setup inicial: 3–4 dias para rodar o processo completo e criar os primeiros LLM judges.
- Manutenção: ~30 minutos por semana depois do setup.
- Quantidade de LLM judges necessários: 4 a 7 por produto típico.

🎧 [Why AI evals are the hottest new skill for product builders | Hamel Husain & Shreya Shankar (1:46:33)](https://www.youtube.com/watch?v=BsWxPI9UM4c) · 2025-09-25

---

## Síntese — Por que evals se tornaram a habilidade mais importante

Três perspectivas convergentes:

1. **Nível de modelo/lab** (Brendan Foody): evals são o gargalo para melhorar fundação de modelos; sem eval, não há RL, não há validação de capacidade.
2. **Nível de produto de IA** (Hamel + Shreya): evals são a forma sistemática de entender o que está errado com sua aplicação de LLM, priorizar melhorias e testar regressões.
3. **Nível de PRD** (Lenny + Shreya): "evals são os novos PRDs" — o prompt do LLM judge captura as expectativas do PM de forma explícita, verificável e que melhora iterativamente com os dados reais.

O que unifica: em sistemas estocásticos (como LLMs), não há garantia de comportamento — só medição sistemática. Evals são a infraestrutura de qualidade do desenvolvimento de produtos de IA, análoga a testes unitários + analytics + QA no desenvolvimento de software tradicional — mas com técnicas adaptadas ao não-determinismo.
