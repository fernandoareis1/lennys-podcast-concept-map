---
tipo: tática
nivel: 3
fluxo: Discovery & Pesquisa
autores: [Vijay Iyengar]
---
# Feed Bruto de Cliente — Cultura Sem Gatekeepers

**Fluxo:** [[01 - Discovery & Pesquisa]] · **Tema:** [[Discovery — Descoberta contínua & validação]] · **Camada:** L3
**Tipo:** Tática · **Fontes:** [[Vijay Iyengar]]

## Ideia central
Crie um pipeline que leva feedback de clientes (de CS, sales, NPS, Twitter) direto para um canal Slack **sem curadoria, sem pré-agregação, sem gatekeeper**. Qualquer engenheiro ou designer pode ler o feed raw, identificar algo que ressoa, e agir diretamente.

O efeito: engineers e designers pensam como PM. O PM deixa de ser o único ponto de contato com a realidade do cliente.

## Como funciona no Mixpanel
O engenheiro Aaron construiu a automação em 2018: gaps reportados por CS e sales → Slack → feed aberto para todo o time. Ao longo do tempo evoluiu para incluir:
- Posts no Twitter sobre o produto
- Feedback de pesquisas de NPS
- Notas de win/loss de deals competitivos

Tudo cai no mesmo canal e numa base em Notion para sorting, tagging e agregação.

O ritual emergente: engenheiros reagem a mensagens com um emoji de email (📧) sinalizando "vou falar com esse cliente." Eles mandam um email para o usuário, fazem os 5 porquês, e melhoram a feature — sem precisar de aprovação de PM.

## Por que "raw" importa
Qualquer camada entre o feedback e o time filtra a realidade. Um PM que sumariza o que clientes disseram já está fazendo interpretação. Um processo de priorização que seleciona quais feedbacks chegam ao time já está fazendo curadoria.

O feed bruto expõe o time à **mesma realidade desconfortável que o cliente está vivendo** — não a versão já processada. Vijay leu esse canal todos os dias por 4-5 anos como engenheiro.

## O que escala e o que não escala
A abordagem escala surpreendentemente bem. No nível do Mixpanel, o volume de feedback não é tão alto que um engenheiro não consiga ler tudo em 20 minutos por dia. O ponto de risco é quando o volume cresce além disso — que é quando a camada de Notion com tagging e sorting vira necessária.

O que não deve mudar com a escala: o princípio de que qualquer pessoa no time de produto pode acessar feedback direto sem intermediários.

## Insights por autor
### [[Vijay Iyengar]]
- "We piped all the customer gaps from our customer success and sales teams into Slack — a feed where all engineers and designers could consume that raw feed of direct customer feedback with no gatekeeper, no process, no pre-aggregation."
- "Engineers would go into that channel and react with an email emoji, meaning 'I'm going to email this customer and find out more.' They'd ask the five why's and then improve the product on their own."
- "That culture is just so important. It empowers all engineers and designers to think like a PM a little bit, which takes a little load off the PM to be the gatekeeper of all that information."
- "The key artifact is that it's all open. There's no gatekeeper behind that process."

> 🎧 [An inside look at Mixpanel's product journey | Vijay Iyengar](https://www.youtube.com/watch?v=t-2oXtZrlEc) · 2023-01-26

## Conceitos relacionados
[[Automação de Pesquisa de Usuário — Gong e Calendly]] · [[Função de Insights Integrada]] · [[Fechar o Loop — Comunidade como Co-Criador]]
