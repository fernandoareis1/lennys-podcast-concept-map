---
tipo: insight
nivel: 3
fluxo: Estratégia & Visão
autores: [Alexander Embiricos]
---
# Código como Linguagem Universal dos Agentes
**Fluxo:** [[02 - Estratégia & Visão]] · **Tema:** [[Estratégia — Estratégia de produto]] · **Camada:** L3
**Tipo:** Insight · **Fontes:** [[Alexander Embiricos]]

## Ideia central
Para que agentes de IA sejam realmente úteis, eles precisam **fazer coisas** no mundo — não apenas conversar. Fazer coisas no mundo exige usar computadores. E a maneira mais eficaz de modelos de linguagem usarem computadores é escrever código. Portanto: **qualquer agente é, no fundo, um agente de código.** Mesmo que o usuário final seja não-técnico e nunca veja uma linha de código, o agente usará código para interagir com APIs, automatizar tarefas, analisar dados e orquestrar sistemas. Isso tem implicações estratégicas profundas: a empresa que construir o melhor agente de código terá a base para o melhor agente geral. Código é composável, interoperável e pode ser compartilhado entre instâncias do agente — se um agente aprendeu a fazer uma tarefa, o script pode ser reusado por outros.

## Como aplicar
1. **Avalie seu agente como um coding agent**: mesmo que seu produto não seja voltado para desenvolvedores, pergunte: "Como meu agente escreve código para executar ações?" Se ele não escreve código, ele provavelmente está usando métodos mais frágeis (point-and-click, accessibility APIs, screenshots).
2. **Use shell/terminal como interface padrão do agente**: é mais confiável que simular cliques ou depender de APIs de acessibilidade. Cria um sandbox controlado e permite que o agente valide suas ações.
3. **Invista em composabilidade**: scripts e competências que o agente aprende devem ser reutilizáveis e compartilháveis entre usuários do mesmo time.
4. **Para PMs e não-engenheiros**: o código é o "WiFi" da era dos agentes — o usuário não precisa saber que está usando, mas é o que possibilita tudo. Entender esse ponto muda como você pensa na arquitetura do produto.
5. **Pense em camadas de abstração crescentes**: prompt → patch (hoje), spec → código (futuro próximo), ideia → produto (horizonte de 1+ ano). Cada camada remove uma etapa manual.

## Insights por autor
### [[Alexander Embiricos]]
- "A melhor forma para modelos usarem computadores é simplesmente escrever código. E então chegamos a essa ideia de que se você quer construir qualquer agente, talvez você devesse construir um agente de código."
- Para o usuário final não-técnico: "Eles não vão saber que estão usando um coding agent, da mesma forma que ninguém pensa se está usando a internet ou não — eles só pensam 'o WiFi está ligado?'"
- Código é composável: "Se um agente aprende como fazer uma tarefa, esse script pode ser reutilizado por outros agentes ou outros membros do time. Você não precisa refazer esse trabalho."
- Implicação estratégica: construir modelo + API + harness em paralelo (time de produto e pesquisa integrado) permite iterar muito mais rápido do que otimizar apenas o modelo.
- Resultados concretos: Codex cresceu 20x desde agosto de 2025; App Sora para Android construído em 18 dias por 2-3 engenheiros, número 1 na App Store.

> 🎧 [Building Codex: OpenAI's coding agent (1:16:34)](https://www.youtube.com/watch?v=xZifSLGOrrw)

## Conceitos relacionados
[[Proatividade como Destino dos Agentes]] · [[Non-determinismo em Produtos de IA]] · [[Trade-off Agência-Controle]] · [[Estratégia — Estratégia de produto]]
