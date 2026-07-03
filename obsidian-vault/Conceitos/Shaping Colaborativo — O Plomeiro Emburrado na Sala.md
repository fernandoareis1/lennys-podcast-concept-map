---
tipo: framework
nivel: 3
fluxo: Priorização & Roadmap
autores: [Ryan Singer]
---
# Shaping Colaborativo — O Plomeiro Emburrado na Sala

**Fluxo:** [[03 - Priorização & Roadmap]] · **Tema:** [[Priorização — Estratégia vs execução]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Ryan Singer]]

## Ideia central
O erro mais comum ao tentar o Shape Up é fazer shaping *sem* engenheiro. O produto e o designer ficam num quarto, produzem uma especificação bela — e quando apresentam ao time de build, tudo explode. A realidade técnica não estava na sala.

**O "plomeiro emburrado":** Ryan Singer usa a analogia do encanador veterano que insiste em abrir as paredes antes de dar qualquer orçamento. Esse é o engenheiro sênior que você precisa trazer para a sessão de shaping — não o PM, não o designer — mas a pessoa que sabe onde os corpos estão enterrados, o que é fácil, o que é difícil, como a infraestrutura atual funciona de verdade.

**O que acontece na sessão:**
1. Começa com o problema estreitado (framing já feito)
2. O trio (PM + designer + eng sênior) tenta ideias numa lousa ou papel
3. Cada ideia é imediatamente testada: a técnica bate? O produto realmente resolve o problema?
4. Rabbit holes e "bombas-relógio" são identificados antes que o projeto esteja em andamento
5. Se for descoberta uma complicação (ex: 3 branches de código diferentes para o mesmo onboarding step), o grupo faz trade-offs *agora*, não na semana 4

**Sinal de boa sessão:** você consegue descrever o que vai ser construído em **menos de 10 moving parts**. Se precisar de mais, o projeto não está suficientemente shaped. O kit básico do calendário: grade de dois meses com dots, view de agenda que desliza embaixo, botão de criar evento, navegação entre meses. Isso cabe em 5 items.

**Fat marker sketches, não Figma:** o artefato da sessão é um esboço de marcador grosso — uma comunicação rápida da ideia que qualquer engenheiro pode ler e dizer "entendi o que vai ser construído." Se o esboço não diz ao eng o que construir, ele não é útil.

**Dica para times mistos:** o nível de detalhe do shaping deve ser calibrado pelo nível de senioridade do time de build. Para times mais juniores, mais detalhe ajuda. Para seniores, menos detalhe libera criatividade.

## Como aplicar
1. **Identifique seu "plomeiro".** Quem na sua empresa sabe onde os corpos estão enterrados tecnicamente? Essa pessoa deve estar na sessão de shaping — não só consultada depois.
2. **Comece com o problema estreitado** (framing prévio). Se o problema for "calendar", a sessão vai se expandir para sempre.
3. **Tente e quebre ideias alternativas.** Não vá fundo numa ideia — explore alternativas rapidamente (e se não tivéssemos o agenda view, tem outro jeito?).
4. **Identifique rabbit holes explicitamente.** Pergunte: "Quais são os time bombs aqui que podemos revelar agora antes que sejam uma crise?"
5. **Valide com o critério dos 10 moving parts.** Se você não consegue descrever o que vai ser construído em menos de 10 itens, o shaping não está completo.

## Insights por autor
### [[Ryan Singer]]
- "O principal modo de falha que vejo no mundo real é sempre, de novo e de novo, pouca clareza. E também o modo de falha mais comum é o engenheiro correr de volta ao produto dizendo: 'não estou recebendo o suficiente de vocês.'"
- "Você tem que ter o engenheiro que realmente insiste em abrir as paredes e olhar os canos antes de dar um orçamento. Quando você tem essa pessoa na sala, em momentos, você abre o código e você realmente olha."
- "Depois de 6 semanas, isso é 30 dias úteis. Divida por 9 — são 4 dias por box. Você obtém muita clareza de um exercício rápido."
- "É shaped se você pode dar isso a uma pessoa técnica e ela diz: 'Sim, sei o que construir agora.'"
- "Nós precisamos ter toda a informação necessária na mesma sala para essas sessões irem rápido."

> 🎧 [A better way to plan, build, and ship products | Ryan Singer (1:45:10)](https://www.youtube.com/watch?v=GF-yUANql0c) · 2025-03-30

## Conceitos relacionados
[[Shape Up — Apetite Fixo e Escopo Variável]] · [[Framing — Estreitar o Problema antes de Shapear]] · [[De-riscar os Maiores Bets Primeiro]] · [[Armadilha do Prazo — Velocidade por Tempo, não Esforço]]
