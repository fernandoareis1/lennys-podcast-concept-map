---
tipo: conceito
nivel: 3
fluxo: Experimentação & Dados
autores: [Lauryn Isford]
---
# Experimentação Como Mitigação de Risco — Quando Não Testar

**Fluxo:** [[05 - Experimentação & Dados]] · **Tema:** [[Experimentação — AB testing & cultura]] · **Camada:** L3
**Tipo:** Conceito · **Fontes:** [[Lauryn Isford]]

## Ideia central
Experimentar tem dois propósitos legítimos: (1) medir impacto com precisão e (2) mitigar risco de mudanças dramáticas. O problema é que muitas equipes de growth experimentam por padrão — como reflexo cultural — mesmo quando nenhum dos dois propósitos é verdadeiro. A/B testing é caro: engenheiros, analistas e PMs gastam tempo desenhando, analisando e interpretando experimentos que poderiam ter sido simplesnente shippados com convicção. A alternativa é **confiar no processo de produto** — mais tempo com clientes, mais rigor na definição do problema, mocks em frente a usuários — e reservar experimentos para mudanças dramaticas com risco real.

**Quando experimentar é necessário:**
- Mudanças dramáticas onde existe risco real de impacto negativo
- Quando a precisão métrica importa genuinamente para a decisão (não apenas para o review de desempenho)
- Quando não existe outra forma de isolar o efeito

**Quando experimentar é desperdício:**
- Variações incrementais onde a direção do impacto é óbvia
- Quando o custo de espera > custo do risco
- Quando a precisão de "6% vs. 7% de ativação" não muda nenhuma decisão real
- Quando o rigor vem do medo de errar, não da necessidade do dado

**Como sair da armadilha do "experimento tudo":**
- Construir cultura de resultados orientada ao cliente, não a pontos percentuais de teste
- Métricas de impacto alternativas: feedback qualitativo, deals fechados, deals não perdidos
- Especialmente em engenharia de growth: não exigir que todo impacto venha de um número de experimento
- Após o ship, usar atribuição e análise pós-lançamento para aprender o que aconteceu

**O caso Airtable Forms:**
- Feature de "cópia da submissão por email" foi lançada sem A/B test
- Razão: rigor de produto (pesquisa qualitativa + análise de dados) deu convicção suficiente
- Resultado: impacto visível no top-line sem precisar do experimento para enxergar
- Aprendizado pós-launch via atribuição foi suficiente para extrair insights

## Como aplicar
1. Antes de desenhar um experimento, pergunte: "Se soubermos que isso moveu 6% em vez de 7%, isso muda alguma decisão?" Se não, não experimente
2. Invista o tempo economizado de não-experimentar em mais sessões com clientes, mais mocks testados qualitativamente, e mais rigor na definição do problema
3. Crie métricas de impacto alternativas para o time de engenharia: tickets de suporte, NPS, deals não perdidos — que não dependem de um número de A/B test
4. Reserve A/B tests para mudanças com risco real: redesigns completos, mudanças de preço, alterações de fluxo crítico
5. Para estabelecer essa cultura: ela precisa vir de cima — o head de growth tem que explicitamente validar trabalhos de alto impacto que não tiveram experimento formal

## Insights por autor
### [[Lauryn Isford]]
- "Sometimes you don't need to experiment. Sometimes if the business, activation rates go up 6% versus 7%, that precision actually doesn't help all that much beyond being able to say in your performance review, 'Hey, I increased activation by 7%'"
- "Experiments can be expensive"
- "Spend more time with customers, be more rigorous in understanding precisely what problem you're solving, get mocks in front of people and see how they react"
- "A results-oriented organization that just wants to do the right thing and move with urgency — that's the way that you can have the most impact"
- Caso Forms: "We just turned it on and wanted to see what would happen because we knew from rigor of a wonderful product team doing robust customer analysis and also doing the data work that this is something that people wanted"

> 🎧 [Lauryn Isford — Mastering onboarding](https://www.youtube.com/watch?v=dLku0AiGPVA)

## Conceitos relacionados
[[Taxa de Fracasso de 80% — A Realidade da Experimentação]] · [[Cultura de experimentação a 1000 por ano]] · [[Métricas de Guardrail — North Star com Contrapeso]] · [[A maioria das ideias falha no teste]]
