---
tipo: tecnica
nivel: 3
fluxo: Experimentação & Dados
autores: [Hamel Husain, Shreya Shankar]
---
# Análise de Erro com Open Coding
**Fluxo:** [[05 - Experimentação & Dados]] · **Tema:** [[Experimentação — Aprender com pouco e qualitativo]] · **Camada:** L3
**Tipo:** Técnica · **Fontes:** [[Hamel Husain]] · [[Shreya Shankar]]

## Ideia central
Antes de escrever qualquer eval automatizado, é preciso **olhar os dados manualmente**. O processo vem de métodos qualitativos das ciências sociais (open coding / axial coding) e tem três fases: (1) revisar traces individuais e anotar livremente o que está errado (*open codes*); (2) agrupar essas notas em categorias de falha acionáveis (*axial codes*) com ajuda de um LLM; (3) quantificar a prevalência de cada categoria para priorizar o que consertar.

Critério de parada: **saturação teórica** — continuar até não descobrir novos tipos de problema. Para a maioria dos produtos, isso acontece em 40–100 traces.

## Como aplicar
1. **Abra a ferramenta de observabilidade** (Braintrust, Phoenix Arize, LangSmith) e filtre traces recentes de produção.
2. **Leia cada trace e anote a primeira coisa errada** que você vê — a falha mais upstream. Use frases descritivas, não palavras genéricas como "janky".
3. **Pare quando atingir saturação teórica**: quando você deixar de descobrir novos tipos de problema.
4. **Use um LLM para criar axial codes**: cole os open codes num prompt e peça que o modelo agrupe em categorias de falha acionáveis. Revise e renomeie — prefira nomes específicos ("handoff sem confirmação") a genéricos ("problema de comunicação").
5. **Quantifique** a frequência de cada categoria com uma fórmula simples de planilha. Os mais frequentes são o que você deve atacar primeiro.

## Insights por autor
### [[Hamel Husain]]
- "Você aprende uma quantidade absurda quando faz isso. Toda pessoa que faz isso fica viciada imediatamente."
- "Escreva a primeira coisa errada que você vê — a falha mais upstream — e siga em frente. Não tente catalogar todos os erros."
- "Contagem básica é a técnica analítica mais poderosa em ciência de dados, porque é simples e acessível a todos."
> 🎧 [Why AI evals are the hottest new skill for product builders (1:46:33)](https://www.youtube.com/watch?v=BsWxPI9UM4c)

### [[Shreya Shankar]]
- "O objetivo não é fazer evals perfeitamente, é melhorar o produto de forma acionável."
- "Open coding, axial coding — esses termos vêm das ciências sociais. Não inventamos nada; só trouxemos para o contexto de LLMs."
- "Saturação teórica: quando você deixar de descobrir novos tipos de problema, é hora de parar."
> 🎧 [Why AI evals are the hottest new skill for product builders (1:46:33)](https://www.youtube.com/watch?v=BsWxPI9UM4c)

## Conceitos relacionados
[[Era dos evals — o eval é o PRD do modelo]] · [[LLM como Juiz — Avaliador Binário]] · [[Ditador Benevolente]] · [[Experimentação com amostras pequenas]]
