---
tipo: framework
nivel: 3
fluxo: Estratégia & Visão
autores: [Kevin Weil]
---
# Ensemble de Modelos Especializados

**Fluxo:** [[02 - Estratégia & Visão]] · **Tema:** [[Estratégia — Estratégia de produto]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Kevin Weil]]

## Ideia central
Para resolver problemas complexos, a estratégia superior não é usar um único modelo grande — é **quebrar o problema em tarefas específicas** e usar um conjunto de modelos especializados (fine-tuned) para cada uma. A OpenAI usa internamente mais de 20 chamadas de modelo para alguns dos seus problemas mais complexos.

**A analogia com empresas:**
Uma empresa é, ela própria, um ensemble de humanos "fine-tuned" para diferentes funções. O engenheiro é fine-tuned em código, o designer em experiência visual, o analista em dados. Nenhum único generalista executa tudo tão bem quanto uma equipe de especialistas. O mesmo princípio se aplica a sistemas de IA.

**Por que fine-tuning especializado supera o modelo maior genérico:**
- Modelos menores e especializados têm menor latência e custo por tarefa
- Fine-tuning em dados de domínio cria capacidade que o modelo geral não alcança
- O orchestrator (modelo orquestrador) pode escalar a complexidade horizontalmente, não verticalmente
- Permite especialização por requisito de confiança/custo: tarefas críticas usam modelos maiores; triagem usa modelos menores

**Implicação para produto de IA:**
A decisão de produto não é "qual modelo usar" mas "qual arquitetura de ensemble orquestra melhor as tarefas do meu produto?" Isso muda o design de um problema de seleção para um problema de composição.

## Como aplicar
1. Mapeie as tarefas distintas que o seu produto de IA executa. Para cada uma, avalie se um modelo especializado/fine-tuned superaria um modelo geral.
2. Identifique o "orchestrator" — o modelo ou lógica que decompõe o problema e despacha para os modelos especializados certos.
3. Para cada subtarefa, defina os requisitos: latência tolerável, custo por chamada, precisão mínima. Use modelos menores para tarefas de triagem; modelos maiores apenas onde necessário.
4. Invista em fine-tuning com dados próprios para as tarefas centrais do produto — isso cria moat de capacidade que competidores não conseguem replicar facilmente (ver [[Pós-treinamento como nova fronteira]]).
5. Monitore com evals por subtarefa, não apenas pelo output final — assim você identifica qual componente do ensemble está degradando.

## Insights por autor
### [[Kevin Weil]]
- "Uma empresa é um ensemble de humanos fine-tuned — o engenheiro, o designer, o analista. O modelo de IA pode e deve funcionar da mesma forma."
- A OpenAI usa internamente 20+ chamadas de modelo para resolver seus problemas mais complexos.
- Diferentes tarefas têm diferentes requisitos de latência e custo — isso determina o tamanho e tipo de modelo adequado para cada subtarefa.
- Fine-tuning em dados proprietários/especializados cria capacidade que modelos gerais não têm — e que é difícil de replicar.
- "Pós-treinamento com dados de especialistas é onde toda a melhoria de modelos está acontecendo agora."

> 🎧 [OpenAI's CPO on why ChatGPT is the worst AI you'll ever use | Kevin Weil](https://www.youtube.com/watch?v=scsW6_2SPC4) · 2025-04-10

## Conceitos relacionados
[[Pós-treinamento como nova fronteira]] · [[Era dos evals — o eval é o PRD do modelo]] · [[O loop e não o lane]] · [[Build and buy]] · [[Post-Training como Novo Frontier — Do Pré-treinamento ao Especialista]]
