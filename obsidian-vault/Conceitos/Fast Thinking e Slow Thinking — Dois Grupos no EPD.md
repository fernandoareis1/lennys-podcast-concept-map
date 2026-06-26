---
tipo: framework
nivel: 3
fluxo: Liderança & Times
autores: [Howie Liu]
---
# Fast Thinking e Slow Thinking — Dois Grupos no EPD
**Fluxo:** [[09 - Liderança & Times]] · **Tema:** [[Liderança — Modelos de time]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Howie Liu]]

## Ideia central
Inspirado em Kahneman (*Thinking, Fast and Slow*), Howie Liu reestruturou o EPD (Eng, Product, Design) da Airtable em dois grupos com modos de operação fundamentalmente diferentes:

| | Fast Thinking (AI Platform) | Slow Thinking (Core Platform) |
|---|---|---|
| **Velocidade** | Semanal — ship features toda semana | Meses — infraestrutura, arquitetura |
| **Objetivo** | "Jaw-drop" — cada feature deve impressionar | Durabilidade — escala, segurança, retenção |
| **Mentalidade** | Startup interna, autonomia máxima | Engenharia robusta, pré-meditação |
| **Exemplo** | Omni (agente conversacional), code gen | HyperDB (100M+ registros), infra enterprise |
| **Função de crescimento** | Top of funnel — excitação, novos casos de uso | Converter sementes em deployments duradouros |

## Como se complementam
O grupo Fast cria o excitamento que traz novos usuários — incluindo enterprise. O grupo Slow garante que esses usuários retêm e expandem. Sem Fast: produto morre de irrelevância. Sem Slow: top of funnel vira "AI tourists" que não ficam.

Problema do Fast sem Slow: muitas empresas AI-nativas têm pipeline wide mas conversão em crescimento durável fraco. Problema do Slow sem Fast: incumbentes lentos que ship AI features a cada quarter quando o mercado muda toda semana.

## Critérios de design para o grupo Fast
- **Autonomia máxima**: membros devem operar quase como founders, sem precisar de aprovação em cascata
- **Polimatas**: PMs que prototipam, designers que entendem modelos, engenheiros com product taste
- **Não prescrição de "o quê"**: o líder define a missão ("dar superpoderes a field agents"), não os watermelons específicos a pegar
- **Protótipos sobre documentos**: demo funcional > PRD; o produto de IA tem que ser experienciado, não lido

## Anti-padrão anterior
Estrutura baseada em feature ownership: um time para search, um para mobile, um para automations. Benefício: ramp-up de codebase. Desvantagem: cada time melhora incrementalmente sua feature, sem olhar para outcomes holísticos que exigem mudança cross-feature.

## Insights por autor
### [[Howie Liu]]
- "Fast thinking significa ship um monte de novas capacidades de AI em base quase semanal. Cada uma deve ser genuinamente incrível. Você deve ter o queixo caindo."
- "Slow thinking não é melhor ou pior. Você não pode só shipar HyperDB (que suporta centenas de milhões de registros) em uma semana como protótipo hacky. É um modo diferente de planejar e executar."
- "Cursor e Windsurf estão shipando features major toda semana e não parece 'temos um roadmap enterprise e outro para SMB'. Parece um produto coeso que avança num ritmo absurdo. Isso é o que queremos."
> 🎧 [How we restructured Airtable's entire org for AI (0:22:12)](https://www.youtube.com/watch?v=GT0jtVjRy2E)

## Conceitos relacionados
[[IC CEO — Volta ao Craft na Era de IA]] · [[Single-Threaded Leader]] · [[Autonomia na Camada VP — O Ponto Ótimo da Organização]] · [[Produto-Ops como avião bimotor]]
