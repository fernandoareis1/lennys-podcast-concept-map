---
tipo: framework
nivel: 3
fluxo: Liderança & Times
autores: [Scott Wu]
---
# Tarefas, não Problemas — Workflow com Agentes de IA

**Fluxo:** [[09 - Liderança & Times]] · **Tema:** [[Liderança — Colaboração & comunicação]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Scott Wu]]

## Ideia central
Para usar agentes de IA de forma eficaz, a unidade de trabalho que se delega deve ser uma **tarefa bem-definida**, não um **problema aberto**. Delegar "re-arquitete o código base" resulta em trabalho ruim; delegar "conserte este bug no componente X" resulta em PR pronto para merge. O mesmo princípio que diferencia delegação eficaz para pessoas junior se aplica a agentes: especificidade e escopo controlado são pré-requisitos para resultado autônomo.

O segundo princípio complementar: o melhor fluxo de trabalho com múltiplos agentes é **assíncrono**. Você dispara várias tarefas em paralelo, checa apenas os pontos de decisão críticos e revisa o output no final — em vez de acompanhar cada passo.

## Como aplicar
1. **Decomponha antes de delegar**: quebre um problema grande em tarefas discretas e sequenciais antes de entregar ao agente. O humano faz a arquitetura; o agente faz a implementação.
2. **Dê contexto, não ambiguidade**: inclua o repositório certo, o arquivo certo, o comportamento esperado. Quanto mais específica a tarefa, maior a taxa de sucesso autônomo.
3. **Rodar em paralelo**: enquanto um agente resolve bug A, outro cobre feature B e outro escreve testes de C. 5 agentes por engenheiro é operação normal na Cognition.
4. **Intervenha só nos 10–20% críticos**: não acompanhe passo a passo. Revise o plano inicial, forneça feedback de ajuste se necessário, valide o output final. Salve o foco humano para decisões de arquitetura.
5. **Ensine o agente ao longo do tempo**: agentes com memória de sessão acumulam contexto sobre o codebase e as preferências do time — invista em onboarding e ajuste progressivo.

## Insights por autor
### [[Scott Wu]]
- "You want to be giving Devin tasks, not problems."
- Tarefas certas para agente: bug fix bem descrito, feature request de front-end, adição de testes/documentação. Problema errado: "refatore todo o sistema."
- Cognition usa times de 5 Devins simultâneos por engenheiro, de forma assíncrona; Devin merges centenas de PRs/mês com apenas 15 engenheiros humanos.
- Princípio de onboarding: antes de grandes tarefas, dê ao agente 2–3 tarefas pequenas para ele aprender o codebase e as convenções do time.
- "A lot of it is really learning to work with Devin to be able to just do more in parallel and build more."
> 🎧 [Inside Devin: The AI engineer that's set to write 50% of its company's code this year | Scott Wu](https://www.youtube.com/watch?v=gI0ZNhA0rvE) · 1:32:32

## Conceitos relacionados
[[Gosto Sobre Precisão — O Novo Skill do Engenheiro de IA]] · [[Gargalos Emergentes na Era de Código com IA]] · [[Vibe Coding — Delegar a Execução ao Modelo]] · [[De Saber a Fazer — A Transição dos Agentes de IA]]
