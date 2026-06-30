---
tipo: tecnica
nivel: 3
fluxo: Experimentação & Dados
autores: [Michael Truell]
---
# Dogfooding como Bússola Tecnológica — Realismo sobre IA

**Fluxo:** [[05 - Experimentação & Dados]] · **Tema:** [[Experimentação — Aprender com pouco e qualitativo]] · **Camada:** L3
**Tipo:** Técnica · **Fontes:** [[Michael Truell]]

## Ideia central
O princípio mais fundamental do desenvolvimento do Cursor: nunca shipar algo que não seja útil para o próprio time. O Cursor foi construído para uso dos próprios fundadores — desde a primeira semana, eles já usavam o editor em tempo integral. Isso cria uma âncora de realismo que nenhuma métrica ou pesquisa de usuário substitui.

## A armadilha da antropomorfização

Quando alguém vê AI fazer algo mágico em uma área, há uma tendência humana de extrapolar: *"se é incrível aqui, deve ser incrível lá também."* Esse é o erro de antropomorfizar os modelos — assumir que eles têm capacidade humana generalizada porque demonstram capacidade específica.

O antídoto é usar o produto todo dia. Você vê os limites reais. Você sabe o que funciona e o que não funciona. A ilusão de magia se dissolve em compreensão prática.

## Chopping vs. big spec

A observação mais prática para usuários de AI no desenvolvimento: os clientes mais bem-sucedidos **quebram as tarefas em pedaços pequenos**.

Dois padrões opostos:
1. **Big spec:** especifique tudo de uma vez → AI trabalha em background → revise o output completo → aprove ou rejeite. Parece eficiente, frequentemente desaponta.
2. **Chopping:** especifique um pouco → AI gera um pedaço → revise → especifique mais → repita. Mais lento por iteração, muito melhor no resultado total.

O tempo total de especificação pode ser o mesmo nos dois casos. O que muda é a capacidade de corrigir curso a cada iteração. Com big spec, um mal-entendido inicial contamina todo o output. Com chopping, você corrige no primeiro passo.

## Cursor como caso de origem

Em 5 semanas após começar a construir, o time do Cursor já havia abandonado o editor anterior e estava usando a própria ferramenta em tempo integral. O produto foi ao público em 3 meses depois da primeira linha de código — não por estar "pronto", mas por estar suficientemente útil para colher feedback real.

O feedback inicial dos usuários mudou uma decisão fundamental: abandonar o editor feito do zero e migrar para uma base VS Code. Essa sensibilidade ao feedback real (que só vem quando você coloca o produto em uso genuíno) é o que o dogfooding torna possível.

## Implicação para produtos de IA

Para produtos de AI especificamente: cada nova versão de modelo muda o que é possível. O "gut feeling" para o que o modelo pode fazer precisa ser recalibrado a cada salto de capacidade. Times que não usam o produto ativamente ficam presos com calibração desatualizada.

Implicação de contratação: os engenheiros e pesquisadores mais valiosos são aqueles que usam a ferramenta ativamente e que se importam visceralmente com a qualidade da experiência — não apenas com as métricas de benchmark.

## Insights por autor
### [[Michael Truell]]
- "We never wanted to ship anything that wasn't useful to us, and we had the benefit of that because we were the end users."
- "After five weeks, we were living on the editor full-time and had thrown away our previous editor."
- "There's an instinct to anthropomorphize these models — it's magical here, so it must be magical there. But these things have massive issues."
- "The most successful customers chop things up. Specify a little, get a little work, review, specify a little more. Not the giant spec handed to the model."
- "Explicitly try to fall on your face in a safe environment — discover the limits of what AI can do. You might be surprised in some places where the model doesn't break."

> 🎧 [The rise of Cursor: The $300M ARR AI tool that engineers can't stop using | Michael Truell](https://www.youtube.com/watch?v=En5cSXgGvZM)

## Conceitos relacionados
[[Falha Conclusiva — Design de Experimento Definitivo]] · [[CC-CD — Calibração Contínua, Desenvolvimento Contínuo]] · [[Prototipagem antes de Modelo — IA Fora do MVP]] · [[O Mundo Depois do Código — Engenheiro como Designer de Lógica]]
