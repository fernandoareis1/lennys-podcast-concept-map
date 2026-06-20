---
tipo: framework
nivel: 3
fluxo: Estratégia & Visão
autores: [Alexander Embiricos]
---
# Stack de três camadas dos agentes
**Fluxo:** [[02 - Estratégia & Visão]] · **Tema:** [[Estratégia — Estratégia de produto]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Alexander Embiricos]]

## Ideia central
Um agente de IA útil em produção não é só um modelo — é um **sistema de três camadas** que precisam estar alinhadas: (1) o **modelo** (raciocínio + conhecimento da tarefa), (2) a **API/infraestrutura** (endpoints, gerenciamento de contexto, rate limits), e (3) o **harness** (o ambiente onde o modelo opera — ferramentas disponíveis, sandbox, compaction). Features significativas exigem trabalho nas três camadas simultaneamente; focar em apenas uma cria agentes bons no benchmark mas ruins em produção.

## Como aplicar
**Camada 1 — Modelo:**
- Treine para o harness que você vai usar (ex: se o agente vai usar o shell, treine no shell; se vai usar APIs bespoke, treine nisso). Otimize para um mundo, mova muito mais rápido.
- Invista em reasoning para tarefas longas: o modelo precisa entender quando compactar contexto, quando pedir ajuda.

**Camada 2 — API/Infraestrutura:**
- Suporte sessões longas (Codex roda overnight, 24h+). Isso exige endpoints que entendem compaction e contextos contínuos.
- Design de rate limits e checkpointing pensado para tasks assíncronas, não só request-response.

**Camada 3 — Harness:**
- Opinião forte sobre como o modelo interage com o mundo (shell, semantic search, ferramentas bespoke). A escolha de harness determina quão rápido você consegue melhorar o modelo.
- Sandbox: segurança e isolamento permitem que o modelo experimente sem medo — essencial para tasks de engenharia.
- Compaction: quando o contexto está quase cheio, o harness prepara o payload para o modelo continuar em novo contexto sem perder estado relevante.

## Insights por autor
### [[Alexander Embiricos]]
- "O stack que pensamos é: modelo + API + harness. E todos os três têm um papel enorme."
- Compaction como exemplo: "Para enviar essa feature que faz o Codex funcionar continuamente por 24h, tivemos de trabalhar nas três camadas ao mesmo tempo — o modelo precisa entender o conceito, a API precisa ter o endpoint, e o harness precisa preparar o payload."
- "Todos os produtos de coding têm harnesses muito diferentes com opiniões muito diferentes sobre como o modelo deve funcionar. Se você quer treinar um modelo bom para todos eles, é muito mais lento. Otimize para um mundo."
- Codex usa o shell diretamente — opinião forte. Isso permite velocidade de melhoria que harnesses genéricos não têm.

> 🎧 [Why humans are AI's biggest bottleneck (and what's coming in 2026) (1:16:34)](https://www.youtube.com/watch?v=xZifSLGOrrw)

## Conceitos relacionados
[[Gargalo humano na era dos agentes]] · [[Dois pilares do produto de IA]] · [[Framework CC/CD]]
