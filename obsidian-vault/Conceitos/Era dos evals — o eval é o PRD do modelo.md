---
tipo: framework
nivel: 3
fluxo: Estratégia & Visão
autores: [Brendan Foody, Hamel Husain, Shreya Shankar]
---
# Era dos evals — o eval é o PRD do modelo
**Fluxo:** [[02 - Estratégia & Visão]] · **Tema:** [[Estratégia — Estratégia de produto]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Brendan Foody]]

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
- "Evals é uma forma de medir e melhorar sistematicamente uma aplicação de IA — no fundo, é data analytics no seu app de LLM."
- "A atividade de maior ROI que você pode fazer ao construir um produto de IA é olhar os seus dados (traces)."
- "Quando você está construindo um app de IA e encontra algo errado, vá lá e conserte. O objetivo não é ter uma bela suite de evals — é melhorar a aplicação."
> 🎧 [Why AI evals are the hottest new skill for product builders (1:46:33)](https://www.youtube.com/watch?v=BsWxPI9UM4c)

### [[Shreya Shankar]]
- "O eval é a especificação viva do produto: você descobre falhas que nunca teria imaginado antes de ver os dados. Isso vai mudar o seu PRD."
- "Existem muitas formas incorretas de fazer evals, mas também muitas formas corretas. Depende de onde você está no produto e dos recursos disponíveis."
> 🎧 [Why AI evals are the hottest new skill for product builders (1:46:33)](https://www.youtube.com/watch?v=BsWxPI9UM4c)

## Aprofundamento ⬇
- [[Era dos evals — Evidências]]

## Conceitos relacionados
[[Análise de Erro com Open Coding]] · [[LLM como Juiz — Avaliador Binário]] · [[IA Constitucional]] · [[Non-determinismo em Produtos de IA]] · [[OEC - Overall Evaluation Criterion]]
