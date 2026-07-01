---
tipo: modelo-mental
nivel: 3
fluxo: Estratégia & Visão
autores: [Mike Krieger, Nick Turley]
---
# Produto na Interseção Modelo-Produto — Vantagem Única de IA

**Fluxo:** [[02 - Estratégia & Visão]] · **Tema:** [[Estratégia — Estratégia de produto]] · **Camada:** L3
**Tipo:** modelo mental · **Fontes:** [[Mike Krieger]] · [[Nick Turley]]

## Ideia central
Para uma empresa de AI labs, o único lugar onde produto tem vantagem defensável é na interseção entre pesquisa de modelos e experiência de produto. Construir produto que qualquer pessoa poderia fazer usando modelos disponíveis via API não é vantagem — é commodity. A pergunta estratégica correta é: "o que só é possível porque temos acesso único à pesquisa de modelo?" E isso muda a unidade funcional de trabalho: de "pegue o modelo e trabalhe com design e produto" para "participar das conversas de post-training sobre como o modelo deve se comportar".

## A nova unidade de trabalho em produto de IA
Na Anthropic, produto não começa após o modelo estar pronto — começa antes. PMs e designers participam de conversas sobre post-training: que comportamentos o modelo deve ter, como deve responder a casos ambíguos, qual é a personalidade certa. Isso cria produto que fundamentalmente não poderia ser construído por um wrapper externo.

## O teste estratégico
Para cada feature ou produto: se alguém de fora pudesse construir isso exatamente igual usando o modelo via API, você provavelmente não deveria estar construindo. Se a feature depende de:
- Acesso a fine-tuning ou post-training específico
- Integração com pesquisa de modelo que não é pública
- Capacidade de moldar comportamento de modelo que terceiros não têm

...então você está no espaço de vantagem única.

## Insights por autor
### [[Mike Krieger]]
- "Where we should play and what we can do uniquely should be stuff that's really at that magic intersection between the two [model research and product experience]."
- "The functional unit of work at Anthropic is no longer take the model and then go work with design and product to go ship a product. It's more like we are in the post-training conversations around how these things should work."
- "If we're shipping things that could have been built by anybody just using our models off the shelf... where we should play and what we can do uniquely should be stuff that's really at that magic intersection."
> 🎧 [Instagram co-founder on building AI products at Anthropic (Mike Krieger)](https://www.youtube.com/watch?v=DKrBGOFs0GY)

### [[Nick Turley]]
- "There really is no distinction between the model and the product. We iterate on model behavior the same way you'd iterate on a product: discovery, user research, data science."
- "We treat the model like a product. Understanding what users are trying to do and failing at is how we tell the ML team what to climb on."
> 🎧 [Inside ChatGPT: The fastest growing product in history (1:35:38)](https://www.youtube.com/watch?v=ixY2PvQJ0To) · 2025-08-09

## Conceitos relacionados
[[Ensemble de Modelos Especializados]] · [[Pós-treinamento como nova fronteira]] · [[Três pilares de IA em plataforma]] · [[Três segmentos do mercado de IA]]
