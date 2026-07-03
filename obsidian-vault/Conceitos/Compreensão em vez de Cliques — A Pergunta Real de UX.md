---
tipo: principio
nivel: 3
fluxo: Design & UX
autores: [Stewart Butterfield]
---
# Compreensão em vez de Cliques — A Pergunta Real de UX

**Fluxo:** [[04 - Design & UX]] · **Tema:** [[Design — Experiência & fricção]] · **Camada:** L3
**Tipo:** Princípio · **Fontes:** [[Stewart Butterfield]]

## Ideia central
O mantra "reduza fricção" e "reduza o número de cliques/toques" é **quase sempre a pergunta errada**. A pergunta certa é: o usuário **compreende** o que está vendo?

Há dois tipos de problema muito diferentes:
- **Problema de fricção**: o usuário sabe exatamente o que quer fazer e o produto está tornando difícil chegar lá. Reduza os passos. (Ex.: quem quer comprar um ingresso Taylor Swift no Ticketmaster — intenção 100%, clareza 100%)
- **Problema de compreensão**: o usuário não sabe o que é o produto, o que deveria fazer a seguir, ou o que vai acontecer se fizer alguma coisa. Reduzir cliques aqui não ajuda em nada.

A maioria dos produtos B2B e de comportamento novo tem **problema de compreensão**, não de fricção. Slack era assim: qualquer novo usuário que chegava ao site tinha intenção zero ponto alguma coisa acima do threshold mínimo. O obstáculo não era o número de passos — era entender o que diabos era aquilo.

## Por que o mantra de "reduza cliques" é enganoso
Você pode tornar qualquer ação em um único clique **expondo todas as opções na tela ao mesmo tempo** — e criar uma experiência terrível. O ideal não é um clique; é que cada micro-decisão seja **trivialmente fácil**.

> "Eight clicks or taps to do something, but every single one is trivially easy — that's great. Two clicks or taps where every part is a fraught decision and I'm comparing 15 options — that becomes impossibly expensive."

**Por que fazer pensar é custoso**:
1. **Biológico**: tomar decisões literalmente queima glicose e ATP. Há custo metabólico real.
2. **Emocional**: se o produto te para e te faz sentir que você não entende, você se sente estúpido. As pessoas associam esse sentimento ao produto para sempre.

## Dos princípios ao design
O mantra de Stewart: **"Don't Make Me Think"** (livro de Steve Krug) — reduzir qualquer necessidade de decidir sem entender o impacto.

Aplicações práticas:
- Em vez de "como reduzimos de 5 para 3 passos?" → "o usuário sabe o que vai acontecer depois de cada passo?"
- Em vez de "qual é a ação padrão?" → "o usuário consegue entender qual das opções fazer sem ter que compará-las todas?"
- Menus longos: nunca exponha tudo. Mostre as 2-3 coisas mais comuns e ponha o resto em "Outros" (Uber original: "Para onde você quer ir?" e "Outros")
- Navegação: agrupe visualmente itens relacionados; hierarquia visual reduz carga cognitiva mais do que reduzir quantidade

## Casos concretos da Slack
- **Magic link no mobile**: em vez de pedir senha (digitação difícil em mobile com senha complexa), envie link por email que abre e autentica automaticamente. Reduziu compressão cognitiva, não cliques.
- **Notificações padrão vs. recomendadas**: novos usuários esperavam notificação de cada mensagem (padrão histórico de apps). Slack sabia que isso seria ruim. Solução: ativar o padrão esperado primeiro, depois de 10 mensagens recebidas oferecer a configuração recomendada. Ensinou o produto dentro do uso.
- **Shouty Rooster (@everyone)**: em vez de remover a feature ou escondê-la, adicionou fricção estratégica — um galo animado avisando "você vai notificar 147 pessoas em 8 fusos horários, tem certeza?" Compreensão, não remoção.

## Insights por autor
### [[Stewart Butterfield]]
- "It became like an assumption that you should always be trying to remove friction when the challenge is really comprehension."
- "If you can't teach them or make it possible for them to discover what the capabilities are, then they're not going to take advantage of them."
- "If your software stops me and asks me to make a decision and I don't really understand it, you make me feel stupid."
- "People coming to Slack.com — their intent was at the absolute minimum threshold... what we had to worry about was creating comprehension in two senses: what is this thing? And what am I supposed to do next?"
- "If people could get over the idea of reducing friction as the number one goal and instead focus on: how can I make this simple? How do I prevent people from having to think in order to use my software?"

> 🎧 [Mental models for building products people love ft. Stewart Butterfield](https://www.youtube.com/watch?v=kLe-zy5r0Mk) · 2025-11-20

## Conceitos relacionados
[[Ilusão do Dono — O Viés do Criador do Produto]] · [[Reduzir fricção em vez de adicionar features]] · [[Onboarding que Usa o Produto para Ensinar]] · [[Conveniência como Lei Termodinâmica da Adoção]] · [[Clareza sobre Engenhosidade — Design Legível]]
