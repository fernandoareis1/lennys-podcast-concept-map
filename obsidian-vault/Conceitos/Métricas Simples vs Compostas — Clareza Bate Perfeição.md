---
tipo: tecnica
nivel: 3
fluxo: Experimentação & Dados
autores: [Jessica Lachs]
---
# Métricas Simples vs Compostas — Clareza Bate Perfeição
**Fluxo:** [[05 - Experimentação & Dados]] · **Tema:** [[Experimentação — AB testing & cultura]] · **Camada:** L3
**Tipo:** Técnica · **Fontes:** [[Jessica Lachs]]

## Ideia central
Data scientists amam métricas compostas com coeficientes e pesos ("merchant health score = 0.35"). O problema: ninguém entende o que é 0.35, ninguém tem intuição de o que significa subir 0.1, e times ficam perdidos sobre como mover a agulha. Uma métrica simples — mesmo que imperfeita — é superior a uma composta perfeita que ninguém consegue debater num all-hands. Se as pessoas não conseguem conversar sobre a métrica, ela não vai gerar ação.

## Como aplicar
1. **Teste de "conversa de corredor"** — se você não consegue explicar a métrica em uma frase, ela é complexa demais.
2. **Prefira 3 métricas simples a 1 composta obscura** — ao decompor o merchant health score em foto-coverage, accurácia de horários e completude do menu, o time de DoorDash sabia exatamente o que mover.
3. **Priorize dentro das simples** — com métricas separadas, use análise de impacto para dizer qual mover primeiro. Mova a #1 até esgotar oportunidade, então #2.
4. **Mantenha um time por métrica** — trocar métricas toda quarter é ineficiente. Times ficam bons em mover uma métrica com o tempo; misturar ou rotacionar cedo desperdiça o aprendizado acumulado.
5. **Use linguagem que qualquer pessoa entende** — "cobertura de fotos dos restaurantes" é mais acionável do que "score ponderado de completude de perfil do merchant".

## Insights por autor
### [[Jessica Lachs]]
- "Data scientists adoram essas métricas compostas com coeficiente. E você termina com uma métrica que ninguém entende de fato. '0.35 — isso é bom? É ruim? Não sei o que é.'"
- "Eu sempre encorajo as pessoas: escolha algo simples, mesmo que não seja perfeito e sua composta fosse mais perfeita. Se as pessoas entendem, se têm intuição sobre ela, se conseguem falar sobre ela em toda a empresa, será uma métrica muito melhor."
- "No exemplo do merchant health score, decompor em três métricas separadas — mesmo que perdendo #4, #5 e #6 da lista — foi muito melhor, porque o time sabia o que estava tentando mover."
- "Você quer mover todos? Sim. Mas fazer as coisas que importam primeiro e mais rapidamente é uma vantagem competitiva."
> 🎧 [Building a world-class data org (1:19:56)](https://www.youtube.com/watch?v=D4PDb_C8Dww)

## Conceitos relacionados
[[OEC - Overall Evaluation Criterion]] · [[Métricas de Proxy para Outcomes de Longo Prazo]] · [[Fail States como Métricas Obrigatórias]] · [[A maioria das ideias falha no teste]]
