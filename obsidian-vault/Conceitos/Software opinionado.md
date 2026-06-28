---
tipo: insight
nivel: 3
fluxo: Estratégia & Visão
autores: [Barbra Gago, Karri Saarinen]
---
# Software opinionado
**Fluxo:** [[02 - Estratégia & Visão]] · **Tema:** [[Estratégia — Estratégia de produto]] · **Camada:** L3
**Tipo:** Insight · **Fontes:** [[Barbra Gago]] · [[Karri Saarinen]]

## Ideia central
Software opinionado tem **melhores práticas ou regras embutidas no produto** — o sistema força uma certa forma de trabalhar e não permite desvios arbitrários. O oposto é software maximamente customizável onde o usuário decide tudo.

Há dois modelos para construir software opinionado:
1. **Encode a prática que já existe**: o mercado já adotou uma metodologia (ex.: agile) mas não tem tooling. O produto vira a implementação técnica do processo. Atlassian com Jira é o exemplo canônico.
2. **Ensine uma forma melhor**: a prática atual tem problemas conhecidos (viés, opacidade, inconsistência). O produto obriga o usuário a fazer de forma diferente e justifica o porquê. Greenhouse com "structured recruiting" é o exemplo — o sistema exigia kit de entrevista padronizado, níveis definidos, pipeline explícito.

O tradeoff é claro: software opinionado cria **defensibilidade e diferenciação** (não dá para fazer o mesmo no Excel), mas limita a flexibilidade. Clientes que precisam do oposto não vão comprar.

## Como aplicar
1. **Identifique onde subjetividade gera danos**: se a decisão mais comum é também a mais enviesada (ex.: quem promover, quem contratar), o produto pode e deve forçar estrutura.
2. **Escolha o modelo**: você vai codificar uma prática emergente já existente (mais rápido para adoção) ou ensinar uma prática melhor (mais difícil de vender, maior impacto)?
3. **Mostre o "porquê" da regra no produto**: quando o software força algo, o usuário precisa entender por quê. Se a UI não explica a razão da restrição, o usuário sente frustração, não ganho.
4. **Aceite a perda de leads**: software opinionado afasta quem quer flexibilidade máxima. Isso é sinal saudável de ICP, não bug.
5. **Use como diferenciador no pitch**: "Nosso sistema não deixa você fazer X porque X causa Y problema" é uma proposta de valor mais forte que "nós também fazemos X".

## Insights por autor
### [[Barbra Gago]]
- "Greenhouse: havia uma forma específica de criar um pipeline, um interview kit — tudo isso era importante porque tornava o recrutamento melhor, mais transparente e menos enviesado."
- "Atlassian construiu em torno de um processo que já estava crescendo e ganhou momentum. O produto virou a solução tecnológica para uma prática que já existia."
- "Com Greenhouse, foi diferente: havia uma forma melhor de fazer e é assim que deve ser feito — nosso software te ajuda a fazer isso."
- Sobre Pando: "Empresas que consertam gaps de compensação anualmente não estão resolvendo o problema sistêmico. O produto cria accountability em ambos os lados — gestor e funcionário — porque sem sistema isso é subjetivo demais."
> 🎧 [Category creation and brand building (55:48)](https://www.youtube.com/watch?v=gCEaUfZUuI0) · 2022-10-27

### [[Karri Saarinen]]
- "Há sempre aquela tensão entre fazer algo para todos vs. fazer algo para alguém. E acredito muito em criar algo para alguém — uma empresa ou equipe específica — e torná-lo o melhor possível para esse caso de uso."
- O Linear Method é a visão opinionada da Linear sobre como o desenvolvimento de software deve funcionar: ciclos de duas semanas, issues atômicas, escritas como tarefas, sem backlogs infinitos.
- Bons defaults eliminam decisões de configuração: o usuário entra no fluxo de trabalho sem precisar montar a ferramenta.
- "Quando eu crio algo para um produto de produtividade, ele deve te dizer como trabalhar — não deixar você escolher tudo."
> 🎧 [Inside Linear: Building with taste, craft, and focus](https://www.youtube.com/watch?v=4muxFVZ4XfM) · 2023-10-08

## Conceitos relacionados
[[Diferente E melhor E relevante]] · [[DHM Model]] · [[Empowered Teams vs Feature Teams]] · [[Pain is the New Moat]]
