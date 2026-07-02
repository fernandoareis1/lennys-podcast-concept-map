---
tipo: mindset
nivel: 3
fluxo: Experimentação & Dados
autores: [Nick Turley]
---
# Velocidade antes do Polimento em IA

**Fluxo:** [[05 - Experimentação & Dados]] · **Tema:** [[Experimentação — Aprender com pouco e qualitativo]] · **Camada:** L3
**Tipo:** Mindset · **Fontes:** [[Nick Turley]]

## Ideia central
Em produtos de IA, as propriedades do produto são **emergentes** — você só descobre o que vale polir *depois* de colocar o produto nas mãos dos usuários. Polir antes de ship significa polir as coisas erradas.

Isso inverte a sabedoria tradicional de craft: o bom PM de produto de consumo clássico é artesão, cuida de cada detalhe antes de lançar. No contexto de IA, esse instinto trabalha contra você porque:
1. O espaço de uso cases real é imprevisível — você precisa de dados reais de uso
2. Os modelos mudam constantemente — o que você poliu fica obsoleto
3. Casos de falha reais (não benchmarks) são o insumo crítico para melhorar o modelo

**Shipping é o início da iteração, não o fim.** A velocity não é desculpa para nunca polir — é uma estratégia para descobrir *o que* polir com evidência real.

O ChatGPT foi originalmente um codebase de hackathon, lançado sem expectativa de sucesso. O model chooser (dropdown enorme, anti-pattern de UX) foi enviado intencionalmente porque aprender com usuários era mais valioso que esperar por uma UI perfeita.

## Como aplicar
1. **Pergunte: o que eu preciso aprender que só posso aprender via ship?** Se a resposta for algo crítico, priorize velocidade.
2. **Identifique o que pode ser polido com dados de uso** versus o que pode ser polido antes — polir output do modelo *pode* ser feito antes; a UI do feature pode ser descoberta depois.
3. **Trate o lançamento como ponto na jornada, não como destino.** Comprometa-se com a iteração pós-lançamento antes de lançar.
4. **Colete failure cases reais.** Benchmarks saturados não revelam o que o modelo falha no mundo real; só uso real faz isso.
5. **Não use velocidade como desculpa.** Uma vez que sabe o que polir, não há desculpa para não polir.

## Insights por autor
### [[Nick Turley]]
- "You won't know what to polish until after you ship. And I think that is uniquely true in an environment where the properties of your product are emergent and not knowable in advance."
- O model chooser (dropdown gigante, anti-pattern de UX): "It's embarrassing, but that's strictly less bad than not getting the feedback you wanted."
- "Shipping is just one point on the journey towards awesomeness, and you should pick that point intentionally — you better follow through."
- "A company with a lot of process will make one call, which is 'we have a quality bar when we ship.' If you reason from first principles, I think you're like, 'We should ship. It's embarrassing, but we should ship.'"
> 🎧 [Inside ChatGPT: The fastest growing product in history (1:35:38)](https://www.youtube.com/watch?v=ixY2PvQJ0To)

## Conceitos relacionados
[[Era dos evals — o eval é o PRD do modelo]] · [[Non-determinismo em Produtos de IA]] · [[Experimentação — AB testing & cultura]] · [[10% Rule — Hipótese Antes da Metade]] · [[Tradeoffs Explícitos para Aumentar Velocidade]]
