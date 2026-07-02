---
tipo: tecnica
nivel: 3
fluxo: Experimentação & Dados
autores: [Nicole Forsgren]
---
# Survey de Barreiras — Diagnóstico Rápido de DevEx

**Fluxo:** [[05 - Experimentação & Dados]] · **Tema:** [[Experimentação — Aprender com pouco e qualitativo]] · **Camada:** L3
**Tipo:** Técnica · **Fontes:** [[Nicole Forsgren]]

## Ideia central
Quando não há instrumentação de dados ou quando as métricas existentes não foram projetadas com propósito claro, o caminho mais rápido para entender os maiores problemas do time de engenharia é um **survey estruturado de barreiras**.

Formato recomendado:
1. "Escolha as **3 maiores barreiras** para sua produtividade" (de uma lista de ferramentas e processos; fazer escolher 3 evita que tudo seja marcado como importante)
2. "Com que frequência cada uma te afeta?" (horária / diária / semanal / trimestral)
3. Campo aberto: "Tem algo mais que deveríamos saber?"

O resultado: um score ponderado por frequência que revela claramente onde focar o trabalho de DevEx. Simples de criar, simples de interpretar, acionável em dias.

**Por que satisfação, não felicidade:**
Não meça "quão feliz você está" — felicidade é influenciada por demais variáveis externas ao trabalho. Meça **satisfação com ferramentas e processos específicos**: é uma resposta mais direta, mais acionável e menos ruidosa.

## Como aplicar
1. **Crie a lista de barreiras candidatas** com os engenheiros (brainstorm inicial ou baseado em observação direta).
2. **Limite a 3 escolhas por respondente** — isso força priorização real.
3. **Adicione a dimensão de frequência** (horária, diária, semanal, trimestral) para identificar o que é doloroso E frequente.
4. **Calcule score ponderado:** barreira × frequência = ranking de prioridade.
5. **Itere:** refaça o survey a cada ciclo de melhoria para medir se a barreira foi removida.
6. **Use como baseline:** mesmo um baseline subjetivo é melhor que nenhum baseline. Ele orienta as próximas ações e serve como ponto de comparação.

## Insights por autor
### [[Nicole Forsgren]]
- "If you're just starting, I would do surveys because surveys can give you a nice overall view of the landscape quickly so that you know where the big challenges are."
- "By making folks prioritize the top three things — let them pick everything, it makes the data super, super messy. But three things and how often, you can just come up with a score or a weighted score."
- Satisfação vs. felicidade: "There are too many things that contribute to happiness... What can be helpful is satisfaction. You can ask 'Are you satisfied with this tool?' and ask follow-up questions."
- "Happy devs make happy code. They write better programs, they do better work, they're better team members and collaborators."
> 🎧 [How to measure AI developer productivity in 2025 (1:07:48)](https://www.youtube.com/watch?v=SWcDfPVTizQ)

## Conceitos relacionados
[[Três Pilares do DevEx — Flow, Carga Cognitiva e Feedback Loops]] · [[7 Passos para Time de Developer Experience]] · [[Métricas Simples vs Compostas — Clareza Bate Perfeição]] · [[Experimentação — Aprender com pouco e qualitativo]]
