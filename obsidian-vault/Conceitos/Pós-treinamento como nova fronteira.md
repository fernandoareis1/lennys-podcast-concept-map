---
tipo: insight
nivel: 3
fluxo: Estratégia & Visão
autores: [Asha Sharma]
---
# Pós-treinamento como nova fronteira
**Fluxo:** [[02 - Estratégia & Visão]] · **Tema:** [[Estratégia — Estratégia de produto]] · **Camada:** L3
**Tipo:** Insight · **Fontes:** [[Asha Sharma]]

## Ideia central
O pré-treinamento (treinar modelos do zero com bilhões de tokens e enormes investimentos de CapEx) está atingindo seus limites de retorno econômico. Um estudo de Nathan Lambert mostrando líderes em benchmarks revelou que acima de 30 bilhões de parâmetros, o custo de mais pré-treinamento raramente justifica o benefício marginal. A fronteira competitiva está se deslocando para o **pós-treinamento**: fine-tuning com dados proprietários, reinforcement learning (RL) com rewards personalizados, e otimização contínua do modelo para casos de uso específicos. 

Empresas que adotam essa abordagem constroem um moat que modelos base — mesmo os mais poderosos — não conseguem replicar: o **IP está no loop, nos dados proprietários e no design de rewards**, não no modelo em si. Em 2025, ~50% dos desenvolvedores já fazem fine-tuning. A previsão é que investimento em pós-treinamento ultrapasse pré-treinamento em breve.

## Como aplicar
1. **Não invista em pré-treinamento próprio**: a menos que você seja OpenAI, Google ou Anthropic, o ROI não fecha. Use modelos de base de terceiros (ou open source de 30B+ parâmetros) como ponto de partida.
2. **Identifique o job to be done mais nítido**: pós-treinamento funciona melhor quando você tem um caso de uso específico com sinal claro de qualidade (ex: "aceitar ou não a sugestão de código", "classificar corretamente um diagnóstico").
3. **Desenhe o loop de rewards antes de coletar dados**: o que define uma "boa" resposta do modelo? Quem avalia? Como é automatizado? Rewards design is product design.
4. **Monte o flywheel de dados**: dados reais de usuários > dados sintéticos > dados comprados. Mas dados sintéticos são legítimos quando dados reais são escassos ou caros de anotar.
5. **Pense como portfólio de modelos, não um único modelo**: diferentes tasks têm diferentes tradeoffs (latência vs. capacidade, custo vs. qualidade). Ensemble de modelos especializados por fine-tuning é superior a um único modelo generalista off-the-shelf.
6. **Meça e A/B teste agressivamente**: fine-tuning sem medição rigorosa é desperdício. Configure evals antes de começar o pós-treinamento.

## Insights por autor
### [[Asha Sharma]]
- "Acredito que veremos tanto dinheiro gasto em pós-treinamento quanto em pré-treinamento — e no futuro, mais em pós-treinamento."
- "Você obtém mais alavancagem economicamente e mais alavancagem do ponto de vista de customização se você está fazendo reinforcement learning ou algum tipo de fine-tuning para otimizar o que está off-the-shelf para algum resultado como preço, performance, qualidade."
- Dragon AI (médicos): de 30-60% para 83% de aceitação de sugestões após anotar 600k interações paciente-médico por especialistas e usar no fine-tuning.
- "50% dos desenvolvedores, de acordo com pesquisas, agora estão fazendo fine-tuning. E sabemos que fine-tuning é bom, mas se você realmente passar pelo loop completo, pode obter resultados melhores."
- "Muito mais no campo de sistema de modelos. Acredito em diversidade de modelos. Claude Sonnet 4 é incrível para um conjunto de casos de uso versus GPT-5 é diferente para outros. Alguns você se importa com a latência, outros quer raciocínio mais lento."
> 🎧 [How 80,000 companies build with AI: Products as organisms and the death of org charts (57:11)](https://www.youtube.com/watch?v=J9UWaltU-7Q) · 2025-08-28

## Conceitos relacionados
[[Produto como organismo]] · [[O loop e não o lane]] · [[Non-determinismo em Produtos de IA]] · [[Dois de três pontos de inflexão]]
