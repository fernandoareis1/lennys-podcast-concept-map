---
tipo: critica
nivel: 3
fluxo: Discovery & Pesquisa
autores: [Sriram Krishnan, Aarthi Ramamurthy]
---
# JTBD e o Problema Multi-Agente — Plataformas vs. Usuário Único

**Fluxo:** [[01 - Discovery & Pesquisa]] · **Tema:** [[Discovery — Jobs to be Done (teoria da demanda)]] · **Camada:** L3
**Tipo:** Crítica de framework · **Fontes:** [[Sriram Krishnan]], [[Aarthi Ramamurthy]]

## Ideia central
Jobs-to-be-Done pressupõe que você está otimizando para **um usuário realizando uma tarefa**. Em produtos com múltiplos agentes — redes sociais, marketplaces, plataformas — essa premissa quebra. Com frequência, a decisão certa de produto é **piorar a experiência de A para melhorar a de B**. JTBD não oferece nenhum instrumento para raciocinar sobre esse trade-off.

## Os exemplos concretos

**Facebook — "People You May Know"**
Ao criar uma conta no Facebook, você recebia sugestões de conexões. Em muitos casos, essas sugestões eram de pessoas que precisavam de amigos, não de você. O produto deliberadamente degradava sua experiência (sugestões de estranhos) para melhorar a experiência delas (ganhar a 10ª conexão em 14 dias — o threshold de ativação). Nenhum job seu estava sendo realizado: era o job deles.

**Twitter — Ranking Algorítmico**
O maior lançamento de produto dos últimos cinco anos no Twitter foi o feed algorítmico. Usuários avançados odiaram: eles queriam controlar o próprio timeline. Mas para o usuário mediano que acaba de entrar, o feed cronológico era ruído. A decisão de piorar a experiência do power user para servir o usuário regular salvou a empresa — e o TikTok é a prova que essa era a aposta certa. JTBD de power users teria vetado o lançamento.

**Amazon — Email de Confirmação**
Durante anos, a Amazon enviava emails detalhados com o conteúdo do pedido. Deixou de fazer. Razão: evitar que o Google tivesse esses dados indexados no Gmail. Motivação legítima de negócio, mas pior para o usuário. Nenhum "job" justificaria essa mudança — mas foi a decisão certa.

## Por que o framework falha nessas situações
1. **Múltiplos sujeitos** — em plataformas, não há "o usuário"; há compradores, vendedores, criadores, consumidores, com incentivos frequentemente opostos.
2. **Sistemas com externalidades** — o que você faz para um agente afeta automaticamente outros. JTBD não modela externalidades.
3. **Horizontes de tempo distintos** — sacrificar DAU de curto prazo (power users frustrados) pode ser correto no longo prazo (maior mercado endereçável). JTBD olha para o job hoje.
4. **Razões estratégicas/competitivas** — decisões legítimas de negócio (bloqueio de dados de concorrente, supply chain, regulação) não se encaixam em nenhuma narrativa de "job".

## Alternativa: Pensamento Sistêmico
Mapeie **todos os agentes** no sistema, seus **incentivos** individuais e como **interagem entre si**. Então a pergunta muda de "qual job estou realizando?" para "dado esse sistema, qual trade-off entre agentes gera o maior valor líquido?"

> "Think of all the players in the system, think of all of their incentives and how they interact with each other... then you can have a much more rational discussion about whether that trade-off is worth it." — Sriram Krishnan

## Quando JTBD ainda funciona
Sriram reconhece que a crítica é "bombástica" e que JTBD tem aplicações — especialmente em produtos de usuário único no estágio inicial (v1), quando você está testando uma hipótese de valor central com um único perfil de cliente. A partir do v2/v3, quando o produto amadurece e os trade-offs entre segmentos aparecem, o framework perde tração.

> "It might work for the V1 or just a hypothesis you're trying to go test out... but really V2, V3, it kind of falls apart." — Aarthi Ramamurthy

## Insights por autor
### [[Sriram Krishnan]]
- "I hate Jobs-to-be-Done, I think it is a terrible framework, I think no successful company has ever been built on top of JTBD and if you pick JTBD, you're probably doomed."
- "When you sign up for Facebook for many, many years, Facebook knew that it needed to get you to 10 friends in 14 days... What Facebook did was it made your experience slightly worse to make that person's experience slightly better. This was performing no job for you, it was trying to perform a job for them."
- "Real life and real product is all about these trade-offs and whenever I've seen people trot out JTBD, it's a tell that they actually haven't dealt with a trade-off."
- "Whenever I get a great product breakthrough... it comes from one person having a product intuition about something, about the psychological thing the product delivers, and systems thinking. Those are the only two places I've ever seen it come up."

### [[Aarthi Ramamurthy]]
- "It's almost meant for people who are so naive about product building and especially product building at scale."
- "V2, V3, it kind of falls apart because you have these super hard trade-offs that you have to make and every company goes through that. So it's almost a little too idealistic in its thinking."

> 🎧 [Hot takes and techno-optimism from tech's top power couple | Sriram and Aarthi](https://www.youtube.com/watch?v=HsD5ycT_umw) · 2023-03-12

## Conceitos relacionados
[[Jobs to be Done (JTBD)]] · [[JTBD — Debate (as escolas do JTBD)]] · [[Nuance acima de Frameworks — O Limite das Metodologias]] · [[Três Tipos de Efeito de Rede]] · [[Marketplace como Jardineiro]]
