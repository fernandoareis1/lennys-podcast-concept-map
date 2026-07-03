---
tipo: tema
nivel: 2
fluxo: Experimentação & Dados
---
# 🧪 Tema · A/B testing & cultura

**Fluxo:** [[05 - Experimentação & Dados]] · **Camada:** L2 (Tema)

A disciplina de testar com **rigor e humildade**: a métrica certa, o ceticismo com resultados bons demais, e a memória institucional que faz o aprendizado se acumular.

## Conceitos (L3)
- [[A-B Testing (Ronny Kohavi)]] — teste tudo, portfólio de apostas · **⬇ tem aprofundamento**
- [[OEC - Overall Evaluation Criterion]] — a métrica única + guardrails
- [[Twyman's Law]] — dado bom demais provavelmente está errado
- [[A maioria das ideias falha no teste]] — 66–92% das ideias não movem a métrica
- [[Lead Bullets vs Cannonballs]] — portfólio de apostas: pequenas + grandes mudanças fundamentais
- [[Humans in the Loop (algoritmos)]] — PMs definem o que algoritmo decide vs. o que humano decide
- [[Cultura de experimentação a 1000 por ano]] — meta ambiciosa como forcing function para construir capacidade de experimentação
- [[Métricas absolutas vs. taxas de conversão]] — times otimizando taxas locais criam incentivo perverso de restringir o funil acima; use números absolutos
- [[Holdout de longo prazo]] — manter cohort de controle e revisitar experimentos em 3/6/9/12 meses; 30-40% dos winners não têm lift de longo prazo
- [[Experimentação com amostras pequenas]] — quando A/B não é viável (baixo volume): power analysis primeiro; cidades-gêmeas; diff-in-diff; 80% de confiança; e quando nada funciona, ship na intuição + loop de feedback pós-lançamento
- [[LLM como Juiz — avaliação automatizada de qualidade]] — eval binário (pass/fail) para um único modo de falha em apps de IA; uso em CI e monitoramento online
- [[Métrica do Cliente — Medir do Ponto de Vista do Comprador]] — meça se o cliente conseguiu o que veio fazer (zero tickets de suporte vs. média de tickets); se o cliente ficasse animado ao ver seu dashboard, você escolheu a métrica certa; bad day chart como background noise
- [[Métricas de Proxy para Outcomes de Longo Prazo]] — encontre métrica de curto prazo que prediz o outcome de longo prazo; retenção não é meta operacional
- [[Métricas Simples vs Compostas — Clareza Bate Perfeição]] — métrica simples que todos entendem > composta perfeita que ninguém debate
- [[Fail States como Métricas Obrigatórias]] — medir e zerar experiências catastróficas (Never Delivered) tem impacto desproporcional no churn vs. melhorar a média
- [[Atrito Estratégico — Friction para Reduzir Comportamentos]] — para reduzir comportamento indesejado, adicione atrito mínimo; TikTok label+"Tem certeza?" = -24% desinformação; delay de 16s no elevador → pessoas usam escadas
- [[Taxa de Fracasso de 80% — A Realidade da Experimentação]] — Netflix/Microsoft: 80-90% dos experimentos falham; iterativo sempre vence big redesign; hierarquia de validação: painted door → mock → MVP vergonhoso → A/B; failure é compass, não parede
- [[Experimentação Como Mitigação de Risco — Quando Não Testar]] — A/B test tem dois propósitos legítimos: precisão e mitigação de risco; na ausência de ambos, confie no processo de produto; custo do experimento é real e frequentemente ignorado
- [[Experimentação como Disciplina Científica]] — estratégia é superestimada; a real estratégia do PM é "como rápido vou de hipótese a dado?"; cultura de experimentos elimina HiPPO e substitui opinião por evidência
- [[Métricas de Produto vs. Métricas de Negócio]] — ARR é métrica de negócio; ARR por segmento/produto/feature é métrica de produto; lentes de produto sobre métricas de negócio tornam estratégia de produto acionável
- [[Efeito de Rede por Design de Convites]] — conectores naturais convidam se o fluxo for simples; convites ubíquos e presentes em múltiplos pontos; usuários não-sociais ignoram, não sacrifique o design por eles
- [[Métricas Além de Engajamento — Saúde vs. Vício em IA]] — otimizar likabilidade em IA gera sycophancy; o critério correto é tempo bem gasto (usuário saiu mais capaz) vs. engajamento; "você sabe quando seu produto está realmente servindo as pessoas"

- [[Predição vs. Causalidade em Dados]] — ML prediz correlações, boas decisões precisam de causalidade; enviar promoções a alto LTV ≠ enviar a quem vai incrementar LTV por causa da promoção

## Descer mais (L4) ⬇
[[A-B Testing — Evidências (Ronny Kohavi)]]
