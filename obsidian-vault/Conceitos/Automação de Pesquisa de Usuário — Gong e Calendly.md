---
tipo: framework
nivel: 3
fluxo: Discovery & Pesquisa
autores: [Kevin Yien]
---
# Automação de Pesquisa de Usuário — Gong e Calendly

**Fluxo:** [[01 - Discovery & Pesquisa]] · **Tema:** [[Discovery — Descoberta contínua & validação]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Kevin Yien]]

## Ideia central
A desculpa mais comum para não falar com usuários é falta de tempo. A solução é **automatizar o agendamento** de entrevistas usando a infraestrutura de vendas que já existe: Gong + Slack + Zapier + Calendly. O time de vendas é um time de pesquisa que você ainda não está usando.

**A premissa fundacional:**
PMs não devem se contentar com vidro embaçado — relatórios filtrados por UXR, CS, vendas ou pesquisa de mercado. Esses são dados processados. PMs precisam de exposição direta à matéria-prima: o cliente em tempo real. A diferença entre ler sobre um cozinheiro e ficar ao lado de um cozinheiro.

**O sistema de automação (B2B):**
1. **Gong alerts**: Configure alertas no Gong para termos relacionados ao que você está investigando (ex.: "ponto de venda", "integração", nome de concorrente)
2. **Slack integration**: Gong posta automaticamente no Slack o trecho da transcrição onde o termo apareceu + e-mail do cliente
3. **Zapier trigger**: Cada novo post desse canal Slack aciona um Zapier
4. **customer.io email**: Zapier usa o e-mail capturado para enviar um e-mail automático de convite de pesquisa com link do Calendly específico para entrevistas de usuário
5. **Entrevista automática**: Entrevistas aparecem no calendário do PM sem nenhuma busca manual

**Para B2B sem Gong:**
- userinterviews.com: plataforma de recrutamento de participantes de pesquisa focada em B2B. Configure critérios de ICP, eles fazem o sourcing, você aprova.
- Integração com canais de comunidade (Reddit, fóruns de suporte, Slack externo): script de alerta personalizado

**O erro de maturidade:**
PMs novos falam muito com usuários. PMs experientes param de falar. "Eu já os conheço de dentro para fora. Posso escrever um PRD de olhos fechados." Isso é uma mentira tentadora — o mundo deles está mudando, a vida deles está mudando, e você precisa de exposição constante às micro-mudanças.

## Como aplicar
1. Identifique 3-5 termos que definem o que você quer aprender agora. Configure alertas Gong para esses termos.
2. Conecte Gong ao canal Slack dedicado a pesquisa de usuário.
3. Configure Zapier: Slack post → extrai e-mail do cliente → envia e-mail via customer.io → convite de Calendly.
4. Crie um Calendly específico para user research (30 min, sem conflito com outras reuniões).
5. Para recrutamento externo de B2B: crie conta em userinterviews.com com critérios do ICP e deixe o sourcing no piloto automático.
6. Nunca deixe de falar com usuários citando "já fiz 100 entrevistas antes." O fluxo deve ser constante.

## Insights por autor
### [[Kevin Yien]]
- "O time de vendas é um time de pesquisa — e se você não vê assim, está perdendo metade do valor."
- O sistema completo foi desenvolvido por Beth Hills, PM contratada na Mutiny: "Ela é a rainha de automatizar pesquisa de usuário."
- "A desculpa de que não tenho tempo para buscar usuários não existe quando o sistema traz eles automaticamente."
- "Há uma diferença absurda entre ler um relatório sobre um cozinheiro e ficar ao lado de um cozinheiro."
- Quando um PM não pode falar com clientes por restrição do CS: "Há algo estruturalmente errado e isso precisa ser resolvido primeiro."

> 🎧 [Unorthodox PM tips: Automating user insights, unselling candidates, decision logs, more | Kevin Yien](https://www.youtube.com/watch?v=xOTO98MXG9o) · 2024-08-18

## Conceitos relacionados
[[Discovery — Descoberta contínua & validação]] · [[Discovery — Entrevistar usuários]] · [[Modelo Mental dos Stakeholders]] · [[SEO por JTBD de ponta a ponta]] · [[Crescimento via comunidade de supply]]
