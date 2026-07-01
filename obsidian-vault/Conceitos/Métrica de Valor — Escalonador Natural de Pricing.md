---
tipo: framework
nivel: 3
fluxo: Monetização & Pricing
autores: [Naomi Ionita]
---
# Métrica de Valor — Escalonador Natural de Pricing
**Fluxo:** [[08 - Monetização & Pricing]] · **Tema:** [[Monetização — Modelos & poder de pricing]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Naomi Ionita]]

## Ideia central
Quando o preço espelha a unidade de valor que o usuário recebe (a "value metric"), cria-se um **escalonador natural**: quanto mais o cliente usa o produto, mais paga — e isso se alinha perfeitamente com o valor entregue. Essa é a lógica por trás dos modelos usage-based (número de mensagens, chamadas de API, terabytes armazenados, palavras escritas). O problema do modelo seat-based histórico é que o preço não cresce com o uso — um usuário muito ativo paga o mesmo que um casual.

A maioria das empresas SaaS adota um **modelo híbrido**: planos de assinatura (bom/melhor/ótimo) com uma quota da value metric embutida em cada tier. Ao atingir o limite, o usuário é naturalmente empurrado para o próximo plano — ou paga por overage.

## Como aplicar
1. **Identifique sua value metric**: qual é a unidade que o cliente derivou valor? (Ex: Slack → mensagens, Dropbox → GB, Invoice2go → notas fiscais emitidas)
2. **Evite ser apenas seat-based**: assinaturas por assento não escalam com o valor gerado e criam conflito com o cliente conforme ele cresce.
3. **Evite ser apenas usage-based**: CFOs precisam de previsibilidade; custo variável puro dificulta aprovação orçamentária.
4. **Construa o híbrido**: planos (bom/melhor/ótimo) com quotas da value metric; overage para quem ultrapassar; isso oferece previsibilidade + escala.
5. **Entenda a demanda relativa por feature**: use surveys de ranking (must-have / nice-to-have / não necessário) e a "questão dos 100 pontos" — distribua 100 pontos entre as features para entender priorização real.

## Insights por autor
### [[Naomi Ionita]]
- "Matching price to value creates alignment with your user — it creates this natural escalator because as people use it more, you get paid more over time."
- "Whether it's number of API calls or messages sent or terabytes of storage used or words written, this usage-based approach really matches price to value over the lifetime of a customer."
- "A small sliver — roughly 5% — have just a pure usage-based model. The vast majority have a hybrid approach."
- Risco do usage-based puro: "I remember using Mixpanel and Segment and even Jira — I was blown away by how much more we were paying." Buyers querem previsibilidade.
> 🎧 [How to price your product (53:17)](https://www.youtube.com/watch?v=xvQadImf568)

## Conceitos relacionados
[[Preço como Roadmap — Não Defina e Esqueça]] · [[Day One vs Day 100 — Empacotamento de Freemium]] · [[Willingness to Pay (regra 20-80)]] · [[Pricing baseado em outcome]]
