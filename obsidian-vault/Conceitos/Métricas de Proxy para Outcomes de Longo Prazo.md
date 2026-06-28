---
tipo: tecnica
nivel: 3
fluxo: Experimentação & Dados
autores: [Jessica Lachs]
---
# Métricas de Proxy para Outcomes de Longo Prazo
**Fluxo:** [[05 - Experimentação & Dados]] · **Tema:** [[Experimentação — AB testing & cultura]] · **Camada:** L3
**Tipo:** Técnica · **Fontes:** [[Jessica Lachs]]

## Ideia central
Retenção é um output desejado, mas é **impossível de mover de forma significativa no curto prazo** — e sem métricas de curto prazo você não consegue experimentar e iterar. A solução é encontrar uma **métrica proxy de curto prazo** que seja empiricamente correlacionada com o outcome de longo prazo. A questão-chave: quais são os inputs que geram retenção? Encontre um input que você consiga medir em dias/semanas, valide experimentalmente que ele prediz o outcome de longo prazo, e goal seu time nele.

## Como aplicar
1. **Não meça o outcome diretamente** — se o outcome demora meses para aparecer (retenção, LTV, churn), você trava a capacidade de experimentar.
2. **Liste os inputs do outcome** — o que causa retenção? Frequência de uso na primeira semana? Conclusão de onboarding? Primeira compra repetida? Número de features ativas?
3. **Valide empiricamente** — rode experimentos ou análises de coorte para confirmar que o input prediz o outcome de longo prazo no seu negócio específico.
4. **Goal o time no proxy** — use a métrica de proxy como meta de equipe. Assim o time pode experimentar e iterar rápido, sem esperar 6 meses para saber se funcionou.
5. **Reveja periodicamente** — as correlações entre proxy e outcome podem mudar. Faça a validação de tempos em tempos (e.g., holdouts de longo prazo).

## Insights por autor
### [[Jessica Lachs]]
- "Retenção é uma coisa terrível para colocar como meta. É quase impossível de mover de forma significativa no curto prazo, e ainda assim você quer experimentar e iterar rapidamente."
- "O que você quer é encontrar uma métrica de curto prazo que você possa medir e que drive um output de longo prazo."
- "Quais são os inputs que geram retenção? Encontre os inputs certos, e então use experimentação para testar se esses inputs de curto prazo estão gerando o output de longo prazo que você busca."
- "Métricas absolutas vs. taxas: fique atento a incentivos perversos criados pela métrica proxy escolhida."
> 🎧 [Building a world-class data org (1:19:56)](https://www.youtube.com/watch?v=D4PDb_C8Dww)

## Conceitos relacionados
[[OEC - Overall Evaluation Criterion]] · [[Métricas de input vs. output]] · [[Holdout de longo prazo]] · [[Métricas Simples vs Compostas — Clareza Bate Perfeição]]
