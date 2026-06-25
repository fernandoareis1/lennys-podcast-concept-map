---
tipo: framework
nivel: 3
fluxo: Priorização & Roadmap
autores: [Itamar Gilad]
---
# GIST Framework — Goals, Ideas, Steps, Tasks
**Fluxo:** [[03 - Priorização & Roadmap]] · **Tema:** [[Priorização — Outcomes & metas]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Itamar Gilad]]

## Ideia central
GIST é uma meta-framework que organiza o trabalho de produto em 4 camadas aninhadas, forçando o time a conectar **metas** a **descoberta** a **entrega** — em vez de pular direto de opinião para código. É o antídoto ao "plan and execute" (decidir o que construir baseado em opiniões e então construir).

**As 4 camadas:**
- **G — Goals (Metas)**: onde queremos chegar. Definidas em 2 dimensões: North Star metric (valor entregue ao usuário) + Top KPI (valor capturado pelo negócio). Métricas organizadas em **metrics trees** — decompõem as métricas principais até o nível de time. Os nós onde as duas árvores se sobrepõem são os mais importantes.
- **I — Ideas (Ideias)**: hipóteses sobre como chegar às metas. Avaliadas pelo ICE (Impact × Confidence × Ease). A chave: a confiança deve ser calibrada por evidência (ver Medidor de Confiança), não por convicção.
- **S — Steps (Passos)**: maneiras de implementar E validar uma ideia ao mesmo tempo. Não são marcos de engenharia — são marcos de aprendizado. Escala: Wizard of Oz → fish food → dog food → AB test → release stagings. Cada step gera evidência que atualiza a confiança na ideia.
- **T — Tasks (Tarefas)**: o que vai para Jira/Kanban. Surge dos steps.

**O que muda em relação ao modelo comum:**
- Times normais vivem em dois mundos desconectados: **mundo do planejamento** (gestores/roadmaps) e **mundo da execução** (devs/kanban). O PM fica no meio tentando traduzir.
- GIST conecta os dois ao criar um terceiro espaço (a camada de Steps/Ideas) que é de responsabilidade do time — e que inclui devs no processo de descoberta.

**GIST Board**: artefato por time, atualizado a cada 2 semanas. Máximo: 4 key results + 2-3 ideias ativas + próximos steps. Não é roadmap de release — é roadmap de aprendizado.

## Como aplicar
1. **Comece com as metas certas**: identifique North Star metric (valor criado para usuários) e o Top KPI (valor capturado). Construa a metrics tree — 2 ou 3 camadas. Distribua sub-métricas por times.
2. **Use ICE com Confidence calibrada**: para cada ideia, score Impact e Ease (1-10). Para Confidence, use o Medidor de Confiança — não deixe o time dar 8/10 de confiança baseado em pitch deck.
3. **Mapeie os Steps antes de codar**: antes de qualquer sprint, pergunte: qual é a forma mais barata de testar a premissa central desta ideia? Fake door? Wizard of Oz? Entrevistas com mockup?
4. **Implemente o GIST Board**: uma vez a cada 2 semanas, o time revisa: estamos nas metas certas? As ideias que testamos têm evidência suficiente? Quais steps corremos e o que aprendemos?
5. **Separe roadmap de release de roadmap de outcomes**: datas de lançamento são úteis quando a ideia já tem alta confiança. Antes disso, o roadmap deve dizer "por Q3 queremos atingir X" — não "por Q3 vamos lançar Y".

## Insights por autor
### [[Itamar Gilad]]
- Origem: Google+ foi opinion-based development. 1000 engenheiros, anos de trabalho, zero de produto-mercado. Google Tabs foi evidence-guided. Sem linha de código antes de validar com Wizard of Oz manual.
- "Google+, at its peak, had about 1000 people. It was a division the size of Android and Docs. And none of it worked because people actually didn't need another social network."
- "The metric is not how fast can we get the bits into production, when there's a lot of uncertainty. It's about getting the right bits to production. It's about time to outcomes."
- "We've got developers very focused on moving tickets to the done state, on burning story points, pushing stuff into production — and they're disengaged from the users and the business. That's something you can fix by adopting a more evidence-guided system."
- "If you do the GIST board, you create a lot more context in the minds of your team and then they need to ask you fewer questions. You need to tell them less what to do."
- Sobre a escala por tamanho de empresa: "Early stage companies even don't know how they create value, so their goal is really to find product market fit. Beyond that, when you move into scale, you need order — a systematic way to evaluate ideas because you get a lot of people and a lot of money and everything is happening at the same time."

> 🎧 [Becoming evidence-guided (1:12:52)](https://www.youtube.com/watch?v=aJWSn-tz3jQ) · 2023-09-21

## Conceitos relacionados
[[Medidor de Confiança — Calibrando Evidência antes de Investir]] · [[ICE (priorização)]] · [[OKRs (Christina Wodtke)]] · [[Continuous Discovery]] · [[Priorização — Outcomes & metas]] · [[A maioria das ideias falha no teste]]
