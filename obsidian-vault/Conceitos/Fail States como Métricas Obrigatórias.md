---
tipo: tecnica
nivel: 3
fluxo: Experimentação & Dados
autores: [Jessica Lachs]
---
# Fail States como Métricas Obrigatórias
**Fluxo:** [[05 - Experimentação & Dados]] · **Tema:** [[Experimentação — AB testing & cultura]] · **Camada:** L3
**Tipo:** Técnica · **Fontes:** [[Jessica Lachs]]

## Ideia central
Métricas de médias escondem os piores cenários. O "Never Delivered" (pedido que nunca chegou) na DoorDash aparecia em frações de porcento — mas cada instância gerava churn direto do consumidor **mais** o custo de reembolso mais novo pedido mais novo Dasher. Se você apenas olha métricas de qualidade médias, essas experiências catastróficas somem. A regra: **todo produto deve ter uma métrica explícita de fail state**, com dono e meta de eliminação.

## Como aplicar
1. **Liste os estados de falha do seu produto** — o que são as piores experiências que um usuário pode ter? Login que não funciona, transação que duplica, entrega que nunca chega, compra sem confirmação.
2. **Quantifique o impacto real** — fail states raramente aparecem nas médias, mas têm impacto desproporcional: churn das ordens subsequentes (invisível nos dados porque o usuário sumiu), custo de reparação, impacto na marca.
3. **Crie uma métrica dedicada para cada fail state** — "Never Delivered", "Login failure rate", "Order never confirmed". Mantenha simples; nomeie com clareza (a DoorDash é famosa por nomes ultradiretos).
4. **Designe um time com meta de eradicação** — not "reduzir", mas "eradicar". A meta ambiciosa força investigação profunda da causa raiz: erro humano? fraude? bug de infraestrutura?
5. **Cuidado com dados ausentes** — se o usuário não consegue logar, ele não aparece nos seus dados de conversão. Qual dado você pode não estar vendo porque o usuário travou antes?

## Insights por autor
### [[Jessica Lachs]]
- "Só porque algo não acontece frequentemente não significa que não é importante. O Never Delivered leva diretamente ao churn — e você está perdendo todos os pedidos futuros daquele consumidor, que são invisíveis nos dados."
- "Se você está só olhando o efeito médio ou os valores médios de delivery times, essas experiências de 'never delivered' nunca vão aparecer porque são tão raras. Mas são terríveis."
- "Com erros de login, as pessoas não conseguem nem entrar. Elas não estão no denominador — então você está perdendo oportunidades que sequer estão no dataset."
- "Nosso time tem como meta erradicar o Never Delivered. Às vezes é erro humano, às vezes é fraude. Você nunca vai eliminar completamente, mas pode ter impacto significativo."
> 🎧 [Building a world-class data org (1:19:56)](https://www.youtube.com/watch?v=D4PDb_C8Dww)

## Conceitos relacionados
[[Métricas Simples vs Compostas — Clareza Bate Perfeição]] · [[Métricas de Proxy para Outcomes de Longo Prazo]] · [[A maioria das ideias falha no teste]] · [[Retenção — Retenção & churn]]
