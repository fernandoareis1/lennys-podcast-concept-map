---
tipo: tecnica
nivel: 3
fluxo: Discovery & Pesquisa
autores: [Adriel Frederick]
---
# Usuário Marginal
**Fluxo:** [[01 - Discovery & Pesquisa]] · **Tema:** [[Discovery — Entrevistar usuários]] · **Camada:** L3
**Tipo:** técnica · **Fontes:** [[Adriel Frederick]]

## Ideia central
O usuário marginal é quem está **na borda da ação**: chegou ao produto (tráfego existe), mas não converte, não retém, não executa a ação-chave. Focar nesse perfil — em especial no pior caso — revela o máximo de fricções. Os dados mostram *onde* estão, mas apenas a observação direta mostra *por quê* não chegam.

## Como aplicar
1. **Identifique com dados:** encontre país/segmento com alto tráfego e baixa conversão — esse é o cluster do usuário marginal.
2. **Vá ao caso extremo:** procure o pior cenário (feature phone, EDGE, fuso horário distante, idioma não-tratado). Isso mostra *tudo* que está errado.
3. **Remova constraints impossíveis:** depois de ver o caso extremo, remova as barreiras difíceis de atacar (ex.: latência de datacenter) e veja o que resta — esses são os problemas priorizáveis.
4. **Observe, não só analise:** funil de dados diz "taxa de drop em step 3", mas só observação diz "o usuário usa o nome legal que ninguém conhece no mundo real".
5. **Use para priorizar:** o marginal user define o que fazer a seguir; o pior caso define o backlog completo.

## Insights por autor
### [[Adriel Frederick]]
- No Facebook: vendo alguém se cadastrar na Índia, percebeu que o nome legal inserido faria com que pedidos de amizade ficassem sem resposta — um bug que nenhum funil revelaria.
- "Don't use data alone to figure out who the marginal user is. It'll give you a clue, not the answer. You have to go watch them."
- Signup com telefone e SMS como "cannonball" no Facebook: descoberto ao ir ao encontro dos usuários marginais fora dos EUA.
> 🎧 [Humanizing product development (1:07:26)](https://www.youtube.com/watch?v=uMhBej6-Ey4)

## Conceitos relacionados
[[Entrevista baseada em história]] · [[Continuous Discovery]] · [[Discovery — Entrevistar usuários]]
