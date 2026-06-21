---
tipo: insight
nivel: 3
fluxo: Estratégia & Visão
autores: [Alexander Embiricos]
---
# Proatividade como Meta dos Agentes
**Fluxo:** [[02 - Estratégia & Visão]] · **Tema:** [[Estratégia — Estratégia de produto]] · **Camada:** L3
**Tipo:** Insight · **Fontes:** [[Alexander Embiricos]]

## Ideia central
Hoje, produtos de IA são reativos: o usuário precisa pensar ativamente em quando e como invocar o modelo. Isso limita o benefício a dezenas de interações por dia, quando o potencial real é de **milhares de interações diárias** — se o agente for proativo. A meta de longo prazo para agentes como o Codex é que eles ajam **sem precisar ser solicitados**: monitoram contexto, identificam oportunidades e surfaceiam ajuda no momento certo, em vez de esperar um prompt. Proatividade não é notificação em massa — é ação contextual integrada ao fluxo do usuário, invisível quando desnecessária e presente quando relevante.

## Como aplicar
- **Mapeie onde o usuário mais se beneficiaria sem saber pedir**: revisão de código, alertas de métrica, bugs em produção — são pontos onde ajuda contextual tem alto valor e baixo custo de interrupção.
- Evite o modelo de push notification: 1.000 notificações por dia é ruim. A alternativa é ação contextual onde o usuário já está (no dashboard, no editor, no browser).
- Para habilitar proatividade, o agente precisa de **acesso ao contexto ambiental**: o que o usuário está vendo, qual código está aberto, qual métrica está em queda. Isso motiva produtos como browsers próprios ou IDE integrados.
- A jornada de proatividade é progressiva: primeiro o usuário aprende a delegar tarefas explicitamente; o agente ganha contexto acumulado; depois, ele começa a agir com menos solicitação explícita.
- Proatividade requer que o agente valide o próprio trabalho (testes, build, preview) — caso contrário, ele fica preso pedindo confirmação a cada passo.

## Insights por autor
### [[Alexander Embiricos]]
- "Produtos de IA hoje são difíceis de usar porque você tem de pensar ativamente sobre quando eles podem te ajudar. Se você não prompta o modelo, ele não está te ajudando. E o usuário médio prompta dezenas de vezes por dia — quando o potencial é de milhares."
- "Um dos nossos grandes objetivos com o Codex é chegar à proatividade." Isso é tratado como meta de produto de longo prazo, não feature.
- Hipótese provocativa: no futuro, um solopreneur poderia ter um app que mostra, em vídeo vertical, ideias e ações que o agente sugere — e o humano apenas desliza left/right para aprovar ou rejeitar. Interação no menor esforço possível.
- A analogia do Halo: num jogo, você chega perto de um objeto e aperta X — a ação certa aparece no momento certo. Esse é o modelo de UX para agentes proativos.
- O Goose (Block) já está fazendo isso em embrião: um engenheiro deixa o agente ouvir suas reuniões e assistir a tela; ele abre PRs, rascunha Slack mensagens e envia emails proativamente.

> 🎧 [Building the future of coding agents | Alexander Embiricos (OpenAI Codex)](https://www.youtube.com/watch?v=xZifSLGOrrw) (1:16:34)

## Conceitos relacionados
[[Agente de Coding como Fundação Universal]] · [[Escada de Agência-Controle em IA]] · [[Não-Determinismo em Produtos de IA]] · [[Compressão do Stack de Talentos com IA]]
