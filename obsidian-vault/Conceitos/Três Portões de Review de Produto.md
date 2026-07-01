---
tipo: framework
nivel: 3
fluxo: Priorização & Roadmap
autores: [Nickey Skarstad]
---
# Três Portões de Review de Produto
**Fluxo:** [[03 - Priorização & Roadmap]] · **Tema:** [[Priorização — Estratégia vs execução]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Nickey Skarstad]]

## Ideia central
Reviews de produto falham quando acontecem tarde demais, quando são silos de função (design review aqui, tech review lá) ou quando aprovam a implementação mas não o problema. O antídoto é estruturar **três portões sequenciais**, cada um com o conjunto certo de pessoas e o conjunto certo de perguntas — e o portão mais importante é o primeiro.

**Os três portões:**

1. **Primeiro princípios** — *O que estamos tentando resolver?*
   O portão mais crítico. Se o time está resolvendo o problema errado, todo esforço subsequente é desperdício. Perguntas: qual é o outcome desejado? Quais são as restrições e os princípios que guiam a solução? O que estamos explicitamente não resolvendo? Aprovação aqui é mais valiosa do que aprovação técnica depois.

2. **Abordagem** — *Como vamos resolver?*
   Uma vez alinhados no problema, alinhar na solução. Inclui review técnico (arquitetura, infra) e de design (wireframes, fluxo). O cruzamento funcional aqui é crítico: design e engenharia precisam estar na mesma sala, não em silos separados.

3. **Pronto para ship** — *Está bom o suficiente para ir?*
   Gate final antes do lançamento. Avaliação de qualidade, edge cases, e se a solução ainda reflete os princípios do portão 1. Não é "está perfeito" — é "está bom o suficiente para aprender".

**O erro mais comum**: times que só fazem o terceiro portão. Chegam ao "está pronto para ship?" depois de meses de trabalho, descobrem que não estavam resolvendo o problema certo, e refazem. Toda a dor está concentrada no fim em vez de no início.

**Times pequenos / pre-PMF**: os três portões podem ser uma única conversa. Em times grandes, precisam ser rituais explícitos com convite cross-funcional e pre-read obrigatório.

## Como aplicar
1. **Nunca pule o portão 1**: before qualquer design ou código, agende uma sessão de 30–60 min só para alinhar no problema. Doc de entrada: "o que acreditamos ser o problema e por quê". Doc de saída: primeiros princípios aprovados.
2. **Cross-funcional em todos os portões**: design reviews sem produto presentes e tech reviews sem design presentes garantem feedback em vácuo. Convite mínimo: PM + designer + engenheiro.
3. **Pre-read obrigatório**: documente o contexto antes de cada portão. Sem pre-read, a reunião vira sessão de atualização — não review.
4. **Dê autonomia nos dois-way doors**: nem toda feature precisa dos três portões. Items reversíveis e de baixo impacto devem ir direto. Reserve os portões para decisões de longa duração.
5. **Leadership plugada sem microgerenciar**: os portões são o momento de input da liderança — não para controlar, mas para garantir que o time não está invisível ao contexto estratégico.

## Insights por autor
### [[Nickey Skarstad]]
- "Aligning on [first principles] is almost the most important thing. It saves a lot of teams a lot of time when they get later in their feedback review process and people are like, 'You're not solving for the right thing.'"
- "Finding ways to make sure that those parts of your process are shared across each function, and you attend them and prepare for them as a team, really helps."
- "Giving teams autonomy to ship some things that you think are two-way doors — things that aren't going to conflate with the larger system — is incredibly important."
> 🎧 [Nickey Skarstad on translating vision into goals (1:00:54)](https://open.spotify.com/episode/6FKUgLvnlpyLOyMbykXm6u) · 2022-07-18

## Conceitos relacionados
[[Decisão como força de momentum]] · [[PR-FAQ — Trabalhar ao Contrário]] · [[Murder Board — Adversário como Filtro de Qualidade]] · [[GIST — Framework de Produto Orientado a Evidência]]
