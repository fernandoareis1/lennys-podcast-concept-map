---
tipo: framework
nivel: 3
fluxo: Design & UX
autores:
  - Gustav Söderström
---
# 🏠 Recall vs. Discovery — A Dicotomia da Homepage

**Fluxo:** [[04 - Design & UX]] · **Tema:** [[Design — Experiência & fricção]] · **Camada:** L3 (Conceito)

**Autor:** [[Gustav Söderström]]

---

## A ideia central

Qualquer homepage de produto de conteúdo serve dois trabalhos radicalmente diferentes para o usuário:

- **Recall** — "quero voltar ao que já conheço": minha playlist favorita, o podcast que parei no episódio 3, a série que estou assistindo
- **Discovery** — "quero encontrar algo novo que eu não sabia que existia"

O erro clássico de produto é redesenhar a homepage sem entender qual dos dois trabalhos domina no momento atual dos seus usuários.

## O erro do Spotify com a Home

O Spotify redesenhou a Home para favorecer discovery — feed único de itens novos, layout tipo TikTok. Os tweets raivosos começaram a chegar em massa. O instinto do time era "os usuários odeiam novidade" ou "são conservadores com mudança".

A análise quantitativa revelou outra coisa: os usuários vinham à Home **90% para recall** e **10% para discovery**. O redesign inverteu para 10/90.

> "What we misjudged was that the way our homepage works, it is almost 90% what we call recall... when we tested the design, we switched it from 90/10 to 10/90." — Gustav Söderström

O sinal estava nos dados de comportamento: o tráfego migrou massivamente de Home → Search e Home → Library. Os usuários não estavam reclamando de mudança — estavam contornando a remoção da funcionalidade de que mais dependiam.

## Dense UI vs. Feed UI

Os dois modos de uso pedem arquiteturas de informação opostas:

| Recall | Discovery |
|--------|-----------|
| UI densa (grade, lista) | Feed único (scroll vertical) |
| Você sabe o que procura | Você não sabe o que quer |
| Ícones menores, mais itens | Imagens grandes, um item por vez |
| Encontrabilidade > surpresa | Surpresa > encontrabilidade |

O Netflix Home é densa para recall. O TikTok é feed para discovery. O erro é usar a arquitetura errada para o trabalho dominante.

## Como diagnosticar o split no seu produto

1. **Meça o fluxo de entrada**: como os usuários chegam à sessão? Via notificação (recall) ou browsing (discovery)?
2. **Meça saídas do redesign**: Search e Library aumentaram? → você cortou recall
3. **Separe coortes**: novos usuários vs. usuários antigos têm splits diferentes. Novos têm mais discovery; veteranos têm mais recall
4. **Não confunda "hábito perturbado" com "design ruim"**: qualquer redesign gera queda temporária de métricas. Olhe a tendência a 60-90 dias

## Redesigns são diferentes de features

Söderström aponta uma assimetria importante: adicionar uma feature é voluntário (o usuário pode ignorar). Redesenhar a interface é **participação involuntária** — todo usuário é afetado imediatamente. O custo de errar é ordens de magnitude maior.

## Conceitos relacionados
- [[UI Tolerante a Falhas — Projetar para a Performance do ML]] — a UI certa depende do que o usuário veio fazer
- [[Preferências declaradas vs. reveladas]] — tweets raivosos ≠ dado; comportamento de navegação = dado
- [[Experience Map]] — mapear os momentos distintos da experiência revela qual trabalho domina
