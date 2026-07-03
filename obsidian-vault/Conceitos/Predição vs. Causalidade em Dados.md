---
tipo: framework
nivel: 3
fluxo: Experimentação & Dados
autores: [Ramesh Johari]
---
# Predição vs. Causalidade em Dados
**Fluxo:** [[05 - Experimentação & Dados]] · **Tema:** [[Experimentação — AB testing & cultura]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Ramesh Johari]]

## Ideia central
O erro mais comum em data science: confundir **predizer** com **decidir**. Modelos de ML encontram correlações — excelentes para predições. Mas boas decisões precisam de **causalidade**: o que muda no resultado *porque eu tomei essa decisão*?

**Exemplo canônico:**
Você tem um excelente modelo de LTV de clientes. Quem vai receber as promoções de marketing?
- Resposta intuitiva: "Os clientes com maior LTV predito"
- Resposta correta: "Os clientes cujo LTV vai *incrementar mais* por causa da promoção" — o diferencial, não o absoluto

Esses conjuntos são frequentemente opostos: clientes de alto LTV já comprariam sem a promoção (você desperdiça o custo); clientes de médio LTV que ainda não foram ativados podem aumentar significativamente o gasto por causa da promoção.

**A distinção técnica:**
- **Machine Learning (correlação):** "Quem é mais provável de fazer X?" → encontra padrões nos dados históricos
- **Causal inference (causalidade):** "Como minha ação muda a probabilidade de X?" → estima a diferença contrafactual

**Aplicação em marketplaces — ranking:**
Comparar dois algoritmos de ranking não é avaliar qual prediz melhor os cliques históricos. É avaliar qual **gera mais bookings reais** quando implantado. O teste correto é um A/B test de algoritmos, não uma comparação off-line de acurácia preditiva.

## Como aplicar
1. **Sempre reformule decisões como perguntas causais:** em vez de "qual cliente tem maior LTV?", pergunte "qual cliente vai comprar mais *por causa* desta ação?"
2. **Desconfie de rankings baseados em predição pura:** o ranker que maximiza predição de clique ≠ o ranker que maximiza receita real; valide com A/B test
3. **Use causal inference para alocar budget:** dados de experimentos bem desenhados + modelos de uplifts revelam quem realmente responde à intervenção
4. **Treine a equipe a pensar em diferenciais, não em absolutos:** "Quantos a mais vão converter *porque* fizemos isso?" vs. "Quem tem maior taxa de conversão?"
5. **Para decisões sem experimento possível:** utilize quasi-experimental methods (diff-in-diff, instrumental variables) para estimar efeitos causais a partir de dados observacionais

## Insights por autor
### [[Ramesh Johari]]
- "Predicting is about picking up patterns. Making decisions is about thinking about these differences — the differential, not the absolute."
- "Correlation is not causation. Prediction is inherently about correlation. But when we ask people to make decisions, we're asking them to think about causation."
- Exemplo do CMO: "Definitely the highest LTV people" get the promotions — mas isso ignora quem realmente vai incrementar LTV por causa da promoção
- "The first and most important thing: get data scientists to be thinking their goal is to help the business make decisions — not just predictions."
- Usou exemplo de oDesk: prever quem será contratado ≠ rankar candidatos de forma que maximize a qualidade dos matches futuros
> 🎧 [Marketplace lessons from Uber, Airbnb, Bumble, and more | Ramesh Johari (1:23:36)](https://www.youtube.com/watch?v=BVzTfsUMaK8)

## Conceitos relacionados
[[Experimentação como Disciplina Científica]] · [[Cultura de experimentação a 1.000/ano]] · [[A-B Testing — Evidências (Ronny Kohavi)]] · [[Falha Conclusiva — Design de Experimento Definitivo]] · [[Experimentação Como Mitigação de Risco — Quando Não Testar]]
