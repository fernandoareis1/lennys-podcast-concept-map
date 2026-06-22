---
tipo: framework
nivel: 3
fluxo: Design & UX
autores: [Alexander Embiricos]
---
# Assistência Contextual Mista
**Fluxo:** [[04 - Design & UX]] · **Tema:** [[Design — Experiência & fricção]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Alexander Embiricos]]

## Ideia central
O dilema do design de agentes: se um agente faz mil coisas por dia por você e precisa notificar cada ação, você recebe mil push notifications — insuportável. A solução é **assistência contextual mista** (mixed-initiative): o agente detecta o que você está tentando fazer com base no contexto (o que você está olhando, o que está fazendo) e **surfa ações sugeridas no momento certo**, em vez de interromper com notificações aleatórias. O modelo é o autocomplete de IDE: quando está certo, você acelera; quando está errado, você ignora e segue em frente — fricção aceitável. O Tesla Autopilot como masterclass: você mantém controle (acelerar, virar o volante, ajustar velocidade) sem desligar o sistema. O agente age, mas o humano permanece no controle de forma natural e fluida.

## Como aplicar
1. **Prefira superfície contextual a notificação push**: em vez de "o agente fez X, aprove", projete para "você está olhando para Y → aqui está uma sugestão relevante agora".
2. **Use o modelo do autocomplete como referência de UX**: baixo custo de erro (fácil ignorar), alto ganho quando certo, integrado ao fluxo existente.
3. **Crie mecanismos de controle granulares**: o usuário não deve precisar "desligar o agente" para ajustar seu comportamento. Controles incrementais (como o volante no Autopilot) permitem colaboração fluida.
4. **Construa com contexto de domínio**: um agente com acesso nativo ao que o usuário está vendo (browser, IDE, dashboard) pode surfaçar ajuda muito mais relevante do que um que depende de screenshots ou accessibility APIs.
5. **Teste a pergunta "o usuário sabe o que o agente pode fazer aqui?"**: se a resposta for não, a UX falhou — o usuário não vai invocar a ajuda disponível. O design deve tornar as capacidades do agente discerníveis no momento certo.

## Insights por autor
### [[Alexander Embiricos]]
- "Imagine que chegamos a um mundo onde temos agentes ajudando você milhares de vezes por dia. Se a única forma de comunicar que ajudamos era através de push notification... você receberia mil notificações por dia. Seria super irritante."
- Solução: "Você está olhando para um dashboard e notou que uma métrica caiu. Nesse momento, uma IA pode tomar uma olhada e surfaçar o fato de que tem uma opinião sobre por que essa métrica caiu — e talvez um fix — exatamente quando você está olhando para ela."
- Tesla como referência: "Acho que o Tesla fez um trabalho realmente bom em habilitar o carro para se dirigir sozinho, mas com todas essas formas diferentes de ajustar o que está fazendo sem desligar o self-driving... é uma masterclass em construir um agente que ainda deixa o humano no controle."
- O autocomplete como validação histórica: "Auto-completion em IDEs é um dos produtos de IA mais bem-sucedidos hoje. Quando está certo, você acelera. Quando está errado, não é tão irritante. Você cria esse sistema de iniciativa mista que responde contextualmente ao que você está tentando fazer."
- A razão estratégica do browser: acesso nativo ao rendering engine elimina dependência de screenshots ou accessibility APIs — dando ao agente muito mais contexto confiável sobre o que o usuário está fazendo.

> 🎧 [Building Codex: OpenAI's coding agent (1:16:34)](https://www.youtube.com/watch?v=xZifSLGOrrw)

## Conceitos relacionados
[[Proatividade como Destino dos Agentes]] · [[Reduzir fricção em vez de adicionar features]] · [[Trade-off Agência-Controle]] · [[Design — Experiência & fricção]]
