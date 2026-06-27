---
tipo: framework
nivel: 3
fluxo: Experimentação & Dados
autores: [Jeff Weinstein]
---
# Métrica do Cliente — Medir do Ponto de Vista do Comprador

**Fluxo:** [[05 - Experimentação & Dados]] · **Tema:** [[Experimentação — AB testing & cultura]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Jeff Weinstein]]

## Ideia central
A responsabilidade do PM é produzir product-market fit — e métricas são a representação numérica do valor que você entrega ao cliente. O erro mais comum é medir eventos internos (logins, eventos técnicos) em vez de medir se o cliente conseguiu o que veio fazer. No Stripe Atlas: a métrica escolhida foi "founders com zero tickets de suporte durante todo o processo de incorporação" — não a média de tickets, não o NPS, mas a porcentagem de founders que passaram sem nenhum atrito. Em 18 meses, o número foi de 15% para 85%. A regra: se você vazasse seu dashboard para o cliente e ele ficasse feliz em ver o que você está medindo, você escolheu a métrica certa. Métricas são também um mecanismo de alinhamento — escolher uma métrica principal força o time a se perguntar o que o cliente realmente quer, não o que é mais fácil de medir.

## Como aplicar
1. Pergunte: "Por que alguém recomendaria nosso produto para um amigo?" — a resposta define o que medir.
2. Meça do ponto de vista do cliente, não da engenharia (zero suporte > média de tickets; tarefa concluída > login).
3. Escolha uma métrica principal que todos entendam sem explicação. Adicione métricas táticas específicas por iniciativa — mas otimize ao redor da principal.
4. Dê um título que faça sentir alguma coisa: "Companies with Zero Support" em vez de "p_support_ticket_count_min_0".
5. Mantenha a métrica num lugar fixo e público (Go Metrics no Stripe). Olhe todo dia. Só mude quando a definição tiver sido testada por semanas.
6. Crie um "bad day chart": emita um log-line sempre que o usuário bateu num problema (404, payout atrasado, declínio em excesso). Visualize como barras empilhadas e escolha quais bad days queimar primeiro.

## Insights por autor
### [[Jeff Weinstein]]
- "Se você vazasse seu dashboard para o cliente e ele ficasse animado em ver que é isso que você está medindo o tempo todo, você achou a métrica certa."
- Atlas: 15% → 85% de founders com zero tickets de suporte; a curva de market share no mesmo período tem o mesmo formato.
- "Métricas são como um contador de batimentos cardíacos do cliente. Se o time todo acorda e olha para a mesma coisa todo dia, isso é muito mais poderoso do que decidir o que fazer do zero a cada mês."
- Bad day chart: "Qualquer ideia de por que o cliente está tendo um dia ruim — coloca um log-line. Visualiza como barras. Escolhe quais queimar."
> 🎧 [Building product at Stripe: craft, metrics, and customer obsession | Jeff Weinstein (2:35:00)](https://www.youtube.com/watch?v=qbZQjprTnrU)

## Conceitos relacionados
[[Study Group — Empatia pelo Cliente em Grupo]] · [[Produto-Market Fit como Missão do PM]] · [[Demand Side Sales]]

