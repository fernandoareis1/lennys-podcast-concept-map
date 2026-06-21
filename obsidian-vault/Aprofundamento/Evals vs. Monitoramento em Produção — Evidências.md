---
tipo: aprofundamento
nivel: 4
fluxo: Experimentação & Dados
conceito_pai: Evals vs. Monitoramento em Produção
autores: [Aishwarya Naresh Reganti, Kiriti Badam, Alexander Embiricos]
---
# 📜 Evals vs. Monitoramento em Produção — Evidências

**↑ Card:** [[Evals vs. Monitoramento em Produção]] · **Tema:** [[Experimentação — AB testing & cultura]] · **Camada:** L4 (Aprofundamento)
**Fontes:** [[Aishwarya Naresh Reganti]], [[Kiriti Badam]], [[Alexander Embiricos]]

> Três perspectivas complementares: consultoras com 50+ deployments, engenheiro de ML da OpenAI, e product lead do Codex. Versão condensada no [[Evals vs. Monitoramento em Produção|card]].

---

## O problema que evals sozinhos não resolvem

Quando times de produto começam a construir com LLMs, a primeira intuição é: "precisamos de evals". Mas a palavra "eval" esconde uma ambiguidade perigosa. **Aishwarya Naresh Reganti** chama isso de *semantic diffusion* — o mesmo termo significa coisas opostas dependendo de quem está na sala:

- Para um data labeler: um conjunto de pares input/output que os humanos classificam manualmente
- Para um engenheiro de ML: um benchmark automatizado com LLM-as-judge
- Para um PM: qualquer métrica que diga se o produto está funcionando
- Para um executivo: os rankings públicos (LMArena, Artificial Analysis)

> "Empresas que checam apenas benchmarks públicos pensando que 'estão fazendo evals' estão erradas: esses são *model evals*, não *product evals*. A questão real é: você quer um feedback loop acionável para seu produto de IA. Como você o constrói depende inteiramente do seu contexto."

O diagnóstico de Aishwarya, depois de analisar 50+ deployments em OpenAI, Google e Amazon, é que essa confusão de terminologia paralisa times. Discutem se "evals" são suficientes quando na verdade nem definiram do que estão falando.

---

## O modelo da OpenAI: evals + monitoramento + vibes

**Kiriti Badam**, engenheiro de ML que trabalhou no Codex antes de se tornar consultor, descreve o stack real que times sofisticados usam na prática:

> "No Codex (OpenAI): evals + monitoramento em produção + um pouco de vibes. Cada engenheiro tem sua lista pessoal de problemas difíceis que joga contra cada novo modelo."

Essa "lista pessoal" é reveladora. Em uma organização com dezenas de engenheiros, existem dezenas de conjuntos informais de casos de teste — bugs impossíveis que cada person acumulou ao longo de anos. Esses casos são complementares aos evals formais porque capturam a cauda longa do que o produto precisa fazer.

O sinal mais forte de produção que Kiriti identifica é comportamental:

> "Se usuários desligam uma feature após mudança de modelo, nenhum eval pré-deploy captura isso."

Evals são construídos com o conhecimento atual — capturam os erros que você já conhece. Monitoramento captura os padrões que surgem do comportamento real, que você não antecipou. Os dois são complementares, não substitutos.

A limitação de evals fica evidente em escala:

> "Se você tiver um conjunto concreto de evals no qual confia totalmente e achar que não precisa de mais nada, não vai funcionar."

O motivo: o espaço de inputs de usuários reais é impossível de cobrir com antecedência. Usuários encontram modos de usar o produto que o time nunca imaginou — e os evals não capturam o que você não imaginou.

---

## A perspectiva do PM do Codex: Reddit como sinal de produção

**Alexander Embiricos**, product lead do Codex na OpenAI, traz uma perspectiva complementar que vem de quem decide o roadmap, não de quem constrói os evals técnicos.

Quando Lenny perguntou sobre evals e benchmarks públicos, Embiricos começou pela retenção:

> "Uma das coisas que estou constantemente me lembrando é que o Codex naturalmente é uma ferramenta que você se torna power user. Então podemos acabar gastando muito tempo pensando em features muito profundas na jornada de adoção. É criticamente importante ir ver o D7 retention. Simplesmente ir usar o produto, se inscrever do zero de novo."

A métrica de D7 retention como âncora revela algo importante: para um produto de agente de IA, a questão mais fundamental não é "o modelo está correto?" mas "os usuários voltam?". A acurácia do modelo importa apenas na medida em que gera retenção.

Mas a insight mais original de Embiricos é sobre **social listening diferenciado por plataforma**:

> "Alguns de nós ficam constantemente no Reddit e no Twitter. Tem elogios e tem muitas reclamações. Levamos as reclamações muito a sério. Para o Twitter/X, é um pouco mais hype. Já o Reddit é um pouco mais negativo, mas real. Tenho prestado cada vez mais atenção em como as pessoas estão falando sobre Codex no Reddit."

A distinção Twitter vs. Reddit é um framework de sinal/ruído que qualquer PM de produto de IA pode usar:
- **Twitter/X**: alta visibilidade, hype elevado, influencers com audiência; bom para detectar zeitgeist, ruim para problemas reais
- **Reddit**: upvotes como agregação de opinião, audiência de usuários reais; boa mecânica de filtragem do que importa vs. reclamações isoladas

Esse monitoramento de "vibes" não é vago — é complementar ao D7 retention porque captura a *qualidade* percebida de uma forma que métricas de engajamento não capturam.

---

## O padrão convergente: três camadas de feedback

Consolidando as três perspectivas, emerge um stack de medição para produtos de IA com três camadas complementares:

**Camada 1 — Evals estruturados** (Aishwarya & Kiriti)
- Dataset de casos críticos que o produto *jamais* pode errar
- Atualizado quando padrões emergentes de produção se tornam recorrentes
- Distintos de benchmarks públicos (que medem o modelo, não o produto)

**Camada 2 — Monitoramento comportamental** (Kiriti & Alexander)
- Sinais implícitos: regenerar resposta, abandonar fluxo, desativar feature
- Sinais explícitos: thumbs up/down, ratings
- Em alto volume: monitore sinais para priorizar revisão manual, não para substituí-la

**Camada 3 — Social listening + retenção** (Alexander)
- D7 retention como indicador de saúde fundamental
- Reddit como sinal de problemas reais com boa mecânica de filtragem
- "Vibes" como proxy de qualidade percebida que métricas brutas não capturam

---

## Quando criar um eval vs. quando monitorar

A heurística prática de Kiriti Badam:

> "Só crie novos critérios de avaliação quando um padrão emergente for recorrente e importante — erros pontuais de ferramenta podem ser corrigidos sem criar um eval."

O fluxo: monitoramento detecta padrão emergente → pattern se confirma como recorrente → novo caso é adicionado ao eval → eval vira guardrail para releases futuros. O monitoramento alimenta os evals, não os substitui.

---

## Conceitos ligados
[[Não-determinismo em Produtos de IA]] · [[Framework CCCD]] · [[Validação como Gargalo de Agentes]] · [[A-B Testing (Ronny Kohavi)]] · [[OEC - Overall Evaluation Criterion]] · [[Agente de IA como Colega de Time]]
