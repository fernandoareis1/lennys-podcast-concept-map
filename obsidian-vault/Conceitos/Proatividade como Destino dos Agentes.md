---
tipo: framework
nivel: 3
fluxo: Estratégia & Visão
autores: [Alexander Embiricos]
---
# Proatividade como Destino dos Agentes
**Fluxo:** [[02 - Estratégia & Visão]] · **Tema:** [[Estratégia — Estratégia de produto]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Alexander Embiricos]]

## Ideia central
O modelo atual de IA é **reativo**: a IA só ajuda quando você a chama. O usuário médio interage com IA dezenas de vezes por dia — mas poderia se beneficiar milhares de vezes por dia se a IA fosse "útil por padrão". O gargalo fundamental não é a capacidade do modelo, mas o **custo de prompting humano**: velocidade de digitação e capacidade de multitarefa limitam quanto a IA pode fazer por você. A destinação estratégica dos agentes é a proatividade: um agente que entende o contexto do que você está tentando fazer e age sem você ter que solicitá-lo explicitamente. Isso exige que o agente valide seu próprio trabalho — se o humano ainda precisa revisar cada output, o gargalo de velocidade humana não foi removido.

## Como aplicar
1. **Meça o "potencial de proatividade"**: quantas vezes por dia seu produto poderia ajudar o usuário vs. quantas vezes ele de fato ajuda? O gap é a oportunidade.
2. **Construa validação antes de autonomia**: para que o agente seja proativo, ele precisa saber quando acertou. Invista em evals, testes automatizados e heurísticas de auto-verificação antes de ampliar o escopo.
3. **Gradone a autonomia por tipo de tarefa**: comece com as tarefas onde o custo de erro é baixo (responder perguntas) antes de delegar as de alto risco (fazer push de código para produção).
4. **Projete para "mixed initiative"**: não é binário (humano faz tudo vs. agente faz tudo). O ponto ótimo é o agente agir proativamente em domínios seguros e surfaçar ações sugeridas para aprovação rápida nas demais.
5. **Trate o onboarding como construção de confiança**: a progressão natural é perguntar → alinhar abordagem → delegar subtarefa → delegar tarefa completa → agente proativo. Projete o produto para guiar o usuário nessa jornada.

## Insights por autor
### [[Alexander Embiricos]]
- "Se você não está promptando um modelo para ajudá-lo, ele provavelmente não está ajudando. Se você pensar em quantas vezes o usuário médio prompta IA hoje, são dezenas de vezes. Mas se você pensar em quantas vezes as pessoas poderiam se beneficiar de uma entidade realmente inteligente, são milhares de vezes por dia."
- O gargalo subestimado: "A limitante atual não é a inteligência do modelo — é literalmente a velocidade de digitação humana ou a velocidade de multitarefa do humano."
- Analogia do intern: Codex hoje é "um intern muito inteligente que se recusa a ler o Slack e não checa o Datadog a não ser que você peça." A meta é um colega que você não precisa microgerenciar.
- "Um dos nossos grandes objetivos com Codex é chegar à proatividade. Acho que isso é criticamente importante para cumprir a missão da OpenAI."
- Métricas que importam: D7 retention e observação de social media (Reddit > Twitter para feedback real, por ser menos hype e ter mecânica de upvote). Testar o produto "como um novo usuário" periodicamente.

> 🎧 [Building Codex: OpenAI's coding agent (1:16:34)](https://www.youtube.com/watch?v=xZifSLGOrrw)

## Conceitos relacionados
[[Código como Linguagem Universal dos Agentes]] · [[Assistência Contextual Mista]] · [[Trade-off Agência-Controle]] · [[Non-determinismo em Produtos de IA]] · [[Estratégia — Estratégia de produto]]
