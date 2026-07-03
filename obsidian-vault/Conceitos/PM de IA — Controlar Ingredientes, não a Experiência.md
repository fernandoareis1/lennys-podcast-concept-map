---
tipo: mindset
nivel: 3
fluxo: Estratégia & Visão
autores: [Tomer Cohen]
---
# PM de IA — Controlar Ingredientes, não a Experiência

**Fluxo:** [[02 - Estratégia & Visão]] · **Tema:** [[Estratégia — Estratégia de produto]] · **Camada:** L3
**Tipo:** Mindset · **Fontes:** [[Tomer Cohen]]

## Ideia central
O product manager tradicional controla a experiência: define o fluxo, as telas, os defaults, o onboarding — cada detalhe. Com IA no coração do produto, essa ilusão de controle desaparece. Você não controla mais a experiência; **você controla os ingredientes**.

A metáfora de Tomer: imagine um chef de restaurante que sempre decidiu cada detalhe do prato. Agora chega uma tecnologia que diz: "Me dê os ingredientes e as diretrizes de como você cozinha, e eu cuido do resto." Para muitos PMs, isso é assustador. O instinto é delegar a IA para o time de engenharia ou ML. O erro é exatamente esse.

## O que significa controlar ingredientes em AI products
Os "ingredientes" que o PM de IA deve controlar:

1. **Objetivo do algoritmo**: qual métrica matemática a IA está otimizando? PMs devem conseguir escrever isso num quadro. No feed do LinkedIn, mudaram de CTR (click-through rate) para downstream engagement — o que mudou completamente o comportamento dos spammers (que saíram) e dos criadores legítimos (que se sentiram mais recompensados).

2. **Features do algoritmo**: não features de UX, mas parâmetros nos quais o modelo aprende. Quais sinais são inputs? Quais são excluídos?

3. **Estratégia de dados e fine-tuning**: quem coleta quais dados, com que cadência, para qual objetivo de treinamento? Isso não é responsabilidade só do time de ML — é responsabilidade do PM porque determina para onde o produto vai.

4. **Infraestrutura**: PMs raramente falam sobre infraestrutura, mas mudar a infraestrutura pode ser o maior alavancador de outcome — maior do que lançar uma nova feature de UX.

## A transição do mindset
| PM tradicional | PM de IA |
|---|---|
| Controla cada tela e fluxo | Define objetivos e dados; a IA cria a experiência |
| Testa variações de UX | Testa objetivos de algoritmo e features |
| Faz handoff de dados/ML para eng | Lidera estratégia de dados e fine-tuning |
| Ignora infraestrutura | Investe em infraestrutura como alavanca de produto |
| Onboarding fixo | Onboarding adaptivo baseado em sinais do usuário |

## Como o LinkedIn implementou
- Criação de uma "AI academy" interna: todo PM passou por treinamento, assim como fizeram com mobile em 2014
- Revisões de produto focadas em "qual é o objetivo do seu algoritmo?" e "quais features você adicionou?"
- Times dedicados de AI practitioners no lado de produto (não só engenharia)
- Em fall 2022 (antes do ChatGPT público): descartaram os roadmaps existentes e pediram que cada time voltasse ao problema que tentavam resolver — agora com LLMs disponíveis, qual seria a solução?

## Insights por autor
### [[Tomer Cohen]]
- "You don't control the experience anymore, you control the ingredients. It's almost like being a chef at a restaurant... just give me the ingredients, give me the guidelines of how you cook and now I'll take care of it."
- "What is the objective of the algorithm? They should be able to write it down on a board. It's ultimately a mathematical formula."
- "You can build a whole strategy just on data collection and fine-tuning and your product will see tremendous success — or you can delegate it and it will never happen."
- "AI is not deterministic. Giving it the rope to learn and do that experience for you ultimately becomes much, much better. You have to have that belief going into it."
- "How many product people talk about the infrastructure they have? Not many. Just changing the infrastructure could be the biggest lever — bigger than building another button or experience for your members."

> 🎧 [Why AI is disrupting traditional product management | Tomer Cohen](https://www.youtube.com/watch?v=R-zCfLQD_84) · ~36:00-44:00

## Conceitos relacionados
[[Era dos evals — o eval é o PRD do modelo]] · [[Armadilha do AI por AI]] · [[Produto que Melhora com o LLM — Anti-Compensação]] · [[Viabilidade na Era do GenAI]] · [[O que realmente melhora apps de IA]]
