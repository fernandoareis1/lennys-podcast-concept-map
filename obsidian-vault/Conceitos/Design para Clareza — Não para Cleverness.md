---
tipo: framework
nivel: 3
fluxo: Design & UX
autores: [Robby Stein]
---
# Design para Clareza — Não para Cleverness

**Fluxo:** [[04 - Design & UX]] · **Tema:** [[Design — Experiência & fricção]] · **Camada:** L3
**Tipo:** Princípio · **Fontes:** [[Robby Stein]]

## Ideia central
Diferenciar pelo design é uma armadilha. Quando um ícone, nome ou padrão já é reconhecido pelo usuário, **reinventá-lo é trabalhar contra você mesmo**. A clareza entrega mais leverage que a criatividade.

Don Norman, em *The Design of Everyday Things*, usa portas como metáfora perfeita: depois de décadas, as pessoas ainda não sabem se devem empurrar ou puxar uma porta com duas alças simétricas em vidro. A porta foi projetada para ser bela, não para comunicar. O design falhou.

Em produtos digitais o padrão é idêntico:
- Criar um ícone de câmera que "é uma câmera mas tem pontos de IA que conectam ao produto vizinho e tem este detalhe visual" → os usuários simplesmente não clicam
- Chamar o produto de algo aleatório quando "AI Mode" comunica exatamente o que é

**Pessoas pensam espacialmente.** Se você tem um feed com holes para fotos, o usuário espera que esses holes se comportem de uma certa forma. Um hole que tem um clock e desaparece no dia seguinte e não tem like vai confundir — não por falta de inteligência, mas porque o contexto espacial criou expectativas específicas.

**Caso Close Friends:** a primeira versão exibia o indicador de "close friends story" *dentro* da story, depois que o usuário já abria. O time achava que era elegante (surpresa!). Os usuários simplesmente não sabiam que havia algo especial antes de abrir — e não abriam com expectativa diferente. A correção: anel verde *fora* da story, no tray. Óbvio. Funcionou.

O nome "AI Mode" é o mesmo princípio: ninguém precisa aprender o que é.

## Como aplicar
1. **Prefira ícones globais.** Se já existe um padrão universal (câmera, coração, lupa), use-o. Só invente um ícone novo quando a ação não tem equivalente existente.
2. **Nomeie pelo que é.** "AI Mode" > "Nano Search" > "Gemini Search Experience". A clareza no nome é design.
3. **Teste a expectativa espacial.** Onde o usuário espera ver o indicador? Onde os olhos vão naturalmente no layout? O indicador precisa estar lá, não onde o designer acha elegante.
4. **Quando reinventar, faça com clareza explícita.** Se você precisa quebrar a convenção, adicione sinalização extra (tooltip, onboarding, anel verde visível) para que a novidade não crie confusão.
5. **Distinção ≠ confusão.** Um produto pode ser distinto (Stories é diferente do feed) e ainda assim claro (o tray de circles no topo é imediatamente reconhecível).

## Insights por autor
### [[Robby Stein]]
- "A lot of people are like, 'We're going to differentiate the design.' If something's a standard and people understand it, if you lean into it, you're going to get so much leverage than if you reinvent it."
- "We designed new icons when we could have used global icons — 'a camera that's kind of a camera but has AI dots that connect it to another product.' People just, it's a camera. Just put the camera in."
- Sobre o nome "AI Mode": "We talked about it internally. If you look at it in the tab, you see it and you know what it is. Or we could call it something random — then what is that? And now you're working against yourself."
- Sobre o anel verde: "We were being cute. We thought it was a secret story. But we put the green ring on the outside so that users would see it in the tray and think 'Ooh, what's that little green guy?' And then they'd click."
- "People think spatially. If you have a feed with holes for pictures, they expect those holes to do things. If you make one of those holes have a clock and it's gone the next day and you can't like it, it's going to be super confusing."

> 🎧 [Inside Google's AI turnaround: AI Mode, AI Overviews, and vision for AI-powered search | Robby Stein (1:21:38)](https://www.youtube.com/watch?v=kOnsqqVbIeY) · 2025-10-10

## Conceitos relacionados
[[Melhoria Implacável — Insatisfação como Força Motriz]] · [[Adição Complementar vs. Substituição de Produto]] · [[Reduzir fricção em vez de adicionar features]] · [[Friction Logging]]
