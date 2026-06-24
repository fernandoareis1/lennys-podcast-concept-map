---
tipo: tática
nivel: 3
fluxo: Liderança & Times
autores: [Farhan Thawar]
---
# Pair Programming como Ferramenta de Gestão

**Fluxo:** [[09 - Liderança & Times]] · **Tema:** [[Liderança — Modelos de time]] · **Camada:** L3
**Tipo:** Tática · **Fontes:** [[Farhan Thawar]]

## Ideia central
Pair programming é a ferramenta de gestão de engenharia **mais subutilizada** que existe. A ilusão de que "dois engenheiros num mesmo computador produzem metade" ignora que o gargalo não são mãos no teclado — é encontrar a solução elegante. Dois pares produzem menos código e mais valor.

## Por que funciona
- O gargalo é encontrar o design certo, não digitar — dois pares aceleram o pathfinding
- **Transferência de conhecimento** é contínua: você aprende atalhos de teclado, forma de pensar e domínio do outro em tempo real
- **Intensidade** é maior: dois pares sem distrações entram em foco profundo; tão intenso que iniciantes dormem 10-12h/noite nos primeiros dias
- **Qualidade**: menos bugs, menos silos, soluções mais elegantes; estudos mostram happiness e knowledge-transfer mais altos

## A regra de Tobi (1 hora)
Toby Lütke e o CTO Cody Fauser praticavam: se em 1 hora não terminaram, **deletam todo o código, ficam com os testes, e começam do zero**. Lógica: "se não conseguimos escrever isso em 1 hora, estamos no design errado." Às vezes Toby excedia por 1 minuto e ainda assim deletava. A solução elegante cabe em 1 hora.

## Como o Shopify usa hoje
Não é 40h/semana como no Pivotal Labs (ambientes de contract manufacturing). É **4-8h/semana** na Shopify — ferramenta cirúrgica para:
- Pathfinding conjunto em problemas complexos
- Incidentes (deux pares diagnosticam mais rápido)
- Momentos onde o design está claro e a velocidade de escrita importa
- Onboarding de novos engenheiros em código existente

## Analogia do lance livre
Como o arremesso por baixo no basquete: estatisticamente superior, mas ninguém faz porque "parece idiota". Shaquille O'Neal, com falhas notórias em lances livres, se recusou a fazer o arremesso por baixo porque "parece dumb." Pair programming é exatamente isso: counterintuitive, mas funciona.

## Com IA
AI copilots (Cursor, Copilot) tornaram-se o "pair" para quando não há humano disponível. A tese de Farhan: AI copilot + dois humanos é melhor ainda — o AI gera, os humanos refinam, questionam e deletam.

## Insights por autor
### [[Farhan Thawar]]
- "Pair programming is the most underutilized management tool in engineering, bar none."
- "The throughput limiter is not hands on keyboard. It's: where is the good, elegant solution?"
- "Code is a liability. The right, usually shorter and more elegant solution appears after pathfinding. The only way to do that is to start, delete, and start again."
- Rodou a maior operação de pair programming do mundo no Pivotal/Xtreme Labs

> 🎧 [How Shopify builds a high-intensity culture | Farhan Thawar (1:40:03)](https://www.youtube.com/watch?v=C_lhMOjG7PE) · 2024-12-19

## Conceitos relacionados
[[Engineer Occasion]] · [[IA amplifica os Melhores]] · [[Compressão do Talent Stack por IA]] · [[Engenheiros Orientados a Produto]]
