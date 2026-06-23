---
tipo: tecnica
nivel: 3
fluxo: Design & UX
autores: [David Singleton]
---
# Friction Logging

**Fluxo:** [[04 - Design & UX]] · **Tema:** [[Design — Experiência & fricção]] · **Camada:** L3
**Tipo:** Técnica · **Fontes:** [[David Singleton]]

## Ideia central
Colocar-se no lugar de um usuário específico, percorrer o produto de ponta a ponta e anotar em modo stream-of-consciousness *tudo* que causar fricção — especialmente nos momentos de alto risco como mensagens de erro e integrações. O resultado é um log que aponta exatamente *onde* vale investir meticulosidade.

O Stripe usa friction logging em múltiplas camadas: todo time de produto tem alguém que faz o percurso periodicamente; executivos séniores fazem o seu próprio loop; o CTO David Singleton percorria o onboarding de um novo usuário **todo mês** durante anos.

## Como aplicar
1. Defina claramente **quem é o usuário** que você está modelando antes de começar.
2. Percorra o produto de ponta a ponta (dashboard → docs → código → integração) e anote tudo que causar estranheza — não só o que quebra.
3. Marque os pontos de **maior fricção** para o perfil escolhido — eles são os candidatos a merecer atenção meticulous.
4. Compartilhe o log com as pessoas certas (PMs, EM, suporte) e decida o que priorizar.
5. Faça em ciclo: individual assíncrono + walkthrough coletivo periódico com todo o time cross-funcional.

## Insights por autor
### [[David Singleton]]
- "You need to put yourself in a particular user's shoes. It's actually important to have a very clear idea of who is the person I am kind of modeling the friction for right now."
- No Stripe há mais código tratando edge cases das APIs do que no fluxo principal — fruto direto de friction logging sistemático.
- Melhoria de checkout: migrar usuários do flow vanilla para Stripe Checkout gerou **+10,5% de receita** — resultado de compor pequenas melhorias meticulous ao longo do tempo.
- Engineers em "engineer occasions" também mantêm friction log durante os dias de trabalho IC — o log é depois compartilhado com o time e relido pelo próprio CTO ao longo do ano.

> 🎧 [Building a culture of excellence (1:30:00)](https://www.youtube.com/watch?v=F0_IKKY3HCk)

## Conceitos relacionados
[[Engineer Occasion]] · [[Design — Experiência & fricção]] · [[Understand Work (UIE)]] · [[Reduzir fricção em vez de adicionar features]]
