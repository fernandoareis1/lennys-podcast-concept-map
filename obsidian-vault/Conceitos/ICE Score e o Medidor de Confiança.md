---
tipo: tecnica
nivel: 3
fluxo: Priorização & Roadmap
autores: [Itamar Gilad]
---
# ICE Score e o Medidor de Confiança
**Fluxo:** [[03 - Priorização & Roadmap]] · **Tema:** [[Priorização — Priorização & foco]] · **Camada:** L3
**Tipo:** Técnica · **Fontes:** [[Itamar Gilad]]

## Ideia central
ICE (Impact, Confidence, Ease) é um framework de priorização de ideias de produto. O diferencial de Itamar é o **Medidor de Confiança** — um espectro visual de 0 a 10 que torna explícito quais tipos de evidência correspondem a quais níveis de confiança, prevenindo o maior problema: dar alta confiança a evidências fracas.

## Os 3 componentes do ICE

### Impact (Impacto)
Quanto a ideia vai mover as métricas que importam (North Star, top KPI, ou métricas locais do time). Estimar o impacto **antes de construir** é o exercício de pensamento crítico mais valioso — força a articular suposições explicitamente.

### Confidence (Confiança)
Quão certo você está das estimativas de impacto e facilidade. É aqui que o Medidor de Confiança entra. A tendência natural é dar alta confiança baseado em feeling — o medidor corrige isso ao amarrar confiança a tipos específicos de evidência.

### Ease (Facilidade)
O inverso de esforço: quão fácil ou difícil é implementar. Itamar prefere "ease" (criação de Sean Ellis) a "effort" — a inversão muda o frame mental para positivo.

## O Medidor de Confiança (0 a 10)

### Zona Azul (Baixa confiança — 0.01)
- Autoconvicção / instinto
- Pitch deck elaborado ou documento detalhado
- Suporte temático ("está alinhado com IA / blockchain / tendência X")

**Problema**: a maioria das pessoas dá confiança alta baseada aqui — "subverte o sistema inteiro"

### Zona Média (0.1 a 0.4)
- Review de colegas ou stakeholders
- Cálculo no verso do envelope (back-of-envelope)
- Dados anedóticos: concorrente tem isso / cliente mencionou / poucos pontos de dados
- Dados de mercado: pesquisas, análise competitiva, grandes datasets

### Zona Vermelha (Alta confiança — 0.4 a 10)
Versões testadas e construídas:
- **Testes de baixa fidelidade**: fake door, smoke test, Wizard of Oz, concierge test, teste de usabilidade
- **Versões rough**: early adopter programs, alpha/beta, fish food (testar internamente primeiro)
- **Testes completos**: previews, betas, labs
- **Experimentos com controle**: A/B tests, testes multivariados
- **Release progressiva**: stage releases, holdbacks, rollbacks

## O truque: comece baixo, suba progressivamente
Não é necessário começar na zona vermelha (caro). Comece com testes de baixíssimo custo para mover do 0.01 para 0.1. Depois de 0.1 para 0.4. Só vá para experimentos caros quando a confiança já é razoável.

Exemplo do Gmail Tabbed Inbox: Wizard of Oz test — HTML estático mascarando como Gmail real. Usuários achavam que estavam usando o Gmail, mas era só uma fachada. Custo mínimo, insight máximo.

"A chave é que você não tem que começar no lado direito, que é caro. Você pode começar cedo e isso leva a testar muitas ideias rapidamente."

## Quando parar de testar
"O risco é baixo, você pode lançar sem testar. Parte do truque também é saber quando parar — não apenas forçar o caminho todo para cima quando você não precisa."

Para bugs simples, melhorias óbvias de UX, ou features técnicas sem ambiguidade de produto: não precisa subir ao topo do medidor.

## O problema da alta confiança prematura
O maior risco prático: pessoas tendem a dar alta confiança baseada em gut feeling e então marcar como confirmado. "Encontrei isso um pouco perturbador porque subverte o sistema inteiro."

Solução: o Medidor de Confiança como artefato visual explícito — quando você debate confiança, você debate o tipo de evidência que a sustenta, não o feeling.

## Insights por autor
### [[Itamar Gilad]]
- "Impact, Confidence e Ease — basicamente uma maneira de atribuir três valores a cada ideia. Sean Ellis inventou ICE usando 'ease' em vez de 'effort'."
- "O que acontece é que as pessoas tendem a ir com instinto e então dar a si mesmas alta confiança. Encontrei isso perturbador porque subverte o sistema inteiro."
- "A métrica não é quão rápido conseguimos colocar os bits em produção... É sobre chegar aos bits certos em produção. É sobre time to outcomes."
> 🎧 [Becoming evidence-guided (0:34:48)](https://www.youtube.com/watch?v=aJWSn-tz3jQ)

## Conceitos relacionados
[[GIST — Camadas do Desenvolvimento de Produto]] · [[Evidence-Guided vs. Opinion-Based]] · [[Outcome Roadmap vs. Release Roadmap]] · [[Framework 4BB]] · [[Tudo no backlog é uma aposta]]
