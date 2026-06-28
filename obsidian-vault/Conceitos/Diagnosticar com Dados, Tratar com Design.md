---
tipo: framework
nivel: 3
fluxo: Experimentação & Dados
autores: [Julie Zhuo]
---
# Diagnosticar com Dados, Tratar com Design
**Fluxo:** [[05 - Experimentação & Dados]] · **Tema:** [[Experimentação — Aprender com pouco e qualitativo]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Julie Zhuo]]

## Ideia central
"Diagnose with data and treat with design." — dados revelam o que está acontecendo e onde estão os problemas ou oportunidades; design inventa a solução. Os dois papéis são complementares, não concorrentes. Confundi-los leva a dois erros simétricos: (1) designer que rejeita dados por medo de perder criatividade; (2) analista que acha que os dados dirão o que construir.

Dados capturam realidade. Design cria realidade. Nenhum substitui o outro.

## O que os dados fazem (e não fazem)

**Fazem:**
- Revelam o que usuários realmente fazem, não o que você imagina que fazem
- Mostram onde existe um problema ou oportunidade (localizam o alvo)
- Questionam a narrativa interna ("nossa empresa é incrível, as pessoas nos amam")
- Ajudam a prever quando o crescimento vai desacelerar antes que isso aconteça
- Testam hipóteses específicas (não "a ideia", mas "essa suposição dentro da ideia")

**Não fazem:**
- Dizer qual feature construir
- Garantir que a solução vai funcionar
- Substituir o julgamento criativo sobre como resolver o problema
- Dar precisão real — a escolha do que medir e a interpretação de "5% a mais é bom?" são sempre atos de julgamento

## Dados incluem mais do que AB tests

Julie Zhuo define dados de forma ampla: inclui quantitativo (métricas, AB tests, DAU), qualitativo (entrevistas de usuário, comentários virais no TikTok, conversas de customer success) e dados de comportamento social (o que viralizou, o que as pessoas compartilham). Com IA, a síntese de dados qualitativos ficou muito mais viável — o argumento "qualitativo não escala" está enfraquecendo.

## O problema das empresas de IA hoje

Julie Zhuo observou um padrão: empresas de IA crescem tão rápido que chegam a centenas de milhões de ARR com 10 pessoas e sem infraestrutura de dados (logs, instrumentação, transformação de dados). Elas sobrevivem em "instintos e vibes" — e funciona, até parar de funcionar. Quando o crescimento desacelera, quem não tem observabilidade do negócio entra em pânico sem saber onde olhar.

**Implicação:** instrumentação e observabilidade de negócio não são luxo de empresa grande. São o que permite saber onde está o problema quando as coisas param de crescer.

## Análise conversacional — nova fronteira

Com produtos baseados em LLMs, métricas clássicas (cliques, sessões, tabs) não funcionam. A sessão inteira é conversa. Medir valor de uma conversa requer:
- Usar ML para inferir intenção do usuário a partir do texto
- Entender se a conversa foi bem — uma pergunta respondida em uma troca é diferente de uma conversa longa e frustrada
- Inventar novas metodologias — o campo está em aberto

## Insights por autor
### [[Julie Zhuo]]
- "You want to diagnose with data and treat with design." — a frase-âncora
- "Data is not a tool that's going to tell you what you should build. But it can tell you if you have a problem and where that problem or opportunity might be."
- "These companies are totally getting by on just good instincts and good vibes. But what always happens is eventually things stop growing."
- "A lot of fast-growing companies are not using data well at this point." — sobre startups de IA
- "To me data is also what did people put onto TikTok and which things went viral, what are they saying in the X verse. If you do a customer interview, that's still all data."
- "You just actually can't make a really great product by thinking you can A-B test your way into it."
> 🎧 [From managing people to managing AI: The leadership skills everyone needs now](https://www.youtube.com/watch?v=c_w0LaFahxk)

## Conceitos relacionados
[[Medição vs Insight — Instrumentação Rica]] · [[Pesquisa como Performance de Centralidade no Cliente]] · [[Falsificar, não Validar]] · [[Decidir com poucos dados é melhor que com zero]] · [[CC-CD — Calibração Contínua, Desenvolvimento Contínuo]]
