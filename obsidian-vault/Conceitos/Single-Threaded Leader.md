---
tipo: framework
nivel: 3
fluxo: Liderança & Times
autores: [Bill Carr]
---
# Single-Threaded Leader
**Fluxo:** [[09 - Liderança & Times]] · **Tema:** [[Liderança — Modelos de time]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Bill Carr]]

## Ideia central
Em organizações complexas, recursos centralizados (engenharia, dados, design) são disputados por múltiplos times. A maioria das empresas resolve com processo centralizado de priorização — reuniões, planos, arbitragem constante. A Amazon foi na direção oposta: **cada área de produto tem um único líder com todos os recursos necessários dedicados a ela** (subordinados diretos ou dedicados).

A mudança fundamental é de **orientação de projeto** (time swarm numa feature por 6 meses, depois dispersa) para **orientação de programa** (time permanente que evolui continuamente sua área, tem métricas próprias, define seu próprio roadmap). O resultado: ownership real, velocidade e accountability clara. Se algo vai bem ou mal, é responsabilidade daquele líder e time — não há "empurra" para coordenação compartilhada.

**O trade-off**: perda potencial de excelência funcional. Time de engenharia espalhado em micro-squads não tem mais um CTO como coach do dia a dia. A Amazon criou **contrameasures** (reviews de promoção cross-organizacional, padrões técnicos de código/entrevista gerenciados centralmente, VPs com "segundo emprego" de representar a função no processo de senioridade).

## Como aplicar
1. **Pré-requisito técnico**: decomponha o monolito em serviços com APIs bem documentadas. Sem isso, times não conseguem agir independentemente.
2. **Defina o escopo com o teste das três perguntas**: o time tem (a) recursos suficientes para mover suas métricas? (b) limites claros com outros times? (c) ownership de um P&L ou outcome mensurável?
3. **Crie contrameasures para excelência funcional**: standards centrais de entrevista, processos de promoção cross-org, revisões técnicas compartilhadas. Não abandone a função ao descentralizar.
4. **Alinhe o plano antes de soltar o time**: revisão intensiva com liderança sênior sobre o que o time vai construir → após alinhamento, o time sprint sem precisar recalibrar todo mês.
5. **Mude o papel da liderança sênior**: de "árbitro de roadmap item a item" para "árbitro de qual time tem quantos recursos" (decisão anual, não semanal).

## Insights por autor
### [[Bill Carr]]
- "Movemos de orientação de projeto para orientação de programa. Um time que sempre trabalha em search pensa holisticamente sobre search, não sobre este projeto específico."
- "O benefício: se tem sucesso ou falha, depende deles. O único argumento que podem fazer é 'precisamos de mais recursos' — não ficam culpando outros times."
- "Ao invés de liderança arbitrar cada item do roadmap — uma decisão diária — eles arbitram quais times têm quantos recursos — uma decisão 1-3 vezes por ano."
- "Você precisa criar contrameasures. Eu nunca escrevi uma linha de código em 20 anos. Não poderia conduzir um code review. Precisávamos de Rick Dalzell criando padrões técnicos para a empresa toda."
- "A string empurra: quando não há um dono claro e responsável por uma iniciativa, o CEO está empurrando uma corda."
> 🎧 [Unpacking Amazon's unique ways of working (1:33:28)](https://www.youtube.com/watch?v=S9WHQa_AJQo) · 2023-11-02

## Conceitos relacionados
[[Empowered Teams vs Feature Teams]] · [[Product Trio]] · [[Organizações como Slime Mold]] · [[PM responsável por valor e viabilidade]]
