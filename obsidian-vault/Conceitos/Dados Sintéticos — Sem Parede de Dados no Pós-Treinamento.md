---
tipo: insight
nivel: 3
fluxo: Experimentação & Dados
autores: [Karina Nguyen]
---
# Dados Sintéticos — Sem Parede de Dados no Pós-Treinamento
**Fluxo:** [[05 - Experimentação & Dados]] · **Tema:** [[Experimentação — Aprender com pouco e qualitativo]] · **Camada:** L3
**Tipo:** Insight · **Fontes:** [[Karina Nguyen]]

## Ideia central
O debate sobre "parede de dados" (data wall) confunde dois tipos de treinamento radicalmente diferentes:

- **Pré-treinamento**: limitado pelo que existe na internet. Quando esgota a diversidade de texto, os ganhos marginais caem.
- **Pós-treinamento via RL (reinforcement learning)**: não tem parede de dados — porque você treina sobre **tarefas geradas sinteticamente**, não sobre texto existente. A quantidade possível de tarefas é virtualmente infinita.

> "O que está acontecendo agora com o novo paradigma da série o1 é que o scaling no pós-treinamento não está atingindo a parede. Porque passamos de datasets brutos de pré-treinamento para uma quantidade infinita de tarefas que você pode ensinar ao modelo no mundo do pós-treinamento via reinforcement learning."

## Como a síntese funciona na prática

### O caso Canvas
Karina treinou três comportamentos core do Canvas inteiramente via dados sintéticos:

1. **Trigger detection** — quando acionar o Canvas vs. não acionar. Exemplo: "Write me a long essay" → aciona; "Tell me about X" → não aciona. O modelo precisa inferir intenção (iteração sobre documento longo vs. resposta pontual).

2. **Edição de documento** — dois modos distintos:
   - *Targeted edit*: selecionar a segunda parágrafo e reescrevê-la no tom pedido
   - *Full rewrite*: substituir o documento inteiro quando a qualidade do rewrite for superior
   Na versão beta, o modelo foi biasado para rewrites completos (qualidade mais alta). Com feedback de usuários, a distribuição foi ajustada.

3. **Comentários** — usar o modelo o1 para simular uma conversa ("Write me a document about XYZ"), gerar o documento, injetar um prompt ("Critique this piece"), treinar o modelo a fazer comentários em trechos específicos com feedback de qualidade.

> "A razão pela qual eu realmente gosto de depender puramente de dados sintéticos em vez de coletar dados de humanos é que é muito mais escalável, mais barato. Você literalmente amostra do modelo e ensina os comportamentos core, e isso vai generalizar para toda a cobertura diversa."

### O fluxo completo: sintético → beta → GA
1. Defina os comportamentos core com evals
2. Gere dados sintéticos para treinar esses comportamentos
3. Lance em beta e colete feedback real de usuários
4. Ajuste a distribuição dos dados sintéticos com base no que os usuários fazem
5. Generalize para GA (general availability)

Canvas e Tasks seguiram esse fluxo exato.

## Diversidade em dados sintéticos: a fronteira ativa
O maior desafio de dados sintéticos não é quantidade, mas **diversidade**. Modelos treinados em dados sintéticos pouco diversos ficam bons em cenários narrow mas falham em distribuições de usuário reais.

> "Um dos problemas mais difíceis sobre dados sintéticos é como torná-los mais diversos? Diversidade em dados sintéticos é uma das questões mais importantes agora."

Injetar diversidade sistematicamente em dados sintéticos gerados é um problema de pesquisa ativo nas labs.

## Implicação para builders
- Você não precisa de dados reais de usuários para começar a treinar comportamentos. Pode iterar em loop fechado com dados sintéticos até ter sinal de produto.
- A lógica de "sem dados, sem modelo" é válida para pré-treinamento; no pós-treinamento, qualquer comportamento definível em evals pode ser sintetizado.
- Prompting como prototipagem: antes de treinar, prototipe o comportamento com prompts. Se funcionar via prompt, você tem a especificação para os dados sintéticos.

## Insights por autor
### [[Karina Nguyen]]
- "People think we are hitting the data wall. I think people think more in terms of pre-trained large models trained on the entire internet. But what's happening now with the o1 series is that the scaling in post-training is not hitting the wall."
- "There will be infinite amount of tasks and that's how the model becomes extremely superintelligent."
- "Synthetic data training is more for product... It's rapid model iteration for similar product outcomes. The way we made Canvas and Tasks was mostly done by synthetic training."
- Sobre diversidade: "One of the hardest things about synthetic data is how do you make it more diverse? Diversity in synthetic data is one of the most important questions right now."
> 🎧 [OpenAI researcher on why soft skills are the future of work](https://www.youtube.com/watch?v=DeskgjrLxxs) · 2025-02-09

## Conceitos relacionados
[[Era dos evals — o eval é o PRD do modelo]] · [[Pós-treinamento como nova fronteira]] · [[Post-Training como Novo Frontier — Do Pré-treinamento ao Especialista]] · [[CC-CD — Calibração Contínua, Desenvolvimento Contínuo]] · [[Non-determinismo em Produtos de IA]]
