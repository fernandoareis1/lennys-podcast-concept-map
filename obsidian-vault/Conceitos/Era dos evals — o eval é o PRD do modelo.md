---
tipo: framework
nivel: 3
fluxo: Estratégia & Visão
autores: [Brendan Foody, Hamel Husain, Shreya Shankar, Karina Nguyen, Kevin Weil]
---
# Era dos evals — o eval é o PRD do modelo
**Fluxo:** [[02 - Estratégia & Visão]] · **Tema:** [[Estratégia — Estratégia de produto]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Brendan Foody]] · [[Hamel Husain]] · [[Shreya Shankar]] · [[Karina Nguyen]] · [[Kevin Weil]]

## Ideia central
"Se o modelo é o produto, o eval é o PRD." O gargalo primário para a melhoria de modelos de IA não é dados de pré-treino — é a capacidade de **definir o que é sucesso** em cada domínio que o modelo precisa dominar. Sem um eval, não há como medir progresso, recompensar os comportamentos certos no RL, ou validar que uma capacidade foi adquirida.

**O que é um eval (na prática):**
Um eval é um conjunto de critérios e exemplos que permite medir se o modelo entregou o output correto para um determinado tipo de tarefa. É análogo a uma rubrica que um professor dá a um assistente de ensino para corrigir provas. A diferença é que aqui a "prova" é resolvida pelo modelo e o "professor" é um expert humano que definiu o critério.

**Por que dominar evals é urgente para empresas:**
- Toda capacidade que você quer que o modelo execute precisa de um eval primeiro.
- "Evals = novo marketing": labs usam evals como sales collateral para demonstrar capacidades de forma objetiva. Empresas que criam evals para seus workflows próprios provam (para si e para parceiros) o que o modelo sabe fazer.
- Evals são escaláveis via RLAIF: o human feedback pode se tornar o verifier, e o modelo aprende a atingir o critério autonomamente.
- Empresas que se recusam a evaliar seus processos por medo de revelar vulnerabilidades estão se atrasando deliberadamente em adotar IA.

**Mercado de evals como negócio:**
O mercado de trabalho humano especializado em escrever evals é uma nova categoria — mais bem-paga que o crowdsourcing antigo porque requer expertise real. Os top 10% dos contribuidores geram a maioria das melhorias de modelo (análogo a uma empresa: top 10% dos funcionários entregam maioria do impacto).

## Insights por autor
### [[Brendan Foody]]
- "Se o modelo é o produto, o eval é o PRD — mas também o material de vendas. Os labs usam evals para demonstrar as capacidades dos seus modelos."
- "O gargalo primário dos labs para melhorar modelos é como eles podem medir efetivamente o que parece sucesso para o modelo."
- "A barreira para aplicar agentes em toda a economia para automatizar qualquer workflow é: como medimos sucesso? Como fazemos o eval?"
- "Os modelos são apenas tão bons quanto seus evals."
- "Toda a economia vai provavelmente se tornar uma máquina de ambiente de evals, construindo mundos e contextos para que haja rubrics ou verificadores."

> 🎧 [Why experts writing AI evals is creating the fastest-growing companies in history | Brendan Foody (1:07:08)](https://www.youtube.com/watch?v=ja6fWTDPQl4) · 2025-09-18

### [[Hamel Husain]]
- "Evals é uma forma de medir e melhorar sistematicamente uma aplicação de IA — no fundo é análise de dados do seu aplicativo de LLM com métricas para iterar com confiança."
- "As pessoas vão direto para os testes sem fazer análise de dados primeiro. Isso é onde as coisas saem do trilho."
- "A atividade de maior ROI que você pode fazer ao construir um produto de IA é construir bons evals e olhar os seus dados regularmente."
- O processo: error analysis (olhar traces → open coding) → axial coding com LLM → contagem → LLM como juiz para falhas complexas.

> 🎧 [Why AI evals are the hottest new skill for product builders | Hamel Husain & Shreya Shankar (1:46:33)](https://www.youtube.com/watch?v=BsWxPI9UM4c) · 2025-09-25

### [[Shreya Shankar]]
- "O objetivo não é fazer evals perfeitamente — é melhorar seu produto de forma acionável."
- "O eval é o PRD: deriva das próprias expectativas do PM sobre o produto, mas melhora iterativamente conforme você olha os dados. Você nunca vai saber todos os modos de falha de antemão."
- "Pessoas foram queimadas por evals mal feitos — LLM judge com escala Likert, por exemplo. Daí ficaram 'anti evals'. Mas o problema é a execução, não o conceito."
- Unit tests, A/B tests e monitoramento online são todos formas de eval; a distinção rígida entre eles cria confusão desnecessária.

> 🎧 [Why AI evals are the hottest new skill for product builders | Hamel Husain & Shreya Shankar (1:46:33)](https://www.youtube.com/watch?v=BsWxPI9UM4c) · 2025-09-25

## Insights por autor
### [[Karina Nguyen]]
- Dois tipos de evals: **determinísticos** (pass/fail — "se o usuário diz 7PM, o modelo deve dizer 7PM") e **win-rate humano** (qual modelo produz o output de maior qualidade?).
- Formato prático: planilha com abas de "comportamento atual", "comportamento ideal", "notas" e "por quê" — pode ser passada ao o1 para ele descobrir como treinar o bom comportamento.
- "O eval mais robusto é o que faz o baseline promtado receber a pontuação mais baixa. Assim você sabe que, se treinou um bom modelo, ele vai subir nesse eval continuamente."
- Ensinou PMs e model designers a escrever evals — "product management of AI feature for AI models".
- Prompting como nova forma de prototipagem: o demo de 100K context com file uploads foi feito como protótipo em browser local antes de qualquer treinamento.
> 🎧 [OpenAI researcher on why soft skills are the future of work](https://www.youtube.com/watch?v=DeskgjrLxxs) · 2025-02-09

### [[Kevin Weil]]
- Evals como habilidade central do PM de IA: escrever evals é análogo a escrever unit tests para o produto.
- Evals determinam o que é possível construir: "entender se o modelo é 60% ou 99,5% confiável determina qual produto você pode construir."
- Usou evals para hill-climbing durante o treinamento do Deep Research — o eval define a direção do treino.
- "Escrever evals está se tornando uma habilidade central de PMs em empresas de IA, da mesma forma que análise de dados se tornou no ciclo anterior."
- A distinção entre "o modelo sabe" e "o modelo faz de forma confiável" é capturada pelos evals — por isso são o gate de cada feature.

> 🎧 [OpenAI's CPO on why ChatGPT is the worst AI you'll ever use | Kevin Weil](https://www.youtube.com/watch?v=scsW6_2SPC4) · 2025-04-10

## Aprofundamento ⬇
- [[Era dos evals — Evidências]]

## Conceitos relacionados
[[Teste de Turing Econômico]] · [[IA Constitucional]] · [[Construir para o disco futuro]] · [[Non-determinismo em Produtos de IA]] · [[OEC - Overall Evaluation Criterion]] · [[Análise de erros qualitativa para produtos de IA]] · [[LLM como Juiz — avaliação automatizada de qualidade]]
