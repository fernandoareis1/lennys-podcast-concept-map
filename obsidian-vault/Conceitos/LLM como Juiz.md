---
tipo: tecnica
nivel: 3
fluxo: Experimentação & Dados
autores: [Hamel Husain, Shreya Shankar]
---
# LLM como Juiz
**Fluxo:** [[05 - Experimentação & Dados]] · **Tema:** [[Experimentação — AB testing & cultura]] · **Camada:** L3
**Tipo:** Técnica · **Fontes:** [[Hamel Husain]] · [[Shreya Shankar]]

## Ideia central
Usar um LLM como avaliador automatizado de outro LLM — especificamente para modos de falha subjetivos e complexos que não podem ser capturados por código. O ponto crítico: o juiz deve avaliar **um único modo de falha por vez** e deve retornar um valor **binário (passou/falhou)**. Escores como "3,2 de 5" são não-acionáveis e não devem ser usados. Antes de confiar em qualquer juiz-LLM, valide sua concordância com julgamento humano.

## Como aplicar
1. Identifique o modo de falha específico que você quer medir (ex: "não fez handoff para humano quando deveria").
2. Escreva um prompt de juiz que descreva **exatamente** quando o comportamento é aceitável ou não — seja específico e baseado em exemplos reais.
3. Defina saída **binária**: `true` (erro presente) ou `false` (sem erro). Nada de escalas Likert.
4. **Valide o juiz**: pegue as traces que você já analisou manualmente (open codes/axial codes) e meça a taxa de concordância entre o juiz-LLM e sua própria avaliação.
5. Use o juiz em **CI pré-produção** (bloqueia releases com taxa de falha alta) e em **monitoramento contínuo** (amostragem de produção).
6. Adicione sempre a categoria "nenhuma das anteriores" no prompt do juiz para detectar lacunas no seu sistema de categorias.

## Insights por autor
### [[Hamel Husain]] e [[Shreya Shankar]]
- "Quando as pessoas perdem confiança nas suas evals, elas perdem confiança em você."
- O maior erro: usar score de 1 a 5 em vez de binário. "3,2 versus 3,7 — ninguém sabe o que isso significa."
- "O escopo do problema é muito pequeno [para o juiz-LLM]. É fazer uma coisa: avaliar um modo de falha específico. O output é passa ou falha. O LLM é muito capaz de fazer isso de forma confiável."
- Mesmo para evals subjetivas, o juiz-LLM tende a ser mais confiável do que você esperaria — porque o escopo é pequeno.
> 🎧 [Why AI evals are the hottest new skill for product builders (1:46:33)](https://www.youtube.com/watch?v=BsWxPI9UM4c)

## Conceitos relacionados
[[Evals para Produtos de IA]] · [[Error Analysis — Open e Axial Coding]] · [[Humans in the Loop (algoritmos)]] · [[CC-CD — Calibração Contínua, Desenvolvimento Contínuo]]
