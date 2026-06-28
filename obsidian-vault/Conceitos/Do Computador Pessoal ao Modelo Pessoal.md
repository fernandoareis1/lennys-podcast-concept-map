---
tipo: framework
nivel: 3
fluxo: Estratégia & Visão
autores: [Karina Nguyen]
---
# Do Computador Pessoal ao Modelo Pessoal
**Fluxo:** [[02 - Estratégia & Visão]] · **Tema:** [[Estratégia — Estratégia de produto]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Karina Nguyen]]

## Ideia central
A evolução dos produtos de IA segue uma progressão em três etapas análoga à história do computador pessoal:

1. **Chatbot síncrono** — paradigma atual. O modelo responde em tempo real quando você faz uma pergunta. Fácil de entender, mas você é o gargalo de produtividade (tem que prompar tudo).

2. **Agentes assíncronos** — agentes trabalham no background enquanto você faz outra coisa. A interação humana acontece na chegada (revisar resultados) e na saída (aprovar/ajustar), não em cada passo. Operador (OpenAI) é o primeiro representante desta fase.

3. **Modelo pessoal** — o modelo aprende suas preferências ao longo do tempo, torna-se personalizado ao seu estilo, e começa a **predizer as próximas ações** que você vai querer tomar. Isso é o análogo do computador pessoal: de ferramenta compartilhada e genérica para extensão individual.

> "Passamos de personal computers para personal model basicamente aqui."

## O papel da confiança
A transição do chatbot para o agente pessoal não é técnica — é **de confiança**. Agentes que trabalham autonomamente precisam construir confiança gradualmente, como acontece entre humanos.

> "A questão é que os agentes devem construir confiança com você, certo? E confiança se constrói ao longo do tempo, como com humanos. E você começa essa colaboração — por isso o modelo de colaboração com você e o modelo é tão importante, porque você constrói confiança e o modelo aprende com suas preferências para que possa se tornar mais personalizado e vai começar a predizer a próxima ação que você quer tomar."

Sem confiança construída, um agente que trabalha por 10 minutos e volta com a resposta errada é **pior** do que nenhum agente — porque você perdeu tempo e não tinha visibilidade do processo.

## Form factor segue função
Cada transição de paradigma tem um form factor natural que emerge da nova capacidade:

| Capacidade | Form factor óbvio |
|---|---|
| 100K context window | File uploads — qualquer documento, livro, relatório |
| Lembretes genéricos | Tasks/notifications — familiar como alarme de celular |
| Edição colaborativa | Canvas — familiar como Google Docs |
| Agente de computador | Virtual assistant — familiar como par de programação |

> "Form follows function. O form factor de file uploads pode permitir que as pessoas literalmente façam upload de qualquer coisa, livros, qualquer relatório, financeiro e perguntem qualquer tarefa ao modelo."

O insight: quando uma nova capacidade emerge, o form factor certo não é inventado — é **derivado** do caso de uso mais óbvio para aquela capacidade. Não foi preciso inventar file uploads depois do 100K context; era a forma natural que a função tomaria.

## Familiar + magia = poderoso
Tasks e Canvas não são breakthrough de funcionalidade. São form factors familiares com AI magic por dentro:

- Notificações (Tasks) = tão familiar quanto alarme de celular
- Editor colaborativo (Canvas) = tão familiar quanto Google Docs
- O que muda: o "assistente" dentro desses form factors é um modelo geral que sabe fazer tudo

> "O que torna muito legal é que os modelos são tão gerais... Dar algo familiar às pessoas é muito familiar, as mesmas notificações são muito familiares, ter lembretes é muito familiar. Então sentir um form factor para as pessoas que é muito familiar, como Canvas, Google Docs é muito familiar, mas então você adiciona um momento mágico de IA e se torna muito poderoso."

## Implicações para roadmap
- **Pense no form factor antes da capacidade**: antes de treinar o modelo, pergunte qual form factor uma capacidade nova tornaria óbvio para usuários.
- **Confiança como feature**: em produtos agênticos, onboarding de confiança não é soft — é o diferencial competitivo.
- **Personalização temporal**: o modelo pessoal requer memória e aprendizado de preferências ao longo do tempo; produtos que não constroem isso hoje ficam para trás quando a expectativa mudar.
- **Tasks como plataforma escalável**: features baseadas em tarefas agendadas escalam naturalmente com melhoria de modelos — conforme o modelo fica mais capaz, a mesma estrutura de task entrega mais valor sem reescrever a UX.

## Insights por autor
### [[Karina Nguyen]]
- "The paradigm between synchronous real time give an answer paradigm into more asynchronous paradigm of agents working on the background."
- "The agents should build trust with you. And trust builds over time, which is like with humans."
- "The model learns from your preferences so that it can become more personalized and will start predicting the next action that you want to take on the computer. We went from personal computers to personal model basically here."
- "Form follows function. The form factor of file uploads can enable people to just literally upload anything."
- "Giving something familiar to people — notifications is very familiar, having reminders is very familiar. So feeling like a form factor for the people who are very familiar, same as Canvas, Google Docs is very familiar, but then you add magical AI moment and it becomes very powerful."
> 🎧 [OpenAI researcher on why soft skills are the future of work](https://www.youtube.com/watch?v=DeskgjrLxxs) · 2025-02-09

## Conceitos relacionados
[[Proatividade como Destino dos Agentes]] · [[Trade-off Agência-Controle]] · [[Construir para o disco futuro]] · [[De Saber a Fazer — A Transição dos Agentes de IA]] · [[Produto como organismo]]
