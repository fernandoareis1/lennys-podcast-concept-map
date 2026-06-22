---
tipo: insight
nivel: 3
fluxo: Experimentação & Dados
autores: [Alexander Embiricos]
---
# Gargalo do agente — velocidade de validação humana
**Fluxo:** [[05 - Experimentação & Dados]] · **Tema:** [[Experimentação — AB testing & cultura]] · **Camada:** L3
**Tipo:** Insight · **Fontes:** [[Alexander Embiricos]]

## Ideia central
O fator limitante subestimado para agentes de IA não é a inteligência do modelo — é a **velocidade com que humanos conseguem revisar e validar o trabalho do agente**. Mesmo com um agente muito inteligente, se a pessoa precisa ler cada PR ou analisar cada saída, o gargalo é a velocidade de digitação/leitura/validação humana.

O unlock real: agentes que conseguem **validar o próprio trabalho** — rodar testes, ver o resultado, iterar sem precisar de checkpoint humano em cada passo. Quando esse loop fecha, a produtividade passa a escalar de forma exponencial.

Implicação para design de produto de IA: a pergunta de design mais importante não é "como deixo o agente mais inteligente?" mas "como reduzo o custo humano de validar o que o agente fez?".

## Como aplicar
1. **Identifique o gargalo de validação no seu fluxo**: onde na sua pipeline de IA a revisão humana é o bottleneck? Que tipo de validação é necessária?
2. **Feche o loop de auto-validação**: configure agentes para rodar os próprios testes, ver os próprios resultados e iterar antes de pedir revisão humana.
3. **Separe validação técnica de validação de qualidade**: um agente pode verificar "o código rodou?" automaticamente; "o design está certo?" pode precisar de humano — mas saiba diferenciar.
4. **Invista em infra de validação**: antes de contratar mais gente para revisar, pergunte se é possível construir infra que permite ao agente validar seu próprio trabalho.
5. **Redefina o papel humano**: em vez de revisor de cada saída, o humano passa a ser configurador dos critérios de validação — uma meta-função de curador, não de executor.

## Insights por autor
### [[Alexander Embiricos]]
- "The current underappreciated limiting factor is literally human typing speed or human multitasking speed."
- "We need to unblock those productivity loops from humans having to prompt and humans having to manually validate all the work."
- "If we can rebuild systems to let the agent be default useful, we'll start unlocking hockey sticks."
- Exemplo interno: engenheiro configurou Codex para verificar o próprio trabalho num loop — pedindo ao Codex: "Por que você não consegue verificar seu trabalho? Corrija" — de forma iterativa.
- "Codex can be on call for its own training" — o próximo passo: Codex monitorando gráficos de training run e tomando ação quando algo vai mal.
> 🎧 [Inside OpenAI Codex: building the future of software engineering (1:16:34)](https://www.youtube.com/watch?v=xZifSLGOrrw)

## Conceitos relacionados
[[Humans in the Loop (algoritmos)]] · [[Non-determinismo em produtos de IA]] · [[CCCD — Calibração e Desenvolvimento Contínuos]] · [[Experimentação — AB testing & cultura]]
