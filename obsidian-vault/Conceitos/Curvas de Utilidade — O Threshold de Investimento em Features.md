---
tipo: framework
nivel: 3
fluxo: Priorização & Roadmap
autores: [Stewart Butterfield]
---
# Curvas de Utilidade — O Threshold de Investimento em Features

**Fluxo:** [[03 - Priorização & Roadmap]] · **Tema:** [[Priorização — Priorização & foco]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Stewart Butterfield]]

## Ideia central
Features não são binárias (tem/não tem). Elas seguem uma **curva S**: abaixo de certo limiar de investimento, o valor gerado é zero ou quase zero. Acima desse limiar, o valor dispara. E além de um ponto de saturação, o investimento adicional retorna pouco.

A pergunta certa ao discutir uma feature não é "devemos fazer isso?", mas: **em que ponto da curva estamos?** E a próxima unidade de investimento ainda está na parte íngreme ou já chegamos na cauda de retornos decrescentes?

## A curva na prática

```
Utilidade
 │
 │                    ╭────────────────────  (saturação)
 │                   ╱
 │                  ╱  ← parte íngreme: retornos explosivos
 │─────────────────╱   ← threshold
 │ (quase zero)
 └───────────────────────────────► Investimento
```

**Exemplo do martelo**: se o cabo quebra com qualquer impacto, o martelo é inútil. Ficando um pouco mais forte, ainda é inútil. Em algum ponto, ele atinge a resistência mínima para funcionar — e aí passa a ter valor. Além disso, adicionar mais qualidade ao cabo faz pouco.

**Exemplo de app**: criar a tabela de usuários no banco de dados não gera nenhum valor ao cliente. Depois de centenas de horas de desenvolvimento, o app passa a funcionar. Mas adicionar a 50ª funcionalidade que ninguém usa retorna quase nada.

## Por que isso importa para priorização
1. **A feature foi implementada uma vez, nunca mais melhorada**: a maioria das features fica na parte inicial da curva (abaixo do threshold) porque foram lançadas, nunca atingiram o ponto de virar insubstituíveis, e foram esquecidas. Esquecemos de subir a curva.
2. **Testar no limiar errado**: times fazem A/B test de uma feature que está na cauda de saturação (ganho máximo de 0.03 pontos percentuais) enquanto outras features estão ainda abaixo do threshold e não geram valor nenhum.
3. **O bar sobe sempre** ("divine discontent" — Bezos): padrões de usuários evoluem. A curva se move para cima e para a direita continuamente. O que era suficiente ontem é insuficiente hoje.

## Como usar
- Para cada área do produto, pergunte: "Estamos abaixo do threshold, no meio da curva, ou na saturação?"
- Abaixo do threshold → invista mais até passar o ponto de inflexão ou abandone
- Na parte íngreme → invista agressivamente
- Na saturação → pare; redirecione o esforço para outra curva que está abaixo do threshold
- Experiências críticas (login, checkout, onboarding) **nunca estão na saturação** porque o bar continua subindo — estas merecem atenção periódica mesmo quando "boas o suficiente"

## Insights por autor
### [[Stewart Butterfield]]
- "Features are thought of as a binary. You either have this feature or you don't. The argument was: have we just not invested enough in this, or have we got all the value out of this and we're in diminishing returns?"
- "People will add a feature, it's not good enough so people don't use it or appreciate it, but now you've added some complexity to the app, and then people give up."
- "The line actually moves because once people are familiar with a piece of software... their standards go up. There's this competition." (Bezos's "divine discontent")
- "If you can't see almost limitless opportunities to improve, then you shouldn't be designing the product."

> 🎧 [Mental models for building products people love ft. Stewart Butterfield](https://www.youtube.com/watch?v=kLe-zy5r0Mk) · 2025-11-20

## Conceitos relacionados
[[ICE (priorização)]] · [[Feature como Adotar um Cachorro]] · [[Custos de Terceira Ordem da Complexidade]] · [[Reduzir fricção em vez de adicionar features]] · [[99% Done ≈ 0% Done]]
