---
tipo: framework
nivel: 3
fluxo: Design & UX
autores: [Kevin Weil]
---
# Raciocinar como Humano sobre IA — UX de Modelos de Raciocínio

**Fluxo:** [[04 - Design & UX]] · **Tema:** [[Design — Experiência & fricção]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Kevin Weil]]

## Ideia central
Ao projetar experiências com modelos de IA, especialmente modelos de raciocínio que "pensam" antes de responder, a heurística mais poderosa é: **trate a IA como trataria um humano em situação equivalente**.

**Exemplo fundacional — o "thinking" do o1:**
Quando a OpenAI lançou o modelo o1 (que raciocina antes de responder), a equipe de produto precisava decidir como mostrar ao usuário que o modelo estava "pensando". Kevin usou a pergunta: "Se você me fizesse uma pergunta que precisasse de 20 segundos para pensar, o que eu faria?"

Resposta óbvia: você pensaria em voz alta, mostraria progresso, não ficaria em silêncio. Isso levou à decisão de mostrar o "pensamento em andamento" do modelo durante o raciocínio — feature que se tornou central na experiência do o1.

**Por que essa heurística funciona:**
LLMs são treinados em texto humano. Seus comportamentos, capacidades e limitações têm análogos humanos. Quando designers pensam neles como "oráculos computacionais" em vez de "entidades que raciocinam como humanos", tomam decisões de UX que criam experiências estranhas.

**Exemplos de aplicação:**
- Latência tolerável: quanto tempo um humano aceitaria esperar antes de abandonar? Mesma lógica para o modelo.
- Tom e assertividade: como um especialista humano comunicaria confiança vs. incerteza? O modelo deve fazer o mesmo.
- Pedido de clarificação: um humano perguntaria antes de responder a uma ambiguidade? O modelo também deveria.

## Como aplicar
1. Para qualquer decisão de UX de IA, pergunte: "Como um humano equivalente se comportaria nessa situação?" Use isso como ponto de partida.
2. Para modelos com latência (raciocínio, pesquisa): mostre progresso, não silêncio. Comunique o que está sendo processado.
3. Para incerteza do modelo: mostre grau de confiança como um humano faria — "acho que...", "tenho certeza que..." — em vez de output binário.
4. Para limites do modelo: permita que ele "peça ajuda" ou "declare o que não sabe", como um humano competente faria.
5. Teste experiências de IA com usuários perguntando: "Se fosse um ser humano fazendo isso, o que você esperaria?" Desvios dessa expectativa são bugs de UX.

## Insights por autor
### [[Kevin Weil]]
- Heurística central: "Ao projetar experiências com IA, raciocine sobre elas como raciocínio sobre humanos."
- Exemplo específico: o "thinking" do o1. "Se você me perguntasse algo que eu precisasse pensar por 20 segundos, o que eu faria?" → Isso levou a mostrar o raciocínio em andamento.
- "Há análogos humanos de quase tudo que estamos construindo em IA. Essa analogia é sempre o ponto de partida."
- Incluindo prompting ("você é Einstein, resolva esse problema") — funciona porque os modelos respondem ao enquadramento de papel, como humanos respondem a contexto social.
- Citou a conexão com como humanos respondem a framing: colocar alguém em certo estado mental muda completamente a resposta.

> 🎧 [OpenAI's CPO on why ChatGPT is the worst AI you'll ever use | Kevin Weil](https://www.youtube.com/watch?v=scsW6_2SPC4) · 2025-04-10

## Conceitos relacionados
[[NLX é o novo UX]] · [[Chat como Interface Universal]] · [[Assistência Contextual Mista]] · [[Non-determinismo em Produtos de IA]] · [[Do Computador Pessoal ao Modelo Pessoal]]
