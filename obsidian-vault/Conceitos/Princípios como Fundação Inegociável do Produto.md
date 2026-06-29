---
tipo: mindset
nivel: 3
fluxo: Estratégia & Visão
autores: [Keith Coleman]
---
# Princípios como Fundação Inegociável do Produto

**Fluxo:** [[02 - Estratégia & Visão]] · **Tema:** [[Estratégia — Visão, missão & narrativa]] · **Camada:** L3
**Tipo:** Mindset · **Fontes:** [[Keith Coleman]]

## Ideia central
Produtos que precisam de confiança pública — especialmente em contextos de moderação, informação ou segurança — não podem ter sua arquitetura de confiança comprometida por conveniência operacional. Os princípios não são aspiração: são **restrições de design** que protegem a proposta de valor central.

No caso do Community Notes, os dois princípios fundadores pareciam "loucos" para muitos dentro da empresa:
1. **Voz do povo, não da empresa**: não existe botão que a empresa pode apertar para mudar o status de uma nota. Se um note aparece, é porque a comunidade decidiu. A empresa não tem override.
2. **Transparência total**: o código do algoritmo é open source, os dados de rating são publicados diariamente. Qualquer pessoa pode replicar o sistema e auditar o que a empresa fez.

Quebrar qualquer um desses princípios tornaria o produto impossível de confiar — e sem confiança, o Community Notes não funciona.

## Como aplicar
1. Antes de construir, articule os princípios que não podem ser violados sem destruir a proposta de valor central.
2. Para cada princípio, pergunte: "Se quebrássemos isso, o produto ainda valeria a pena existir?" Se a resposta for não, é um princípio real.
3. Quando alguém pressionar para fazer exceção ("e se for esse caso especial?"), volte ao princípio: "Se este caso é especial demais para o princípio funcionar, então o sistema está errado, não o princípio."
4. Transparência tem custo técnico real — arquitete desde o início pensando nela, não como afterthought.
5. "Even advertisers can get notes. We shouldn't exempt Elon." — consistência universal é o que dá credibilidade.

## Insights por autor
### [[Keith Coleman]]
- "If there's a problem with a note that's so bad, you want to do something about it's a problem with the system. We need to redesign the system to be showing good notes." — o princípio substitui controles manuais por rigor sistêmico.
- "People needed to get comfortable with this. They need to trust this. So the whole thing has to be out in the open." — transparência como requisito de confiança, não como virtude adicional.
- Jay Baxter: os princípios de transparência forçaram decisões arquiteturais difíceis (como treinar ML de forma replicável em script Python) que não teriam sido feitas por padrão.
- O Community Notes sobreviveu a 4 CEOs diferentes (Jack, Parag, e Elon como mais proeminentes) em parte porque os princípios eram claros demais para qualquer líder ignorar arbitrariamente.
- "We didn't have a button that will change the status of a note." — a restrição técnica é a garantia de confiança.

> 🎧 [An inside look at X's Community Notes | Keith Coleman & Jay Baxter (1:47:58)](https://www.youtube.com/watch?v=8dgyqYHLcCI)

## Conceitos relacionados
[[Estratégia — Visão, missão & narrativa]] · [[Transparência Radical como Vantagem Competitiva]] · [[Vacas Sagradas como Roadmap]] · [[Algoritmo de Bridging — Acordo entre Divergentes]]
