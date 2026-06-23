---
tipo: framework
nivel: 3
fluxo: Estratégia & Visão
autores: [Brandon Chu]
---
# PM de plataforma — princípios e ciclos
**Fluxo:** [[02 - Estratégia & Visão]] · **Tema:** [[Estratégia — Estratégia de produto]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Brandon Chu]]

## Ideia central
Ser PM de plataforma é radicalmente diferente de ser PM de produto de consumo. Você não está desenhando a experiência do usuário final — está **desenhando o canvas** sobre o qual outros vão construir as experiências. Isso muda tudo: os ciclos de feedback, a validação, os trade-offs e a psicologia necessária.

**Diferenças fundamentais:**

| Dimensão | PM de Produto | PM de Plataforma |
|---|---|---|
| Ciclo de feedback | Semanas | Anos (5-10x mais longo) |
| Quem define a UX | Você | Desenvolvedores que constroem sobre você |
| O que você valida | Feature → usuário final | API → alpha dev → beta → produto final → usuário |
| Celebrações | Cada lançamento | Cada etapa do ciclo (API em alpha = marco) |

**Princípios de plataforma e stack-rank de constituintes:**
Toda plataforma serve múltiplos stakeholders. A decisão mais crítica é definir **quem vence quando há conflito**:
- **Amazon**: em caso de conflito, o consumidor vence sobre o vendedor. Efeito colateral: vendedores frustrados.
- **Shopify**: em caso de conflito, o empreendedor/merchant vence sobre o desenvolvedor de apps. Efeito colateral: devs sacrificam dados às vezes.

Sem esses princípios explícitos, cada decisão de política ou design vira um impasse. Com eles, as equipes resolvem conflitos sem escalar.

**Psicologia necessária:**
- Aceitar que a validação demora anos — o PM precisa celebrar marcos intermediários (alpha de API, primeiros devs adotando) como se fossem lançamentos.
- Contar a narrativa maior para o time: "isso vai mudar como merchants acessam apps" — sem isso, o time perde a motivação em ciclos longos.

## Insights por autor
### [[Brandon Chu]]
- "Você não está desenhando a experiência do usuário final. Você está desenhando um canvas para que desenvolvedores construam suas próprias ideias criativas. É um tipo de trabalho completamente diferente."
- "Os ciclos são 5 a 10 vezes mais longos. Quando a API foi para alpha, não há press release. Como você faz o time se sentir incrível por aquele trabalho?"
- "Em Shopify, se há trade-off entre merchant e developer, optamos pelo merchant. É importante que o merchant tenha acesso a esse dado mesmo que isso prejudique o developer."
- "Oscilar entre plataforma e consumer é a experiência ideal, porque cada um te ensina algo que o outro não consegue."

> 🎧 Episódio com Brandon Chu, VP de Produto na Shopify (frontmatter do transcript com erro — URL não disponível)

## Conceitos relacionados
[[Liquidez do marketplace]] · [[Filtros que fragmentam supply]] · [[Empowered Teams vs Feature Teams]] · [[Single-Threaded Leader]]
