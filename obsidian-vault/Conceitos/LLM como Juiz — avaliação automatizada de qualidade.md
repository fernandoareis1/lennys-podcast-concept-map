---
tipo: tecnica
nivel: 3
fluxo: Experimentação & Dados
autores: [Hamel Husain, Shreya Shankar]
---
# LLM como Juiz — avaliação automatizada de qualidade
**Fluxo:** [[05 - Experimentação & Dados]] · **Tema:** [[Experimentação — AB testing & cultura]] · **Camada:** L3
**Tipo:** Técnica · **Fontes:** [[Hamel Husain]] · [[Shreya Shankar]]

## Ideia central
Após identificar um modo de falha específico via análise de erros, é possível usar um LLM como "juiz" para detectar automaticamente essa falha em escala — em unit tests, CI/CD e monitoramento de produção. A chave é escopo estreito e **output binário (pass/fail)**:

- O LLM juiz avalia **um único modo de falha** por vez, não a qualidade geral.
- A resposta deve ser binária: passou ou falhou. Escalas Likert (1–7) são anti-padrão — ninguém sabe o que 3.2 vs. 3.7 significa.
- Antes de usar o juiz em produção, **valide-o contra anotações humanas** usando uma matriz de confusão — não apenas "% de concordância" (métrica enganosa quando erros são raros).
- 4 a 7 juízes LLM costumam ser suficientes para cobrir os modos de falha relevantes de um produto.

## Como aplicar
1. Identifique um modo de falha prioritário via análise de erros (ex.: "agente não passou a chamada para humano quando deveria").
2. Escreva um prompt de juiz com critérios explícitos de quando o modo de falha ocorre, e instrua o LLM a responder true/false.
3. Valide o juiz: compare suas respostas com suas anotações manuais (axial codes) usando matriz de confusão — minimize os falsos positivos e falsos negativos.
4. Itere no prompt do juiz até que o alinhamento com o humano seja satisfatório.
5. Implante o juiz como: (a) teste automatizado pré-deploy, (b) monitoramento online amostrado (ex.: 1.000 traces/dia).

## Insights por autor
### [[Hamel Husain]]
- "Você não quer escrever um eval de escala de 1 a 5. Isso é uma forma covarde de não tomar uma decisão. Você precisa decidir: isso é bom o suficiente ou não?"
- Validar o juiz contra anotações humanas via matriz de confusão — apenas "% de concordância" é perigoso quando erros são raros (você pode ter 90% de concordância com um juiz que nunca detecta o erro).
- "Quando as pessoas perdem confiança nos seus evals, perdem confiança em você." — a validação do juiz é crítica para credibilidade.

> 🎧 [Why AI evals are the hottest new skill for product builders | Hamel Husain & Shreya Shankar (1:46:33)](https://www.youtube.com/watch?v=BsWxPI9UM4c) · 2025-09-25

### [[Shreya Shankar]]
- "O escopo do problema é muito pequeno — avaliar um único modo de falha — e o output é pass/fail. Isso é algo que LLMs conseguem fazer de forma muito confiável."
- O juiz pode ser usado tanto em unit tests/CI (pré-deploy) quanto em monitoramento online (produção amostrada). "Os produtos que fazem isso têm uma visão muito nítida de como sua aplicação está performando."
- Um erro comum: criar o prompt de juiz sem iterar. Sempre meça o alinhamento com o humano e reduza os erros nas diagonais não-verdes da matriz de confusão.

> 🎧 [Why AI evals are the hottest new skill for product builders | Hamel Husain & Shreya Shankar (1:46:33)](https://www.youtube.com/watch?v=BsWxPI9UM4c) · 2025-09-25

## Conceitos relacionados
[[Era dos evals — o eval é o PRD do modelo]] · [[Análise de erros qualitativa para produtos de IA]] · [[OEC - Overall Evaluation Criterion]] · [[A-B Testing (Ronny Kohavi)]] · [[Non-determinismo em Produtos de IA]]
