---
tipo: framework
nivel: 3
fluxo: Estratégia & Visão
autores: [Peter Deng]
---
# Ir Devagar para Ir Rápido — Sistemas na Fase 1→100

**Fluxo:** [[02 - Estratégia & Visão]] · **Tema:** [[Estratégia — Estratégia de produto]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Peter Deng]]

## Ideia central
A fase 0→1 é sobre encontrar PMF. A fase 1→100 é sobre hipercrescimento sustentável — e aqui o erro fatal é continuar operando no modo "move fast and break things". Quando o foguete decola, você sente as G-forces. Quem já viveu isso sabe: é diferente de voar em altitude de cruzeiro. O princípio central de Peter Deng é que nessa fase você precisa ir devagar para ir rápido — construir as abstrações certas, a arquitetura certa, os sistemas certos. Exemplos reais: o sharing loop do Newsfeed, o sistema de venues do Uber para pickups em qualquer lugar do mundo, a infraestrutura de push do Messenger. Esses sistemas são o motivo pelo qual esses produtos ainda funcionam décadas depois.

## Como aplicar
1. Na fase 1→10, adote uma abordagem de portfólio: não é binário "construir sistemas vs. mover rápido" — é quanto do seu tempo está em cada um, e esse percentual vai aumentando à medida que você escala.
2. Identifique as abstrações-chave do seu produto: o que representa o conceito mais fundamental (o "venues" do Uber, o "sharing loop" do Newsfeed)? Acertar essa abstração cria durabilidade.
3. Quando um sistema começa a virar "spaghetti", é sinal de que você pulou a fase de abstração. Uber rider app em certo ponto precisou ser re-arquitetado — custoso mas necessário.
4. G-forces de hipercrescimento comprimem tempo de decisão. Você não pode pensar claramente durante a decolagem — pense antes. Planeje os movimentos de xadrez antecipadamente.
5. "Go slow to go fast" não é permissão para nunca lançar. É sobre qual fração do tempo você dedica a construir certo vs. construir rápido.

## Insights por autor
### [[Peter Deng]]
- "Quando você está em hipercrescimento, sente as G-forces. Pilotar a 35.000 pés é diferente de decolar num foguete."
- Newsfeed: arquitetura do sharing loop pensada meticulosamente → produto que não mudou substancialmente em 12 anos.
- Messenger: 0 → 4,7 bilhões de mensagens por dia em dois anos e meio. Forethought em infraestrutura foi o que viabilizou isso.
- Uber venues: sistema interno de pickup/dropoff em venues, mundialmente configurável → habilitou escala global de forma sustentável.
- Não é uma mudança binária de estado. É uma ramp rate — crescente ao longo do tempo conforme você vai da fase 1→5 para 5→10 para 10→100.

## Conceitos relacionados
[[Equipe de Growth como Mecanismo de Diagnóstico]] · [[Sistemas, não Metas]] · [[Riding the Lightning]] · [[Fast Thinking vs. Slow Thinking — Dois Grupos de Produto]]
