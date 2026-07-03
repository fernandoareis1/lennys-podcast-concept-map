---
tipo: framework
nivel: 3
fluxo: Discovery & Pesquisa
autores: [Tanguy Crusson]
---
# Lighthouse Users — Construir com Poucos para Escalar para Muitos

**Fluxo:** [[01 - Discovery & Pesquisa]] · **Tema:** [[Discovery — Descoberta contínua & validação]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Tanguy Crusson]]

## Ideia central
O antídoto para "esconder-se atrás da pesquisa" (CSAT, NPS, surveys) é construir literalmente **para pessoas com nome e sobrenome**. O **Lighthouse Users Program** é a estrutura que torna isso sistemático em uma empresa grande: 10 usuários no começo, que são o proxy de todos os clientes futuros. Iterar com eles até saber que o produto funciona. Expandir para 100. Depois 1000. Cada stage tem uma característica diferente de aprendizado.

> "I've seen a lot of teams... hiding behind research and not being close enough to the ground with customers."

## Os três estágios
**10 usuários (alpha)**: Validação de problema e solução. Cada usuário é conhecido pelo nome e contexto. Os encontros são em Zoom — conversas, co-criação, exposição do produto. A saída é qualitativa: clipes de vídeo mostrando o problema e como o produto resolve, não dashboards. O critério de saída é: conseguimos explicar por que esses 10 são proxy de todo o mercado?

**10→100 (alpha continuado)**: Teste de variações e cenários. Diferentes tamanhos de empresa, diferentes setups de segurança, diferentes formas de usar. O produto ainda não é self-service — o time atende ativo no Slack, faz Zooms de suporte. O learning aqui é de edge cases e de como o core funciona em contextos variados.

**100→1000 (beta)**: O objetivo muda: tornar o produto self-service. Os problemas são de onboarding, documentação, UX que exige explicação. A saída é: o produto funciona sem o time segurando a mão?

Só depois de 1000 o produto está pronto para GA e para as métricas adultas (MAU, DAU, NRR).

## Product Engineers via exposição direta
O efeito colateral mais valioso do programa é o que acontece com os engenheiros:

Quando um time trabalha com 10 usuários conhecidos por meses, os engenheiros começam a aparecer no planning com opiniões próprias: "Falamos com a Marta semana passada e ela tem esse problema específico — deveríamos resolver isso antes de X."

Isso é a diferença entre **system engineers** (que constroem o que o PM especifica) e **product engineers** (que entendem profundamente o problema do usuário e contribuem ativamente para a solução). A exposição direta ao cliente é o que cria product engineers — não treinamentos, não frameworks.

> "All of a sudden you're not talking about a product manager, you're talking about a product team with product engineers."

## Safety Funnel — não estrague clientes existentes
Em produtos maduros, uma nova bet não pode fazer experimentos que impactem milhões de usuários. A solução é o **Safety Funnel**: um hard stop explícito sobre quantas pessoas podem ter uma experiência ruim.

Em vez de maximizar exposure para maximizar métricas, o time **limita deliberadamente** o número de usuários no produto cedo. O racional: se alguém tem uma experiência ruim e vai embora, você raramente o recupera. Melhor que apenas 10 pessoas tenham uma experiência imperfeita do que 10.000.

Isso inverte a lógica corporativa padrão (mais usuários = mais sucesso) no zero-a-um: **menos usuários, melhor experiência, mais aprendizado qualitativo**.

## O princípio da mudança climática
Tanguy usa uma analogia para explicar por que 10 usuários conhecidos superam qualquer survey de 10.000 respostas:

> "What makes people want to change and actually gives them a trigger to change? A lot more empathizing with individual people's experience. If I know someone that's impacted by climate change, it's going to make me relate a lot more strongly to the concept of climate change."

Reports sobre mudança climática existem há décadas. O que muda comportamento não é o dado — é a história individual. O mesmo vale para decisões de produto: uma conversa de 30 minutos com um usuário específico muda o time mais do que 30 slides de pesquisa.

## Aplicação prática
- Recrute 10 usuários que sejam **proxy do mercado total** — documente por que cada um representa um segmento.
- Coloque todo o trio (PM + design + eng) nas chamadas — não filtre pela UXR.
- Crie um Slack compartilhado com os lighthouse users — presença contínua, não só entrevistas agendadas.
- Separe as métricas por stage: qualitativas para os primeiros 10-100, quantitativas apenas acima de 1000.
- Comunique os aprendizados internamente sempre via clips de vídeo curtos, não slides de pesquisa.

## Insights por autor
### [[Tanguy Crusson]]
- "I've seen a lot of teams... hiding behind research and not being close enough to the ground with customers."
- "All of a sudden you're not talking about a product manager, you're talking about a product team with product engineers."
- O princípio da mudança climática: conexão com a história individual muda comportamento, dado abstraído não.

> 🎧 [Hard-won lessons building 0 to 1 inside Atlassian | Tanguy Crusson](https://www.youtube.com/watch?v=cZqpqb5qR5A) · 2024-06-16

## Conceitos relacionados
[[Continuous Discovery]] · [[Solve before Scale]] · [[Marginal User]] · [[Point A — Incubação em 4 Fases]] · [[Obsessão por Redução de Fricção — Magia via Manual]]
