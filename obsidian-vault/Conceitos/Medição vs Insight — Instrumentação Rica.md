---
tipo: framework
nivel: 3
fluxo: Experimentação & Dados
autores: [Crystal Widjaja]
---
# Medição vs Insight — Instrumentação Rica
**Fluxo:** [[05 - Experimentação & Dados]] · **Tema:** [[Experimentação — Aprender com pouco e qualitativo]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Crystal Widjaja]]

## Ideia central
A maioria dos times de dados coleta medições, não insights. A diferença é fundamental:

**Medição (observação sem contexto):**
> "Usuários power users fazem 4x mais reservas."

Isso é um fato observável do banco de dados transacional. Não te diz o que fazer.

**Insight (observação + por quê + ação):**
> "Usuários power users de GoFood são 2x mais propensos a usar desconto de frete grátis em pedidos de alto GMV do que usuários novos."

Isso te diz: segmente a promoção de frete para poder users em pedidos grandes — não gaste com novos usuários porque eles não convertem melhor.

**A regra do jornalismo:**
"Real news is information that changes what you do in the real world. If you don't change what you're doing, what you are doing is just getting entertainment." — Crystal usa Twitter de notícias vs Twitter de entretenimento como analogia: dado que não muda seu comportamento é entretenimento, não inteligência de produto.

**Como a instrumentação ruim se parece:**
- Centenas de eventos no banco de dados, cada um com uma ou nenhuma propriedade
- Exemplo ruim: evento `map_loaded`, propriedade: nenhuma
- Exemplo bom: evento `map_loaded`, propriedades: número de motoristas visíveis, cidade, lat/long, surge pricing ativo, tarifa mínima atual, código de voucher presente

Com a instrumentação ruim, você vê que usuários com dois motoristas na tela convertem menos, mas não sabe onde (em quais cidades, em quais horários) esse problema acontece. Sem essa segmentação, você não pode agir.

**O processo para chegar ao insight:**
1. Observe o fato (medição)
2. Forme hipótese do por quê (contexto)
3. Verifique se a instrumentação tem as propriedades necessárias para testar a hipótese
4. Segmente quem está fazendo o quê, em qual contexto
5. Teste causalmente — encontre correlação primeiro, depois experimento

**Caso GoPay:**
Crystal viu que usuários do GoFood convertiam menos com vouchers, mas a medição não dizia por quê. Com instrumentação rica (tipo de usuário × valor do pedido × tipo de desconto), surgiu o insight: poder users respondem a frete grátis em pedidos altos; novos usuários não. Isso mudou toda a estratégia de marketing de vouchers.

## Como aplicar
1. **Audite seus eventos de analytics:** para cada evento, quantas propriedades você tem? Se menos de 3, você não consegue segmentar o contexto
2. **Para cada evento, pergunte:** "Se eu visse uma anomalia nesse evento, quais seriam as 5 perguntas que eu faria para entender o por quê?" Essas 5 respostas são as propriedades que você precisa rastrear
3. **Diferencie seu dashboard:** separe métricas de saúde (medições) de queries de investigação (insights). Não trate o mesmo como os dois
4. **Crie rituais de "why":** proíba que perguntas de análise terminem numa observação. Toda sessão de dados termina em: "E daí? O que vamos fazer diferente?"
5. **Teste hipóteses antes de construir:** se você não tem dados para criar hipótese, você não tem dados para priorizar a feature

## Insights por autor
### [[Crystal Widjaja]]
- "Measurements do not equate to insights. A measurement is an observation — a data point. It doesn't have context, it doesn't give you information that lets you act."
- "Real news is information that changes what you do in the real world. If you don't change what you're doing, what you are doing is just entertainment."
- "The symptom of a bad data tracking approach: a ton of rows with a ton of events, but every event has one property or no property."
- "You're missing so much context of the user's experience that you're unable to make assumptions about why the user didn't convert."

## Conceitos relacionados
[[Física do Crescimento — Restrições e Alavancas]] · [[Assumption Testing]] · [[Decidir com poucos dados é melhor que com zero]] · [[Retenção com Contexto — Benchmark 60%]]
