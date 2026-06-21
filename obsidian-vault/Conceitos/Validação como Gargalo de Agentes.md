---
tipo: insight
nivel: 3
fluxo: Experimentação & Dados
autores: [Alexander Embiricos]
---
# Validação como Gargalo de Agentes
**Fluxo:** [[05 - Experimentação & Dados]] · **Tema:** [[Experimentação — AB testing & cultura]] · **Camada:** L3
**Tipo:** Insight · **Fontes:** [[Alexander Embiricos]]

## Ideia central
O gargalo do desenvolvimento de software não é mais *escrever* código — é *validar* código. Agentes de IA escrevem código depressa demais para humanos revisarem com conforto. O fator limitante agora é a **velocidade de digitação e multitarefa humana**: um usuário só consegue dar prompt a um agente e revisar seu output dezenas de vezes por dia, enquanto o potencial real é de milhares de interações. Enquanto o loop de validação exigir atenção humana constante, o ganho de produtividade fica represado.

A mesma lógica se aplica ao AGI: o momento em que modelos treinarem outros modelos em loop fechado — sem bottleneck de revisão humana — é o ponto de inflexão real. Por isso, o problema mais subestimado no desenvolvimento de agentes não é inteligência do modelo, mas *infraestrutura de auto-validação*.

## Como aplicar
1. **Identifique o seu gargalo de validação atual**: o que o agente entrega que ainda requer atenção humana para checar? Esse é o seu maior ponto de alavancagem.
2. **Design para "image before diff"**: no code review, mostrar primeiro o resultado visual (não o diff) deixa o usuário avaliar *se funcionou* antes de precisar entender *como funcionou*. Ordene a informação para minimizar a carga cognitiva de validação.
3. **Invista em auto-validação do agente**: prompts como "Por que você não consegue verificar o seu próprio trabalho? Corrija isso." permitem que o agente configure seu próprio harness de validação.
4. **Compaction para tarefas longas**: agentes que rodam overnight precisam de mecanismo para compactar o contexto antes de atingir o limite — sem isso, o loop fecha em poucas horas.
5. **Meça a qualidade da validação, não só a velocidade da geração**: KPIs como D7 retention e "vibes" em comunidades (Reddit) capturam se o resultado do agente é confiável, não apenas rápido.

## Insights por autor
### [[Alexander Embiricos]]
- "O fator limitante subestimado atual é literalmente a velocidade de digitação humana ou a velocidade de multitarefa humana ao escrever prompts."
- Escrever código é divertido para engenheiros; revisar código de IA é menos divertido. O produto precisa atacar o ponto de fricção, não só acelerar o que já é agradável.
- Compaction: feature que usa as três camadas do stack (modelo + API + harness) para permitir sessões de 24h+. O modelo precisa saber quando compactar; a API precisa ter o endpoint; o harness precisa preparar o payload.
- Codex como "on call" para o próprio treinamento: o agente monitora gráficos de training run que hoje humanos vigiam — a próxima fronteira de produtividade é o fechamento desse loop.
- "Se você construir o agente para que seja padrão útil, começaremos a desbloquear os hockey sticks. Infelizmente não acho que será binário — vai depender muito do que você está construindo."

> 🎧 [Building Codex: OpenAI's coding agent](https://www.youtube.com/watch?v=xZifSLGOrrw)

## Conceitos relacionados
[[Evals vs. Monitoramento em Produção]] · [[Agente de IA como Colega de Time]] · [[Framework CCCD]] · [[A-B Testing (Ronny Kohavi)]]
