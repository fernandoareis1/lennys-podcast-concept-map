---
tipo: técnica
nivel: 3
fluxo: Experimentação & Dados
autores: [Sander Schulhoff]
---
# Few-Shot Prompting — Exemplos como Maior Uplift Individual

**Tema:** [[Experimentação — AB testing & cultura]] · **Fluxo:** [[05 - Experimentação & Dados]]

Dentre todas as técnicas de prompt engineering, few-shot prompting — incluir exemplos de input/output antes da tarefa real — é a de maior uplift individual. A distância de zero-shot para few-shot é a maior que existe entre qualquer par de técnicas.

## O que é

Few-shot prompting consiste em fornecer ao modelo 3–10 exemplos da tarefa que você quer que ele execute antes de pedir a tarefa real:

```
Usuário: Traduza para francês.
Input: "The weather is nice today."
Output: "Le temps est beau aujourd'hui."

Input: "I love coffee."
Output: "J'adore le café."

Input: "Where is the train station?"
Output: [model completes here]
```

O formato Q/A (pergunta/resposta) é o mais comum e funciona em praticamente qualquer domínio.

## Por que funciona

Os exemplos sinalizam simultaneamente três coisas ao modelo:
1. **Formato esperado** — comprimento, estrutura, tom
2. **Conteúdo esperado** — nível de detalhe, vocabulário
3. **Tarefa exata** — remove ambiguidade da instrução em texto

Sem exemplos, o modelo interpreta a instrução com base em distribuições gerais do treinamento. Com exemplos, o modelo recalibra para a distribuição específica que você quer.

## Dados de Sander

Nos experimentos do Learn Prompting e do HackAPrompt, few-shot prompting consistentemente produziu o maior salto de qualidade em relação a qualquer outra técnica isolada. O impacto é especialmente grande em:
- Tarefas de extração estruturada (JSON, tabelas)
- Tarefas criativas com tom específico
- Classificação com categorias não-padrão

## Quando NÃO ajuda

Few-shot prompting não ajuda (e pode prejudicar) quando:
- Os exemplos são inconsistentes entre si
- Os exemplos são diferentes da distribuição do input real
- O contexto disponível é limitado e exemplos "comem" espaço de instruções críticas

## Aplicação prática

- Use no mínimo 3 exemplos; o ganho marginal depois de 10 é pequeno
- Coloque exemplos APÓS as instruções, ANTES da tarefa real
- Se os exemplos variam em estilo, o modelo vai variar também — seja consistente
