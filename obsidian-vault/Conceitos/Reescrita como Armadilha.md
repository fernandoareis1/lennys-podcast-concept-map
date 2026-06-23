---
tipo: insight
nivel: 3
fluxo: Priorização & Roadmap
autores: [Camille Fournier]
---
# Reescrita como Armadilha
**Fluxo:** [[03 - Priorização & Roadmap]] · **Tema:** [[Priorização — Estratégia vs execução]] · **Camada:** L3
**Tipo:** Insight · **Fontes:** [[Camille Fournier]]

## Ideia central
Rewrites completos raramente entregam o que prometem. Engenheiros subestimam drasticamente o tempo de migração do sistema antigo para o novo, o conhecimento enterrado no sistema legado (regras de negócio não documentadas, edge cases, formatação de dados), e o custo de manter o sistema antigo enquanto o novo é construído em paralelo.

A alternativa é uma evolução incremental e faseada: identificar as partes críticas que precisam de uplift, encapsulá-las como APIs bem definidas, e melhorar peça a peça — sem congelar o produto por meses ou anos.

Se o sistema funciona bem o suficiente e não precisa de novas funcionalidades, a pergunta honesta é: vale a pena reescrever algo que você poderia não tocar por anos sem prejudicar o negócio?

## Como aplicar
1. **Teste de congelamento**: pergunte "se não tocarmos nesse sistema por 2 anos, o negócio sofre?" — se não, questione a urgência do rewrite.
2. **Estime migração separadamente**: force um estimate explícito para migração de dados, clientes e APIs — normalmente é o maior gargalo.
3. **Isole, não substitua tudo**: identifique a parte que mais trava entregas e proponha um uplift desse módulo específico (API-first).
4. **Documente o que o sistema atual faz** antes de qualquer refatoração — regras de negócio ocultas se perdem na tradução.
5. **Mantenha entrega contínua**: recuse propostas que congelam feature development por mais de 4–6 semanas sem resultado tangível visível.

## Insights por autor
### [[Camille Fournier]]
- "Engenheiros massivamente subestimam o tempo de migração do sistema antigo para o novo — e isso causa problemas enormes."
- "Você ainda tem que suportar o sistema antigo enquanto trabalha no novo. Isso é infuriante para quem está esperando por features."
- "Há tanta lógica enterrada em sistemas legados — não documentada, estranha. É muito mais difícil replicar o que importa do que as pessoas esperam."
- "Se você pudesse não tocar naquilo por muito tempo sem prejudicar o negócio, vale a pena trocar?"

## Conceitos relacionados
[[Priorização — Estratégia vs execução]] · [[Engenheiros no Loop Criativo]] · [[Gestão como Serviço — não Comando]]
