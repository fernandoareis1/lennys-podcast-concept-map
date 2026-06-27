---
tipo: insight
nivel: 3
fluxo: Estratégia & Visão
autores: [Jason Droege]
---
# De Saber a Fazer — A Transição dos Agentes de IA

**Fluxo:** [[02 - Estratégia & Visão]] · **Tema:** [[Estratégia — Estratégia de produto]] · **Camada:** L3
**Tipo:** Insight · **Fontes:** [[Jason Droege]]

## Ideia central
A tendência central da IA agora é passar de modelos que *sabem coisas* para modelos que *fazem coisas*. Os benchmarks de conhecimento estão ficando robustos; a fronteira passou para ação e agência. A questão que os labs e produtos precisam responder não é mais "quanto sabe o modelo?" mas "o que ele pode fazer *por mim*?" Isso exige treinar agentes dentro de *ambientes* (sandboxes que simulam sistemas reais — Salesforce, healthcare records, calendários) para que aprendam a navegar situações específicas e a decidir quando pedir ajuda humana. A generalização é o problema: o número de combinações de ambiente + objetivo + cultura de empresa é quase infinito, então a estratégia é coletar dados generalizáveis o suficiente para cobrir a maior amplitude possível sem precisar cobrir cada permutação individualmente.

## Como aplicar
1. Ao avaliar onde investir em IA, distinga: o produto está no domínio do conhecimento (fácil, commoditizando) ou no domínio da ação/agência (hard, diferenciado)?
2. Para agentes: mapeie o conjunto de ambientes relevantes (ex: Salesforce, JIRA, sistema interno X) e priorize os mais generalizáveis.
3. Defina critério claro de quando o agente deve escalar para humano — a confiabilidade do "pop up to human" é tão importante quanto a taxa de acerto do agente.
4. "Easy to learn, hard to master" — adoção rápida cria falsa expectativa de deploy rápido; pipeline real leva 6-12 meses para robustez em processos críticos.
5. AI vai muito bem em melhorar processos com 10-20% de precisão humana atual; ainda luta para fechar o gap nos últimos 2% de processos com 98% de precisão.

## Insights por autor
### [[Jason Droege]]
- Modelos estão indo de "saber" para "fazer" — essa é a tendência que moldará os próximos 2-3 anos.
- A transição exige ambientes de RL (reinforcement learning) onde o agente aprende a navegar sistemas reais com objetivos reais.
- POCs chegam a 60-70% facilmente; o resto é como "cada nine em uptime de datacenter" — ordem de magnitude de investimento para cada passo.
- Experts humanos são bottleneck crescente: cada empresa tem seu próprio "julgamento" que precisa ser digitalizado para que o agente opere no contexto correto.
> 🎧 [Scale AI CEO on Meta's $14B deal, scaling Uber Eats to $80B | Jason Droege (1:24:02)](https://www.youtube.com/watch?v=W99jdYZOlN0)

## Conceitos relacionados
[[Proatividade como Destino dos Agentes]] · [[Trade-off Agência-Controle]] · [[Era dos evals — o eval é o PRD do modelo]] · [[Estratégia — Estratégia de produto]]
