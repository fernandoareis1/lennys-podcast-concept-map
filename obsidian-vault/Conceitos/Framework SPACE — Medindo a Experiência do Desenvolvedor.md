---
tipo: framework
nivel: 3
fluxo: Priorização & Roadmap
autores: [Nicole Forsgren]
---
# Framework SPACE — Medindo a Experiência do Desenvolvedor
**Fluxo:** [[03 - Priorização & Roadmap]] · **Tema:** [[Priorização — Outcomes & metas]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Nicole Forsgren]]

## Ideia central
Medir produtividade de engenharia com uma única métrica (linhas de código, número de PRs, velocidade de sprint) é uma armadilha — qualquer métrica isolada é facilmente gameable. O **Framework SPACE** propõe cinco dimensões complementares que, juntas, capturam a real saúde de um time de desenvolvimento:

- **S**atisfaction — o quanto os desenvolvedores estão satisfeitos com o trabalho, ferramentas e time
- **P**erformance — os outcomes alcançados (qualidade do código, impacto nos usuários, redução de bugs)
- **A**ctivity — contagens de atividades (PRs, deployments, commits) como *sinais*, não fins em si
- **C**ommunication & Collaboration — como o time e os sistemas se comunicam; quanto trabalho vai para um chatbot vs. um colega
- **E**fficiency & Flow — capacidade de entrar em estado de flow, throughput do sistema, tempo gasto em trabalho que não gera valor

**A chave:** SPACE é um *framework* (não uma receita prescritiva). Ao contrário do DORA — que tem quatro métricas fixas sobre velocidade e estabilidade do pipeline — SPACE não diz o que medir. Isso é sua força: permite que cada time adapte as dimensões ao seu contexto. No mundo de IA, SPACE se expande naturalmente para incluir uma sexta dimensão: **Trust** — o quanto os desenvolvedores confiam no código gerado pela IA.

**Por que métricas prescritivas falham na era da IA:**
- Linhas de código: trivialmente gameable com AI gerando código verboso
- DORA (deployment frequency, lead time, MTTR, change fail rate): válido para medir o pipeline, mas cego às novas formas de feedback loop que AI introduz
- Qualquer métrica isolada cria o incentivo errado

## Três dimensões de DevEx que toda métrica deve respeitar
1. **Flow state** — capacidade de entrar em concentração profunda; AI interrompe o flow tradicional (linha a linha) mas cria novos flows (gerir agentes, revisar outputs)
2. **Cognitive load** — quanto espaço mental é consumido pela mecânica do sistema; alta carga cognitiva bloqueia inovação mesmo quando a produtividade de output parece boa
3. **Feedback loops** — velocidade com que o desenvolvedor sabe se algo funcionou; AI acelera drasticamente esses loops, mas também os redistribui (feedback chega no meio do processo, não só ao final)

## Como aplicar
1. **Não comece com ferramentas** — comece com entrevistas: "Me conte sobre ontem. O que foi fácil? Onde você travou?"
2. **Use SPACE para mapear o estado atual** — identifique qual dimensão está mais comprometida no seu time
3. **Não meça felicidade, meça satisfação** — "Você está satisfeito com esta ferramenta?" tem sinal limpo; "você está feliz?" não tem
4. **Pesquisas rápidas com três perguntas** — satisfação geral + três maiores bloqueadores + frequência de cada bloqueador. Deixe o respondente escolher os top 3, não tudo
5. **Atribua métricas ao propósito** — para CEO/board: velocidade de ideia a experimento. Para devs: tempo economizado, menos toil. Para margem: custo de testes automatizados vs. manuais

## Insights por autor
### [[Nicole Forsgren]]
- "A maioria das métricas de produtividade são uma mentira. Linhas de código é muito fácil de manipular — posso promptar algo para escrever o código mais longo já escrito."
- "DORA tem quatro métricas. Se usadas para avaliar velocidade e estabilidade geral do pipeline, ótimo. Se usadas cegamente agora com IA, você vai perder fenômenos super importantes."
- "SPACE é um framework. Não digo o que medir. Às vezes as pessoas ficam frustradas porque eu não digo. Mas essa é a sua força."
- "No contexto de IA, eu adicionaria uma nova dimensão ao SPACE: Trust. Confiança — LLMs são não-determinísticos. Você não pode simplesmente aceitar o output."
- "Felicidade é muito ampla. Satisfação pode ser medida com sinal limpo: 'Você está satisfeito com essa ferramenta?' e você pode fazer perguntas de follow-up."
> 🎧 [How to measure AI developer productivity in 2025 (1:07:48)](https://www.youtube.com/watch?v=SWcDfPVTizQ) · 2025-10-19

## Conceitos relacionados
[[Métricas de input vs. output]] · [[PM Orientado a Impacto]] · [[DevEx como Produto — Sete Passos]] · [[Intensidade por Minuto — Kilojoules por Hora]]
