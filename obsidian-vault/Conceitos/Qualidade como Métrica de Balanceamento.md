---
tipo: framework
nivel: 3
fluxo: Experimentação & Dados
autores: [Nickey Skarstad]
---
# Qualidade como Métrica de Balanceamento

**Fluxo:** [[05 - Experimentação & Dados]] · **Tema:** [[Experimentação — AB testing & cultura]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Nickey Skarstad]]

## Ideia central
Em produtos de marketplace e serviços, crescimento sem qualidade é crescimento que se autodestrói. A solução é usar uma **métrica de qualidade como north star que "balanceia" as métricas de crescimento** — você cresce, mas só o crescimento com qualidade vale.

Na Airbnb Experiences, o time não usou bookings ou receita como north star: usou a **taxa de reviews** (proporção de bookings que resultava em review). Um review pressupõe que o usuário apareceu, viveu a experiência e se sentiu motivado a deixar feedback. Se a taxa de reviews estava alta, o produto estava entregando valor real.

Métricas de qualidade servem de guardrail:
- Forçam o time a não sacrificar experiência real por números superficiais
- Alinham produto e operações em torno do mesmo objetivo
- Permitem crescimento sustentável: qualidade → NPS → retenção → crescimento orgânico

**Em outros contextos:**
- E-commerce: % de produtos com avaliações altas / taxa de retorno de compras
- SaaS: NPS segmentado por coorte de uso / % de usuários que chegam ao "momento aha"
- Conteúdo: % de sessões completadas / ratio de sessões de retorno

## Como aplicar
1. **Identifique o sinal de qualidade real** no seu produto — o que indica que o usuário teve a experiência prometida, não só que "usou" o produto.
2. **Promova essa métrica de qualidade ao nível de north star ou KPI de balanceamento** — qualquer crescimento que piora essa métrica deve ser questionado.
3. **Calibre operações em torno dela:** treine hosts, otimize suporte, eduque usuários com base no que move essa métrica.
4. **Dogfood regularmente:** a equipe deve vivenciar o produto para identificar quando a qualidade não está boa antes que as métricas caiam.
5. **Comunique o racional ao time:** "estamos otimizando para experiências de 5 estrelas, não só para bookings" tem que ser entendido por engenharia, ops, design e liderança.

## Insights por autor
### [[Nickey Skarstad]]
- "We were obsessed with making sure every person who booked actually had a good experience when they showed up to experiences."
- "We used review rate as our end-all, be-all top line goal... it trickled down — everyone understood that it was important."
- "If you are building early product, think about how you can pick good quality metrics that might actually balance or conflate with growth metrics, and use that as your north star."
- Dogfooding como mecanismo: "We would go back to the teams and be like, 'We were just in San Francisco. We were on an experience last night, and it did not go well. What do we do about it?'"
- Airbnb: "Airbnb does not ship product if it is not good. They are obsessed with the end consumer experience."
> 🎧 [Nickey Skarstad (Airbnb, Etsy, Shopify, Duolingo) on translating vision into goals, second-order decisions (1:00:54)](https://open.spotify.com/episode/6FKUgLvnlpyLOyMbykXm6u)

## Conceitos relacionados
[[OEC - Overall Evaluation Criterion]] · [[Métricas Simples vs Compostas — Clareza Bate Perfeição]] · [[Portas de Mão Única vs Mão Dupla — Decisões Reversíveis]] · [[Metrics Tree — Desdobramento do North Star]]
