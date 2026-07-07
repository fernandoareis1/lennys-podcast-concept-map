---
tipo: mindset
nivel: 3
fluxo: Estratégia & Visão
autores: [Benjamin Mann, Karina Nguyen]
---
# Construir para o disco futuro
**Fluxo:** [[02 - Estratégia & Visão]] · **Tema:** [[Estratégia — Estratégia de produto]] · **Camada:** L3
**Tipo:** Mindset · **Fontes:** [[Benjamin Mann]] · [[Karina Nguyen]]

## Ideia central
Em era de progresso exponencial em IA, times de produto cometem o erro de construir para as capacidades **atuais** do modelo. O mindset correto é "skate to where the puck is going": **construa para as capacidades de 6 a 12 meses no futuro**.

A heurística: se algo está funcionando 20% das vezes hoje, vai estar funcionando 100% das vezes em 6 meses. Tomar essa curva a sério muda radicalmente as apostas de interface, arquitetura e priorização de roadmap.

**Exemplo do Claude Code**: a equipe apostou no terminal como interface primária para agentes de engenharia. À época, parecia limitado. A lógica: terminal é location-agnostic (roda local, em GitHub Actions, em cluster remoto) — e quando os agentes ficarem suficientemente bons, isso importa muito. A interface certa para 2026 foi escolhida em 2024.

O antídoto ao erro: internalize a curva exponencial concretamente — não como fato abstrato, mas como premissa de design. Para cada feature, pergunte: "Estou construindo para o modelo de hoje ou para o modelo que existirá quando esta feature tiver tração?"

## Como aplicar
1. **Mapeie as capacidades em desenvolvimento** com horizonte de 6-12 meses, não apenas capacidades atuais. Use benchmarks como proxy.
2. **Identifique o que hoje funciona 20%** e projete que estará em 100% em breve. Esses são os candidatos para apostar agora.
3. **Escolha interfaces que escalam com a inteligência do agente**, não com a conveniência de hoje. Terminal > chat > autocomplete em termos de grau de liberdade quando agentes ficarem mais fortes.
4. **Resistir à tentação de polir para as limitações atuais**: não simplifique a UX para compensar o que o modelo ainda não faz bem — o modelo vai melhorar; a arquitetura vai ficar presa.
5. **Recalibrar o roadmap a cada ciclo**: com lançamentos mensais de modelos, o horizonte de "onde o disco está indo" se encurtou; recalibrar com mais frequência.

## Insights por autor
### [[Benjamin Mann]]
- "Skating to where the puck is going: não construa para hoje, construa para 6 meses a frente, um ano à frente."
- "As coisas que funcionam 20% das vezes vão começar a funcionar 100% das vezes. E acho que foi isso que fez o Claude Code ser um sucesso."
- "As pessoas não vão ficar presas em IDEs para sempre. Vão fazer tudo que um engenheiro de software precisa fazer, e o terminal é o lugar certo porque pode ficar em muitos lugares."
- "São AGI-pilled o suficiente? É a pergunta que eu sempre faço para o time."
> 🎧 Episódio com Benjamin Mann, co-founder da Anthropic (frontmatter do transcript com erro — URL não disponível)

### [[Karina Nguyen]]
- "A Canvas idea estava no ar desde 2022, antes do ChatGPT. Mas o modelo Claude 1.3 não estava lá para fazer edições de alta qualidade. Você constrói ideias de produto de forma que, quando os modelos estiverem realmente bons, vai funcionar muito bem."
- "Form follows function. O form factor de file uploads pode permitir que as pessoas literalmente façam upload de qualquer coisa — livros, relatórios financeiros — e perguntem qualquer tarefa ao modelo."
- "Notificações são muito familiares, ter lembretes é muito familiar. Então você pega um form factor familiar — Canvas é como Google Docs, Tasks é como alarme de celular — e adiciona um momento mágico de IA, e se torna muito poderoso."
> 🎧 [OpenAI researcher on why soft skills are the future of work](https://www.youtube.com/watch?v=DeskgjrLxxs) · 2025-02-09

## Conceitos relacionados
[[Teste de Turing Econômico]] · [[Dois de três pontos de inflexão]] · [[Hill Climb — ótimo local vs global]] · [[Do Computador Pessoal ao Modelo Pessoal]]
