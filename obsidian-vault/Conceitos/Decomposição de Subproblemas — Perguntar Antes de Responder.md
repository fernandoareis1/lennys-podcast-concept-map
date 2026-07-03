---
tipo: técnica
nivel: 3
fluxo: Experimentação & Dados
autores: [Sander Schulhoff]
---
# Decomposição de Subproblemas — Perguntar Antes de Responder

**Tema:** [[Experimentação — AB testing & cultura]] · **Fluxo:** [[05 - Experimentação & Dados]]

Antes de pedir a resposta final a um LLM, peça que ele identifique os subproblemas que precisam ser resolvidos primeiro. Essa etapa intermediária de decomposição melhora dramaticamente a qualidade da saída final em tarefas complexas.

## O padrão

Em vez de:
> "Resolva X"

Use:
> "Quais subproblemas precisam ser resolvidos para que X seja respondido adequadamente?"

Deixe o modelo responder essa pergunta. Depois:
> "Agora resolva X, levando em conta esses subproblemas."

## Por que funciona

LLMs são autoregressive — geram um token de cada vez com base no que veio antes. Quando a tarefa é complexa, a solução "direta" frequentemente pula etapas de raciocínio intermediário que seriam óbvias para um especialista humano.

A decomposição força o modelo a:
1. Mapear o espaço do problema antes de comprometer-se com uma solução
2. Ativar conhecimento relevante que não seria acessado na rota direta
3. Criar uma estrutura que serve como guia (e constrangimento) para a resposta final

## Exemplo — Concessionária de carros

Sander usa o exemplo de uma concessionária perguntando "Devemos oferecer financiamento de 0% para atrair clientes?":

**Sem decomposição:** o modelo responde diretamente, provavelmente com argumentos genéricos de marketing.

**Com decomposição:** o modelo primeiro identifica subproblemas:
- "Qual é o impacto de 0% no custo de capital da concessionária?"
- "Que tipo de cliente responde a esse incentivo vs. o que já compraria?"
- "Como os concorrentes estão posicionados?"
- "Qual é o efeito no mix de modelos vendidos?"

A resposta final, tendo mapeado esses subproblemas, é significativamente mais sofisticada.

## Variações

- **Chain-of-thought** é um primo desta técnica: "pense passo a passo" força estruturação similar
- **Tree-of-thought**: decompõe em múltiplos ramos e escolhe o mais promissor
- Para pipelines de IA, a decomposição pode virar uma etapa explícita no fluxo antes de chamar o modelo principal

## Quando usar

Especialmente útil em: análises de negócio, decisões de produto, diagnóstico de código, design de sistemas. Menos necessário em tarefas simples onde a decomposição é trivial.
