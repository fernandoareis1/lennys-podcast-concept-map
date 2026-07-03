---
tipo: framework
nivel: 3
fluxo: Experimentação & Dados
autores: [Sander Schulhoff]
---
# Prompt Engineering de Produto vs. Conversacional

**Fluxo:** [[05 - Experimentação & Dados]] · **Tema:** [[Experimentação — Aprender com pouco e qualitativo]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Sander Schulhoff]]

## Ideia central
Há dois modos fundamentalmente distintos de prompt engineering, e a maioria das pessoas só conhece um:

**Modo conversacional:** você usa Claude ou ChatGPT, pede algo, o resultado não é bom, você refina. "Torne mais formal." "Adicione uma piada." Você vê cada output e ajusta em tempo real.

**Modo produto (product-focused):** você tem um ou alguns prompts críticos que rodam para milhares ou milhões de inputs por dia. Você não vai ver os outputs individuais. Você precisa que esse prompt funcione com robustez estatística. A maioria da pesquisa acadêmica é sobre esse modo.

**Por que isso importa para PMs:** no modo conversacional, você pode ser informalmente preguiçoso — "escrever email mal escrito, melhorar" funciona. No modo produto, o nível de rigor é completamente diferente. Se 1 em cada 100 chamadas sai sem o raciocínio que você precisava, isso é uma falha de produto. No produto com um milhão de usuários, isso é 10.000 outputs ruins.

**As técnicas de maior ROI no modo produto:**
1. **Few-shot** — dar exemplos de input/output desejado. Boost enorme de performance. Mais eficaz junto com XML ou Q/A como formato.
2. **Informação adicional** — inserir contexto rico sobre a tarefa, empresa, domínio. Colocar no INÍCIO do prompt (cacheável; evita que o modelo esqueça a tarefa original se o contexto for longo).
3. **Decomposição** — para tarefas complexas: "antes de responder, liste os subproblemas que precisam ser resolvidos." Distribui trabalho para ferramentas/agentes diferentes.
4. **Auto-crítica** — após o output: "avalie sua resposta e sugira melhorias." Depois: "implemente essas melhorias." Free performance boost em muitas situações.
5. **Ensembling** — múltiplas instâncias do prompt com variações (diferentes roles, perspectivas); take the majority answer. Mais complexo mas consistentemente eficaz.

**O que NÃO funciona (mito popular):** role prompting ("você é um professor de matemática") não tem efeito estatisticamente significativo em tarefas de precisão/accuracy. Funciona para tarefas expressivas (escrita, estilo). Promessas de reward ("vou te dar $5 se fizer bem") também não têm efeito comprovado.

**Chain-of-thought / Think Step-by-Step:** ainda útil para modelos não-reasoning (GPT-4o). Desnecessário para modelos de reasoning como o3 que fazem isso por padrão.

## Como aplicar
1. **Identifique em qual modo você está**: se é para uso pessoal conversacional, relaxe; se é para um produto, invista em engenharia do prompt como código de produção.
2. **No modo produto**: use few-shot com no mínimo 3-5 exemplos de input/output desejado em formato consistente (XML ou Q/A).
3. **Inclua informação adicional no topo do prompt**: biogradia do usuário, contexto da empresa, domínio do problema. Esse contexto fica cacheado e barateia chamadas subsequentes.
4. **Para tarefas complexas, decomponha**: "antes de responder, liste os subproblemas" permite paralelizar com tool-calling agents.
5. **Abandone role prompting para accuracy**: se você usa "você é um expert em X" esperando melhorar accuracy, pare. Reserve para estilo e expressividade.

## Insights por autor
### [[Sander Schulhoff]]
- "Estudos mostraram que prompts ruins podem te derrubar para 0% num problema, e prompts bons podem te levar a 90%."
- "No modo produto, você tem que ter confiança em coisas que não vai ver. Com o modo conversacional, você vê o output imediatamente. No modo produto, milhões de usuários estão interagindo com esse prompt."
- "Role prompting não tem efeito estatisticamente significativo em tarefas de accuracy. Funciona para tarefas expressivas — escrita, estilo, sumarização."
- "Few-shot prompting e informação adicional providenciam provavelmente o maior uplift para prompt engineering conversacional. E são ainda mais críticos no modo produto."
- "Coloque a informação adicional no início do prompt. Isso faz ela ser cacheada — chamadas subsequentes com o mesmo contexto ficam muito mais baratas."

> 🎧 [AI prompt engineering in 2025: What works and what doesn't | Sander Schulhoff (1:37:47)](https://www.youtube.com/watch?v=eKuFqQKYRrA) · 2025-06-19

## Conceitos relacionados
[[Era dos evals — o eval é o PRD do modelo]] · [[Intentionalidade Primeiro — O GPS não Escolhe o Destino]] · [[Contexto como Camada Diferenciadora de Produto IA]] · [[O que realmente melhora apps de IA]]
