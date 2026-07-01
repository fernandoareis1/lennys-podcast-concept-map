---
tipo: modelo-mental
nivel: 3
fluxo: Experimentação & Dados
autores: [Nicole Forsgren]
---
# Curva J de DevEx — Ganhos que Compõem Após o Vale
**Fluxo:** [[05 - Experimentação & Dados]] · **Tema:** [[Experimentação — AB testing & cultura]] · **Camada:** L3
**Tipo:** Modelo mental · **Fonte:** [[Nicole Forsgren]]

## Ideia central
Investimentos em Developer Experience (DevEx) seguem uma curva J: os primeiros ganhos são rápidos e visíveis (quick wins), depois vem um vale onde os ganhos fáceis se esgotam e o trabalho fica mais difícil e mais lento de mostrar valor — e então, se você persiste, os retornos se compõem.

A curva J explica por que programas de DevEx morrem: quando o time chega no vale (fase 2), liderança conclui que "não está funcionando" e corta o investimento — justo antes dos ganhos compostos se materializarem.

**A lógica do composto:**
- Fase 1 (quick wins): resolver os problemas mais óbvios. Alta visibilidade, feedback imediato, constrói credibilidade.
- Fase 2 (vale): os problemas restantes são mais profundos, sistêmicos, sem ROI óbvio de curto prazo. Times que não entendem a curva J percebem isso como fracasso.
- Fase 3 (composto): cada melhoria de infraestrutura habilita as próximas. Tempo salvo em CI barateia experimentos. Observabilidade melhor encurta loops de debug. Os ganhos se multiplicam.

**Business value concreto:**
- Empresas pequenas (50-200 devs): centenas de milhares de dólares de economia por ano em tempo de engenharia
- Empresas médias (500+ devs): dezenas de milhões
- Grandes empresas (10k+ devs): bilhões — não é exagero; 10k devs × 1h/dia perdida = 10k horas/dia, 2.5 milhões de horas/ano

**O papel dos quick wins:**
Quick wins não são o objetivo — são o combustível. Eles sustentam o programa durante o vale. Sem quick wins visíveis nos primeiros 60-90 dias, o programa não sobrevive até a fase de composto.

## Como aplicar
1. **Comunique a curva J** antes de começar: diga explicitamente que vai haver um vale entre os quick wins e os ganhos compostos
2. **Planeje os quick wins** para os primeiros 30-60 dias — não escolha o mais impactante, escolha o mais visível
3. **Instrumente o vale**: durante a fase 2, meça métricas de leading indicator (tempo de onboarding, taxa de adoção de ferramentas) não só de output
4. **Crie checkpoints de 90 dias** com a liderança para mostrar progresso de leading indicators mesmo sem o composto visível ainda
5. **Calcule o business value antes**: com dados de tempo de engenharia, estime o ROI esperado na fase 3; ancore a conversa com liderança nesse número

## Insights por autor
### [[Nicole Forsgren]]
- "Quick wins sustain you, but the real value is in the J-curve compounding."
- "Most DevEx programs die in the valley. They mistake phase 2 for failure."
- "For large companies with thousands of engineers, the business value of DevEx is in the billions. That's not hyperbole — that's arithmetic."
- "You need quick wins not because they're the goal, but because they buy you time to get to the compound returns."

## Conceitos relacionados
[[DevEx como Produto — PM Mindset para Developer Experience]] · [[Métricas de Produtividade na Era da IA — SPACE vs Prescrição]] · [[Holdout de longo prazo]] · [[Lead Bullets vs Cannonballs]]
