---
tipo: tecnica
nivel: 3
fluxo: Experimentação & Dados
autores: [Marily Nika]
---
# Prototipagem antes de Modelo — IA Fora do MVP

**Fluxo:** [[05 - Experimentação & Dados]] · **Tema:** [[Experimentação — Aprender com pouco e qualitativo]] · **Camada:** L3
**Tipo:** Técnica · **Fontes:** [[Marily Nika]]

## Ideia central
Nunca invista em treinar um modelo de ML para validar um MVP. O custo de tempo e de talento especializado (data scientists, máquinas de treinamento, semanas de espera) é incompatível com a etapa de validação. A alternativa correta é prototipar o comportamento do modelo com um wireframe/Figma ou um Wizard of Oz — e reservar o investimento em IA para quando você já tiver dados reais ou dados adjacentes de produtos existentes.

## Como aplicar
1. **MVP → prototype first**: Se você quer validar se usuários adotariam uma feature com IA, construa um protótipo Figma que *simula* o output do modelo. Não treine nada.
2. **Critério para investir em IA**: você tem dados próprios (de produto existente ou adjacente) que podem ser usados para treinar? Se não, você ainda está em estágio de validação.
3. **Pré-requisitos antes de engajar data scientist**: (a) problema definido, (b) audiência e pain point claros, (c) hipótese de que dados existentes podem resolver o problema.
4. **Regra da qualidade de lançamento**: o AI PM define o threshold de acurácia aceitável para lançar ("se o modelo classifica certo 70% das vezes, isso é bom o suficiente para o usuário?"). Essa decisão é editorial, não técnica.

## Insights por autor
### [[Marily Nika]]
- "Don't do it for your MVP. It makes zero sense. Do not waste time of data scientists that can train models with using powerful machines that are going to take weeks to train."
- Alternativa: "Create a little Figma prototype and just show it to some users, just fake what the AI is going to be doing."
- Quando usar IA de verdade: "You should use AI where you think you already have some data or data from an adjacent product that you feel you can leverage."
- Decisão de threshold: "When is the quality of your product good enough to launch? It's totally your responsibility as a PM to decide — is 70% accurate, 80% accurate, where is the bar?" Isso não existe no PM tradicional.

> 🎧 [AI and product management | Marily Nika (14:42)](https://www.youtube.com/watch?v=qNPPoj1qUG0)

## Conceitos relacionados
[[Experimentos Wizard of Oz]] · [[AI PM — Gerenciar o Problema, não o Produto]] · [[CC-CD — Calibração Contínua, Desenvolvimento Contínuo]]
