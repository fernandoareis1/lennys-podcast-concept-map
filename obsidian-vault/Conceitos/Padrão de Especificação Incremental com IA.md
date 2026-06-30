---
tipo: tecnica
nivel: 3
fluxo: Design & UX
autores: [Michael Truell]
---
# Padrão de Especificação Incremental com IA

**Fluxo:** [[04 - Design & UX]] · **Tema:** [[Design — Experiência & fricção]] · **Camada:** L3
**Tipo:** técnica · **Fontes:** [[Michael Truell]]

## Ideia central
O erro mais comum ao trabalhar com IA para desenvolvimento é dar uma tarefa grande e esperar o resultado final. O padrão que funciona é especificação incremental: especifique um pouco → IA produz → revise → especifique um pouco mais → IA produz → revise. O tempo total de especificação pode ser o mesmo, mas dividido em pedaços menores a qualidade do resultado aumenta dramaticamente porque cada revisão informa a próxima especificação.

## Por que funciona
- Erros no entendimento da IA são detectados cedo, antes de se propagarem para um sistema maior
- O humano mantém controle da direção sem precisar detalhar cada passo desde o início
- A revisão frequente cria um loop de feedback que alinha o output ao intent real
- Tarefas menores têm menor variância — a IA performa melhor em escopo bem definido

## O espectro de interação
Há um espectro de como humano e IA colaboram:
- **Autocomplete** (menor especificação por iteração): sugestão palavra-a-palavra; humano dirige cada token
- **Edit inline**: humano especifica mudança pontual; IA aplica
- **Instrução de bloco**: "faça isso nessa função"; IA propõe; humano aprova
- **Agente com tarefa escoped**: "implemente esta feature"; IA age por múltiplos passos; humano revisa ao final

O padrão de especificação incremental funciona em todos os pontos do espectro — o princípio é o mesmo: menor escopo por iteração = melhor resultado.

## Insights por autor
### [[Michael Truell]]
- "I would chop things up into bits, and you can spend basically the same amount of time specifying things overall, but chopped up more. So you're specifying a little bit, you're getting a little bit of work, you're specifying a little bit, getting a little bit of work."
- "The most successful customers really lean on... scoping down the stuff that you're going to hand off to the bot... biasing toward chopping things up and making things smaller."
- "You can specify a little bit, AI writes something, review, specify a little bit, AI writes something, review. Autocompletes all in the way of that spectrum."
> 🎧 [How Cursor is building the future of coding (Michael Truell)](https://www.youtube.com/watch?v=En5cSXgGvZM)

## Conceitos relacionados
[[Programação por Intenção — Um Mundo Além do Código]] · [[Gosto Sobre Precisão — O Novo Skill do Engenheiro de IA]] · [[Vibe Coding — Delegar a Execução ao Modelo]] · [[De Saber a Fazer — A Transição dos Agentes de IA]]
