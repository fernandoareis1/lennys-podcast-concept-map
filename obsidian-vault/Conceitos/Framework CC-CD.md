---
tipo: framework
nivel: 3
fluxo: Experimentação & Dados
autores: [Aishwarya Naresh Reganti, Kiriti Badam]
---
# Framework CC/CD
**Fluxo:** [[05 - Experimentação & Dados]] · **Tema:** [[Experimentação — Aprender com pouco e qualitativo]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Aishwarya Naresh Reganti]] · [[Kiriti Badam]]

## Ideia central
**Continuous Calibration / Continuous Development** — um flywheel para construir produtos de IA de forma iterativa sem perder confiança do cliente. O lado direito do loop (**desenvolvimento contínuo**) cria e expande capacidades; o lado esquerdo (**calibração contínua**) monitora em produção e alimenta o ciclo com dados reais. Os dois juntos criam um sistema auto-melhorável.

## Como aplicar
**Loop de Desenvolvimento Contínuo (direita):**
1. **Escopo de capacidade** — defina o que o sistema *deve* e *não deve* fazer. Líderes e PMs geralmente descobrem aqui que o time não está alinhado.
2. **Curadoria de dados** — monte um dataset representativo de inputs esperados e outputs desejados. Pequeno, mas honesto.
3. **Evals** — não são cura-tudo; são *dimensões de avaliação* (métricas) que você mede continuamente, não só antes do lançamento.
4. **Deploy** — com guarda-rails: humanos no loop onde o risco é alto; monitoramento de anomalias ativo.

**Loop de Calibração Contínua (esquerda):**
5. **Monitoramento em produção** — capture feedback real, incluindo casos-borda emergentes que nenhum eval previu.
6. **Triagem rápida de incidentes** — hotfixes só quando inevitável; o objetivo é reduzir surpresas, não aumentar patches.
7. **Alimentar o loop** — os dados de produção entram como novos exemplos no dataset de curadoria → ciclo recomeça.

## Insights por autor
### [[Aishwarya Naresh Reganti]]
- "Evals não são um cure-all. Muitas pessoas confundem avaliação (processo) com métricas de avaliação (dimensões). Você precisa dos dois."
- "Se você não tem as métricas de avaliação certas, você voa cego em produção."
- Tiveram de fechar um produto em produção porque os hot-fixes não acompanhavam os problemas emergentes — motivação central do CC/CD.

### [[Kiriti Badam]]
- "O objetivo não é ser a primeira empresa a ter um agente. É ter construído os flywheels certos para melhorar ao longo do tempo."
- Equipe do Codex na OpenAI: combina evals clássicos com monitoramento constante do Reddit ("lá tem elogio e tem reclamação — os dois são úteis").

> 🎧 [Why most AI products fail: Lessons from 50+ deployments (1:26:22)](https://www.youtube.com/watch?v=z7T1pCxgvlA)

## Conceitos relacionados
[[Dois pilares do produto de IA]] · [[Assumption Testing]] · [[Decidir com poucos dados é melhor que com zero]] · [[Humans in the Loop (algoritmos)]]
