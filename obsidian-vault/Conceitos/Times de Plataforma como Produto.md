---
tipo: framework
nivel: 3
fluxo: Liderança & Times
autores: [Camille Fournier]
---
# Times de Plataforma como Produto
**Fluxo:** [[09 - Liderança & Times]] · **Tema:** [[Liderança — Modelos de time]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Camille Fournier]]

## Ideia central
Times de plataforma não são "SRE v2" nem apenas manutenção de infraestrutura. Plataformas são produtos — com usuários internos reais, problemas de discovery, e necessidade de PMs dedicados. A função de um time de plataforma é gerenciar a complexidade sistêmica e entregar alavancagem ao negócio: reduzir cycle time, resolver gargalos que impedem launches, fazer reduções de custo mensuráveis.

Para funcionar, times de plataforma precisam de três perfis: engenheiros de software (para construir offerings coerentes), engenheiros de sistemas/SRE (para operational excellence), e product managers (para orientação por impacto, não por tecnologia cool).

O sinal para criar um time de plataforma: acima de ~50 engenheiros, quando você vê os mesmos perfis resolvendo os mesmos problemas em múltiplos times — centralizar faz sentido de custo e eficiência.

## Como aplicar
1. **Defina métricas de impacto**: cycle time de engenharia, número de launches desbloqueados, reduções de custo — não "estamos rodando no Kubernetes".
2. **Adicione PMs ao time de plataforma**: sem produto, engenheiros constroem o que parece interessante tecnicamente, não o que resolve problemas reais dos times internos.
3. **Trate stakeholders como clientes**: adote práticas de discovery interno — entrevistas com times que usam a plataforma, priorização baseada em impacto, não em voz mais alta.
4. **Espere o momento certo para criar**: com menos de 50 engenheiros, a coordenação ad hoc funciona melhor; formalize quando a ineficiência se tornar visível.
5. **Aceite que migração é parte do trabalho**: cloud providers evoluem, versões deprecam — planejar migrações suaves para os times consumidores é core job de plataforma.

## Insights por autor
### [[Camille Fournier]]
- "Plataformas são produtos. Você precisa pensar em como criar offerings coerentes que tornem a empresa mais produtiva."
- "Muitas empresas simplesmente não acreditam que deveriam 'desperdiçar' headcount com PMs para times internos — e aí você tem engenheiros inteligentes construindo o que parece certo sem saber o que construir."
- "Platform engineering não é só manter infraestrutura cloud e fazer scripts pequenos. Isso não cria uma plataforma coesa e coerente."
- "Um sinal claro: quando você vê as mesmas pessoas em cada time tendo que resolver os mesmos tipos de problema. Por que tenho três pessoas em cada time lidando com isso em vez de centralizar?"

## Conceitos relacionados
[[PM de plataforma — princípios e ciclos]] · [[Liderança — Modelos de time]] · [[Single-Threaded Leader]] · [[Empowered Teams vs Feature Teams]]
