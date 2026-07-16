---
tipo: conceito
nivel: 3
fluxo: Estratégia & Visão
autores: [Logan Kilpatrick]
---
# Verticalizar para Não Competir com a Plataforma

**Fluxo:** [[02 - Estratégia & Visão]] · **Tema:** [[Estratégia — Posicionamento & diferenciação]] · **Camada:** L3
**Tipo:** Conceito · **Fontes:** [[Logan Kilpatrick]]

## Ideia central
Ao construir em cima de uma plataforma de IA (OpenAI, Anthropic, etc.), a pergunta mais importante não é "o que eu posso fazer com isso?" mas **"onde a plataforma não vai?".** A OpenAI está focada em capacidades gerais — raciocínio, código, escrita, agentes gerais. Quem vai competir diretamente com isso está brigando com a empresa que controla o modelo. Quem constrói para um vertical específico (direito, saúde, design gráfico, sales) usa o modelo como commodity e adiciona a camada que a plataforma nunca vai construir: domínio especializado, UX específica, dados proprietários, integrações de fluxo de trabalho, e conhecimento tácito do setor.

**O princípio:**
- OpenAI constrói a "camada geral": reasoning, coding, writing, imagem, voz
- Você constrói a "camada específica": Harvey para direito, Runway para vídeo criativo, Jasper para marketing
- O modelo melhora continuamente → seus diferenciais verticais se tornam relativos ao modelo, não abolidos por ele

**O risco do produto horizontal:**
- Produto geral que compete com ChatGPT precisa ser "radicalmente diferente" em 10 dimensões que ChatGPT tem problemas
- Caso contrário você está engenheirizando a mesma coisa que a OpenAI, com menos recursos de pesquisa
- "I have a lot of empathy for people who are building general assistants — it's a good idea, but you shouldn't be surprised when we end up launching some general purpose agent product"

**O modelo mental correto:**
- "Será que a OpenAI vai lançar um agente de sales de IA? Não." → seguro para construir
- "Será que a OpenAI vai lançar um assistente geral?" → provavelmente sim
- Vertical = domínio + dados + UX + integrações que a OpenAI não vai construir

**GPTs como caso especial:**
- GPTs são a estratégia da OpenAI de distribuir verticalização para criadores
- Para quem não é desenvolvedor: GPT é uma forma de criar produto vertical sem código
- Para startups: GPT pode ser produto ou caminho de descoberta — mas não é moat (qualquer um pode copiar a instrução)

**O que cria moat em produto de IA:**
- Dados proprietários (Harvey tem dados de casos jurídicos que ninguém mais tem)
- Integração de fluxo de trabalho específico (Zapier conecta tudo, nenhuma LLM vai construir 5.000 integrações)
- Especialização de UX (Visual Electric tem interface para designers, não é só "imagem de turtle")
- Network effect dentro do vertical

## Como aplicar
1. Ao avaliar uma ideia de produto de IA, pergunte: "Isso é horizontal (qualquer um pode usar) ou vertical (serve a um setor/use case específico com necessidades únicas)?"
2. Para definir o vertical: identifique onde existe conhecimento tácito não disponível no treinamento geral do modelo — regulação de setor, terminologia proprietária, fluxo de trabalho específico
3. Mapeie explicitamente o que a OpenAI provavelmente vai lançar nos próximos 2-3 anos (capacidades gerais, novos modelos) e o que definitivamente não vai (seu vertical específico)
4. Avalie: "Os dados que meu produto gera podem ser usados para melhorar o produto de IA?" — se sim, você tem um loop que cria moat ao longo do tempo
5. Para produtos gerais: o bar é "10 problemas que o ChatGPT tem" — liste os 10 antes de construir; se não encontrar, repense a tese

## Insights por autor
### [[Logan Kilpatrick]]
- "We're deeply focused on very, very general use cases — I think where you start to get into vertical applications, there's a great example: Harvey"
- "Our goal and our mission is really to solve this very general use case and then people can do things like fine-tuning and build all their own custom UI and product features on top of that"
- "You shouldn't be surprised when we end up launching some general purpose agent product — but we're not going to launch an AI sales agent. That's just not what we're building towards"
- "If you're going to try to build the next general assistant, it has to be so radically different — people have to really be like, 'Wow, this is solving these 10 problems that I have with ChatGPT'"
- Sobre GPTs: "Very narrow vertical tools are what's going to be a huge unlock for [the next billion people coming online into AI]"

> 🎧 [Inside OpenAI | Logan Kilpatrick](https://www.youtube.com/watch?v=XkMbkWG2ca4)

## Conceitos relacionados
[[Product-Led Growth (PLG)]] · [[Profundidade antes de amplitude]] · [[Beachhead + Bowling Pin — Cruzar o Abismo]] · [[Disruption por Expansão de Supply]]
