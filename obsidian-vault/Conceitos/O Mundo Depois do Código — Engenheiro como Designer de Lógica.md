---
tipo: framework
nivel: 3
fluxo: Estratégia & Visão
autores: [Michael Truell]
---
# O Mundo Depois do Código — Engenheiro como Designer de Lógica

**Fluxo:** [[02 - Estratégia & Visão]] · **Tema:** [[Estratégia — Visão, missão & narrativa]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Michael Truell]]

## Ideia central
A tese do Cursor é que o processo de construir software vai mudar fundamentalmente. Não é "você digita no Slack e pede ao bot para construir" (chatbot), nem é "nada muda, TypeScript para sempre" (código intacto). É algo mais estranho e mais poderoso que os dois.

A transição: das linguagens formais (TypeScript, Go, Rust) para uma representação de lógica que se parece com pseudocódigo ou inglês. O engenheiro ainda está no volante. Ele ainda controla cada detalhe. Mas o que ele descreve passa de "como implementar" para "o que quero que aconteça". A abstração sobe um nível.

## Duas visões erradas

**Visão 1 — o chatbot:** "Você digita no Slack o que quer, o AI constrói, você pede ajustes." O problema: imprecisão. Para ter controle completo sobre como o software funciona, você precisa de um formato mais preciso do que texto descritivo desconectado do código. Você não consegue "gesticular" o que quer.

**Visão 2 — código intacto:** "Vamos continuar escrevendo TypeScript para sempre." O problema: a tecnologia vai melhorar demais para que isso seja verdade por muito tempo.

## A aposta real: lógica legível por humanos

O mundo depois do código é aquele em que a representação da lógica do software:
- É mais tersa e mais fácil de entender do que milhões de linhas de código
- Evolui das linguagens formais em direção a pseudocódigo/inglês
- Pode ser editada diretamente pelo humano (não só descrita ao bot)
- Ainda dá controle completo sobre cada decisão do software

O loop de desenvolvimento vai se tornar muito mais rápido: especificar o intent → executar → ajustar, sem a camada de tradução trabalhosa que existe hoje entre "o que o time quer" e "o que o computador executa".

## O engenheiro como designer de lógica

A habilidade que cresce em valor: **taste** — ter a ideia certa sobre o que deve ser construído. Não taste visual (UI, animações). Taste sobre a lógica: como o software deve funcionar, que tradeoffs fazer, que comportamento especificar.

Hoje, "ser cuidadoso" é uma das habilidades mais críticas do engenheiro. No futuro, a balança vai pender mais para o taste (ideia certa) e menos para o cuidado (implementação correta de baixo nível).

## Implicação para o IDE

Se o que "construir software" significa vai mudar radicalmente nos próximos anos, a extensibilidade dos editores existentes é insuficiente para acompanhar. Logo, você precisa controlar o aplicativo inteiro — não apenas um plugin. Essa foi a lógica para construir um IDE próprio ao invés de ser um add-on para VS Code ou JetBrains.

## Insights por autor
### [[Michael Truell]]
- "More and more, being an engineer will start to feel like being a logic designer — specifying intent for how you want everything to work."
- "Taste will be increasingly important. Not just visual taste, but having the right idea for what should be built."
- "We think it ends up looking like something in between — not chatbot, not code-unchanged. Something weirder than both."
- "If you see insufficient ambition in the existing players, there's still opportunity — even in the 'hottest' space."
- "The extensibility of existing coding environments is so, so limited. If the form factor of programming is going to change, you need to own the whole app."

> 🎧 [The rise of Cursor: The $300M ARR AI tool that engineers can't stop using | Michael Truell](https://www.youtube.com/watch?v=En5cSXgGvZM)

## Conceitos relacionados
[[Inovação vs Otimização — O Flip em AI]] · [[Dados Sintéticos — Sem Parede de Dados no Pós-Treinamento]] · [[Visão como Fotografia do Futuro]]
