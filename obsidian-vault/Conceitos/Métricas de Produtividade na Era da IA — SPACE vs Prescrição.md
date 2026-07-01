---
tipo: framework
nivel: 3
fluxo: Experimentação & Dados
autores: [Nicole Forsgren]
---
# Métricas de Produtividade na Era da IA — SPACE vs Prescrição
**Fluxo:** [[05 - Experimentação & Dados]] · **Tema:** [[Experimentação — AB testing & cultura]] · **Camada:** L3
**Tipo:** Framework · **Fonte:** [[Nicole Forsgren]]

## Ideia central
A maioria das métricas de produtividade de engenharia é uma mentira — e com IA isso ficou ainda pior. Linhas de código, que já eram gameable, tornaram-se trivialmente manipuláveis. O erro fundamental é usar métricas prescritivas (como as 4 métricas DORA) de forma imprecisa, ou criar proxies fracos que medem atividade em vez de impacto.

**DORA vs. SPACE:**
- **DORA** (Deployment Frequency, Lead Time, MTTR, Change Failure Rate): framework prescritivo — funciona exatamente como descrito ou não funciona. Não faça riffs em cima. As 4 métricas foram derivadas empiricamente de dados de milhares de times e a relação causal entre elas foi validada; mexa em uma e você quebra a lógica.
- **SPACE** (Satisfaction, Performance, Activity, Communication/Collaboration, Efficiency/Flow): framework *adaptável* — projetado para ser customizado ao contexto de cada time e empresa. Não prescritivo.

**Por que SPACE se encaixa melhor na era da IA:**
IA introduz não-determinismo fundamental. O mesmo prompt pode gerar outputs diferentes. Isso exige uma dimensão ausente nas métricas tradicionais: **Confiança (Trust)**. Times que adotam IA precisam medir se os engenheiros confiam nos outputs, se os loops de feedback são confiáveis e se o sistema age de acordo com o esperado. Trust é a nova variável de calibração.

**O problema das métricas de atividade:**
- Linhas de código: gameable, não mede valor
- PRs por semana: incentiva PRs pequenos e triviais
- Número de commits: idem
- Velocidade de sprint: local, não reflete impacto sistêmico

A pergunta certa não é "quanto o time produziu?" mas "qual foi o impacto do que foi produzido?"

## Como aplicar
1. **Audite suas métricas atuais**: identifique quais são de atividade vs. impacto; descarte as de atividade puras
2. **Se usar DORA, use exatamente como prescrito**: não substitua deployment frequency por "feature releases", não meça lead time de uma forma conveniente
3. **Construa seu SPACE customizado**: escolha 1-2 dimensões por categoria; não meça tudo — meça o que você vai agir
4. **Adicione Trust para times de IA**: pesquisa de satisfação com outputs de IA + taxa de aceitação de sugestões vs. taxa de edição pós-aceitação
5. **Use satisfação, não felicidade**: "você está satisfeito com seu ambiente de desenvolvimento?" captura algo acionável; "você está feliz?" não captura

## Insights por autor
### [[Nicole Forsgren]]
- "Lines of code became even more gameable with AI. We need to be way more thoughtful about what we measure."
- "DORA is prescriptive. Don't riff on it. SPACE is designed to be adapted."
- "Trust is the new dimension we need to add to SPACE in the AI era — LLMs are non-deterministic by design."
- "Satisfaction surveys are more actionable than happiness surveys for DevEx measurement."
- "Productivity metrics are often a lie. The question is whether they're a useful lie."

## Conceitos relacionados
[[DevEx como Produto — PM Mindset para Developer Experience]] · [[Curva J de DevEx — Ganhos que Compõem Após o Vale]] · [[Flow State com IA — Blocos de 45 Minutos]] · [[Métricas Simples vs Compostas — Clareza Bate Perfeição]] · [[Experimentação como Disciplina Científica]]
