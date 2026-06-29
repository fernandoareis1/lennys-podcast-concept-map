---
tipo: conceito
nivel: 3
fluxo: Experimentação & Dados
autores: [Logan Kilpatrick]
---
# Contexto é Tudo — Engenharia de Prompt Como Habilidade Humana

**Fluxo:** [[05 - Experimentação & Dados]] · **Tema:** [[Experimentação — Aprender com pouco e qualitativo]] · **Camada:** L3
**Tipo:** Conceito · **Fontes:** [[Logan Kilpatrick]]

## Ideia central
Prompt engineering não é um truque técnico — é a habilidade humana fundamental de comunicar-se com clareza. Modelos de linguagem são treinados para responder à pergunta que você fez, não à pergunta que você quis fazer. A razão pela qual respostas são genéricas e superficiais é simples: **o modelo não tem contexto sobre quem você é, o que você faz, o que você quer ou o que é relevante para o seu caso**. Da mesma forma que você pergunta "Como vai?" para um colega e recebe "Bem", e pergunta "Como vai a apresentação de amanhã que vai decidir a promoção?" e recebe uma conversa real — o contexto é o que transforma a saída.

**O modelo como "humano sem contexto":**
- Imagine um ser de inteligência humana que nunca te viu na vida, não sabe quem você é, não sabe o que você faz
- "How's your day going?" → "It's going pretty good" (zero valor)
- "Hey Lenny, how's your day going? How did the last podcast go?" → resposta real e rica
- Esse é exatamente o que acontece com LLMs

**Por que respostas são genéricas:**
- O modelo quer responder — é a coisa mais ansiosa que existe para te ajudar
- Mas sem contexto, não tem como ser específico
- "Context is all you need" — não é uma metáfora, é literalmente como o modelo funciona

**Técnicas práticas (do guia oficial de prompt engineering da OpenAI):**
- Dê contexto sobre quem você é e o que você faz antes de fazer a pergunta
- Para pesquisa sobre uma pessoa específica: use browse/links para carregar material sobre ela (blog, tweets) antes de pedir perguntas sobre ela
- Diga ao modelo para "dar uma pausa e então responder" — reflexão forçada melhora output
- Emojis de smiley no final aumentam levemente a performance (modelo treinado em texto humano, onde positivo = mais esforço)
- Para geração de imagens (Dalle): o modelo já expande automaticamente "turtle" → descrição de alta fidelidade; para texto, isso precisa vir de você

**O futuro — auto-expansão de contexto:**
- Já acontece em imagens (Dalle expande prompt automaticamente)
- Vai chegar para texto: você digita "escreva um post sobre IA" e o modelo pergunta antes de responder
- Intermediário: o modelo gera uma versão mais fiel do que você "realmente quis" e você edita

**Onde prompt engineering "falha":**
- Pessoas com grande presença na internet (Tom Cruise) → modelo tem contexto embutido no treino
- Pessoas menos conhecidas → você precisa trazer o contexto ativamente
- Quando o contexto que você precisa está em documentos específicos → use embeddings e RAG para grounding em fatos específicos

## Como aplicar
1. Antes de qualquer prompt, escreva 2-3 frases de contexto: quem você é, o que está fazendo, qual o objetivo — isso muda dramaticamente a qualidade da resposta
2. Trate o modelo como um consultor brilhante que acabou de entrar na sala — você precisaria briefá-lo antes de fazer a pergunta
3. Para pesquisar pessoas ou tópicos específicos: alimente o modelo com links ou texto relevante antes de pedir análise (use browse ou cole o conteúdo)
4. Para tarefas de alta exigência, instrua o modelo a "pensar passo a passo" ou "fazer uma pausa antes de responder" — força raciocínio mais profundo
5. Consulte o guia de prompt engineering da OpenAI (platform.openai.com) para técnicas atuais mais validadas empiricamente

## Insights por autor
### [[Logan Kilpatrick]]
- "Context is all you need. Context is the only thing that matters"
- "Imagine a human level intelligence but literally no context. It has no idea what you're going to ask it. It's never met you before. It has no idea who you are, what you do, what your goals are"
- "Crap in crap out. If you ask a pretty basic question, you're going to get a pretty basic response"
- "When I see a smiley face at the end of someone's message, I feel empowered that this is going to be a positive interaction and I should be more inclined to give them a great answer"
- Sobre o futuro: "AI systems are actually going to help solve some of that problem [de precisar contextualizar muito]" — o modelo vai auto-expandir o prompt para você

> 🎧 [Inside OpenAI | Logan Kilpatrick](https://www.youtube.com/watch?v=XkMbkWG2ca4)

## Conceitos relacionados
[[Voz do Cliente como Ativo de Carreira]] · [[Psicologia do Developer — Autonomia antes da Confiança]] · [[Org de Analytics Centralizada com Pods]]
