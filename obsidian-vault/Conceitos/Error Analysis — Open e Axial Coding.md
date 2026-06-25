---
tipo: tecnica
nivel: 3
fluxo: Experimentação & Dados
autores: [Hamel Husain, Shreya Shankar]
---
# Error Analysis — Open e Axial Coding
**Fluxo:** [[05 - Experimentação & Dados]] · **Tema:** [[Experimentação — Aprender com pouco e qualitativo]] · **Camada:** L3
**Tipo:** Técnica · **Fontes:** [[Hamel Husain]] · [[Shreya Shankar]]

## Ideia central
Técnica adaptada das ciências sociais (análise qualitativa) para mapear falhas em produtos de IA. O processo tem duas fases: **open coding** (anotar livremente o primeiro problema visível em cada trace) e **axial coding** (agrupar essas notas em categorias de falha acionáveis). Inspirada em Andrew Ng e em décadas de análise de sistemas estocásticos em ML — não foi inventada; foi adaptada para o contexto de LLMs.

## Como aplicar
1. **Amostre traces reais** do seu produto (logs de interação usuário-IA).
2. **Open coding:** para cada trace, escreva uma nota curta e descritiva sobre o primeiro problema que você identifica. Seja específico ("não confirmou transferência de chamada com o usuário"), não genérico ("janky"). Pare ao achar o primeiro erro — não liste todos.
3. Continue até atingir **saturação teórica**: o momento em que novas traces não revelam novos tipos de problema. Para a maioria dos produtos, ~50–100 traces é suficiente.
4. **Axial coding:** use um LLM (ChatGPT, Claude, Gemini via planilha) para agrupar os open codes em categorias. Revise e refine as categorias para que sejam acionáveis.
5. **Conte** as categorias (pivot table). A frequência orienta prioridade — mas um erro gravíssimo pode ir para o topo mesmo com baixa contagem.
6. Decida: este erro exige **eval code-based**, **LLM como juiz**, ou apenas uma correção direta no prompt/sistema?

## Insights por autor
### [[Hamel Husain]] e [[Shreya Shankar]]
- "Todo mundo que faz isso fica viciado imediatamente. Você aprende muito sobre sua aplicação."
- Nomear um **benevolent dictator** — uma pessoa com expertise de domínio que decide o que é "bom" — evita que o processo fique paralisado em comitê.
- Axial codes devem ser acionáveis: "Limitação de capacidade" é genérico demais; "não transferiu para humano em solicitação explícita" é acionável.
- "Contagem básica é a técnica analítica mais poderosa em ciência de dados porque é simples e é subestimada."
> 🎧 [Why AI evals are the hottest new skill for product builders (1:46:33)](https://www.youtube.com/watch?v=BsWxPI9UM4c)

## Conceitos relacionados
[[Evals para Produtos de IA]] · [[LLM como Juiz]] · [[Experimentação com amostras pequenas]] · [[Decidir com poucos dados é melhor que com zero]]
