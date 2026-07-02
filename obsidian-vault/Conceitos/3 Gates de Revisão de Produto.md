---
tipo: tecnica
nivel: 3
fluxo: Discovery & Pesquisa
autores: [Nickey Skarstad]
---
# 3 Gates de Revisão de Produto

**Fluxo:** [[01 - Discovery & Pesquisa]] · **Tema:** [[Discovery — Descoberta contínua & validação]] · **Camada:** L3
**Tipo:** técnica · **Fontes:** [[Nickey Skarstad]]

## Ideia central
Revisões de produto que acontecem só ao final — quando tudo já foi desenhado e codificado — geram feedback do tipo "você está resolvendo o problema errado." Isso destrói tempo e moral. A solução é três checkpoints cross-funcionais ao longo do processo, não apenas um ao final.

## Os 3 Gates

### Gate 1 — First Principles
- **Quando:** antes de qualquer design ou código
- **Pergunta:** O quê exatamente estamos tentando fazer? Quais são as premissas fundamentais? O que mais importa? O que *não* importa?
- **Output:** alinhamento em first principles; quem assiste: PM, design, eng, liderança relevante
- **Por que é o mais importante:** 90% dos "você errou o alvo" acontecem aqui. Resolver cedo é 10× mais barato.

### Gate 2 — Approach & Architecture
- **Quando:** depois do design exploratório e antes de codificação pesada
- **Pergunta:** Qual abordagem vamos usar? A solução resolve os first principles? Há considerações técnicas críticas? (infrastructure review, architecture review)
- **Output:** direção de solução aprovada; flags técnicos antecipados

### Gate 3 — Ship-Ready Review
- **Quando:** produto pronto para lançar
- **Pergunta:** Isso atinge nosso goal? Atinge nosso quality bar? Liderança está informada e sem surpresas?
- **Output:** aprovação de lançamento ou lista de blockers finais

## Princípios de operação
- **Cross-funcional:** cada gate inclui PM + design + eng + liderança relevante — *não* revisões separadas por função sem comunicação entre si
- **Pré-read obrigatório:** material enviado antes para que o tempo de reunião seja debate, não apresentação
- **Two-way door viajam sem gate:** features reversíveis e de baixo impacto não precisam passar pelos 3 gates; reserve o processo para decisões com peso
- **Times pequenos simplificam:** com 2-3 pessoas no time, os gates acontecem informalmente; escalar o processo conforme cresce

## O problema que resolve
> "Where I've seen them fail is when they happen at the function level, and they're not done or shared as a team. The design leader will give the designer feedback, and then you don't hear about it. Or there'll be some technical flaw that happens in a very specific technical review that doesn't get back to the larger team."
> — Nickey Skarstad

## Insights por autor
### [[Nickey Skarstad]]
- "Getting approval on [first principles] is almost the most important thing. Because it saves a lot of teams a lot of time when they get later in their feedback review process and people are like, 'You're not solving for the right thing.'"
- "I think that, again, it depends on your organization. If you have a very small team, you might be very plugged in and these things might not need to happen."

> 🎧 [Nickey Skarstad (Airbnb, Etsy, Shopify, Duolingo) on translating vision into goals](https://open.spotify.com/episode/6FKUgLvnlpyLOyMbykXm6u)

## Conceitos relacionados
[[Discovery-Delivery em Paralelo, Não em Sequência]] · [[One Way vs Two Way Door — Reversibilidade de Decisão]] · [[Canonical Doc]]
