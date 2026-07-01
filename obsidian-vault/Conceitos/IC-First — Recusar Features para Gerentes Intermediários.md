---
tipo: framework
nivel: 3
fluxo: Estratégia & Visão
autores: [Nan Yu]
---
# IC-First — Recusar Features para Gerentes Intermediários
**Fluxo:** [[02 - Estratégia & Visão]] · **Tema:** [[Estratégia — Estratégia de produto]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Nan Yu]]

## Ideia central
O Linear tem uma política explícita: recusar qualquer feature que beneficie gerentes intermediários (reporting customizável, campos obrigatórios, dashboards de controle) à custa da experiência do IC (Individual Contributor). Os ICs são quem realmente usa o software diariamente — se eles desengajam, os dados de reporting ficam inúteis de qualquer forma. Esse mecanismo evita o inchaço inevitável que torna software empresarial horrível de usar.

## Como aplicar
- Mapeie cada solicitação de feature: quem se beneficia — o executor do trabalho ou quem reporta sobre o trabalho?
- Crie uma regra clara: features que piorem o workflow do IC para facilitar reporting de gestores são automaticamente rejeitadas
- Mostre o ciclo vicioso para convencer vendas: campos obrigatórios → ICs escolhem valores aleatórios → dados de reporting ficam incorretos → reporting torna-se inútil de qualquer forma
- Foque nos 3 primeiros itens da lista de pedidos do cliente, não nos 10 — negocie o restante

## Insights por autor
### [[Nan Yu]]
- "The stuff that we absolutely have to say no to is the exact kind of thing that leads to this bloatedness that makes ICs hate their lives — customization features requested by middle managers to make reporting easier at the cost of making IC workflows worse."
- O exemplo de Customer Requests ilustra a solução certa: resolver a necessidade real do gestor (rastrear pedidos por empresa) via integração automática com CRM — sem criar atrito para o IC.
- A regra IC-First é o mecanismo que permite ao Linear crescer em enterprise sem perder a experiência que conquistou os ICs no início.
> 🎧 [Linear's Head of Product on building faster (1:21:08)](https://www.youtube.com/watch?v=nTr21kgCFF4) · 2024

## Conceitos relacionados
[[Velocidade e Qualidade Não São Trade-offs]] · [[DHM Model]] · [[Produto lovável (MLP)]]
