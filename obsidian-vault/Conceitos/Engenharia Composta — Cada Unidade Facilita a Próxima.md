---
tipo: framework
nivel: 3
fluxo: Liderança & Times
autores: [Dan Shipper]
---
# Engenharia Composta — Cada Unidade Facilita a Próxima
**Fluxo:** [[09 - Liderança & Times]] · **Tema:** [[Liderança — Modelos de time]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Dan Shipper]]

## Ideia central
Em um time que usa IA para construir produto, a disciplina de "engenharia composta" é: **cada unidade de trabalho deve tornar a próxima unidade de trabalho mais fácil**.

O padrão default (e ineficiente): cada PRD que você escreve para um agente custa o mesmo esforço. Você vira um digitador de PRDs.

O padrão composto: você gasta energia uma vez para criar um prompt que transforma seus pensamentos desestruturados em um PRD bem formado. A partir daí, todos os PRDs futuros custam menos — e você investe essa diferença em fazer o próximo nível de automação.

**Como se manifesta na prática:**
- Prompts e slash commands no Claude Code que codificam padrões recorrentes
- Uma biblioteca compartilhada de comandos no GitHub que o time inteiro reutiliza
- Fluxos de automação (n8n, Make, scripts) para os workflows mais repetidos da equipe
- O Cora team (2 engenheiros + 15 instâncias de Claude Code) construiu um produto com 2.500 usuários ativos e milhões de emails processados — porque cada sprint tornou o próximo sprint mais eficiente

**Head de AI Operations como função organizacional:**
O risco da engenharia composta é que ninguém tem tempo de construir as automações enquanto está combatendo incêndios. A solução é um **Head de AI Operations** — uma pessoa dedicada a:
1. Acompanhar onde o time está repetindo tarefas manualmente
2. Construir os prompts e automações correspondentes
3. Garantir que o time realmente use (behavioral update)

O background ideal: curioso por IA, orientado a processos, entende o craft da função que está automatizando.

## Como aplicar
1. **Crie uma lista de repetições:** qualquer tarefa que você faz mais de uma vez por semana é candidata a automação; liste-as e priorize pela frequência × esforço
2. **Reserve 20% do sprint para automação:** defina um ritual (ex: sexta de tarde) onde alguém do time constrói a automação da semana em vez de só entregar features
3. **Compartilhe o acúmulo:** prompts, slash commands, scripts — guarde em um repositório acessível ao time inteiro; o acúmulo coletivo é o moat
4. **Contrate/identifique um Head de AI Ops:** esta função tem mais ROI que contratar o décimo engenheiro — uma boa pessoa de AI ops multiplica todos os outros
5. **Meça a aceleração:** compare o tempo médio por PR/feature hoje vs. há 3 meses; se não está caindo, a engenharia composta não está funcionando

## Insights por autor
### [[Dan Shipper]]
- "For every unit of work, you should make the next unit of work easier to do."
- "You spend a little bit of work to make all of the next PRDs that you're doing easier to write because you're writing less of them."
- "Having an AI operations lead lets you basically identify those things and have them solved without people who are doing the work actually having to take time to do it."
- "With Cora, it's Kieran, Nityesh, and 15 Claude Code instances — so it's more powerful than you think."
- Sobre o Head de AI Ops ideal: "At minimum, you really just want someone who's like, 'I want to tinker. I want to build stuff.' There's also people who have a little bit more of that process orientation."

## Conceitos relacionados
[[Compressão do Talent Stack por IA]] · [[CEO como Catalisador de Adoção de IA]] · [[Incubação pelo Uso Próprio]] · [[Produto-Ops como avião bimotor]] · [[Economia de Alocação]]
