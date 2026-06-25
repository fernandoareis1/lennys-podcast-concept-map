---
tipo: framework
nivel: 3
fluxo: Experimentação & Dados
autores: [Hamel Husain, Shreya Shankar]
---
# Evals para Produtos de IA
**Fluxo:** [[05 - Experimentação & Dados]] · **Tema:** [[Experimentação — AB testing & cultura]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Hamel Husain]] · [[Shreya Shankar]]

## Ideia central
Evals são o conjunto de técnicas para medir e melhorar sistematicamente aplicações de IA. Não se trata de testes de software comuns: o espaço de saídas é estocástico e aberto, então o objetivo principal é criar um **ciclo de feedback confiável** — ir dos "vibe checks" subjetivos para métricas acionáveis que permitem iterar com confiança. É descrito como a atividade de maior ROI para qualquer builder de produto de IA.

## Como aplicar
1. Comece com **vibe checks** (inspecionar saídas manualmente) — são válidos no início, mas não escalam.
2. Faça **Error Analysis**: inspecione traces reais, anote falhas em linguagem natural (open coding), agrupe em categorias (axial coding) e conte frequências.
3. Defina **avaliadores automatizados**: code-based para verificações objetivas (formato, JSON, presença de texto) ou LLM-as-judge para falhas subjetivas e complexas.
4. Valide o avaliador contra julgamento humano antes de confiar nele — "LLM que concorda com você X% das vezes" é o critério de qualidade do juiz.
5. Rode evals **em pré-produção** (CI) e **em produção** (monitoramento contínuo por amostragem).

## Insights por autor
### [[Hamel Husain]] e [[Shreya Shankar]]
- "Evals é, na sua essência, analytics de dados sobre sua aplicação LLM e uma forma sistemática de olhar para esses dados."
- O erro mais comum: pular direto para escrever testes antes de entender os dados. "Isso é onde as coisas desandam."
- O objetivo não é perfeição: "O objetivo não é fazer evals perfeitamente, é melhorar seu produto de forma acionável."
- Evals não são só testes de CI — podem monitorar 1.000 traces em produção por dia, dando medida de qualidade em tempo real.
> 🎧 [Why AI evals are the hottest new skill for product builders (1:46:33)](https://www.youtube.com/watch?v=BsWxPI9UM4c)

## Conceitos relacionados
[[Error Analysis — Open e Axial Coding]] · [[LLM como Juiz]] · [[CC-CD — Calibração Contínua, Desenvolvimento Contínuo]] · [[A-B Testing (Ronny Kohavi)]] · [[Falha Conclusiva — Design de Experimento Definitivo]]
