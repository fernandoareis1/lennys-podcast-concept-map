---
tipo: framework
nivel: 3
fluxo: Experimentação & Dados
autores: [Aishwarya Naresh Reganti, Kiriti Badam]
---
# Evals vs. Monitoramento em Produção
**Fluxo:** [[05 - Experimentação & Dados]] · **Tema:** [[Experimentação — AB testing & cultura]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Aishwarya Naresh Reganti]], [[Kiriti Badam]]

## Ideia central
Há uma falsa dicotomia no campo de IA: ou "evals resolvem tudo" ou "monitoramento em produção resolve tudo". **Evals** (datasets de avaliação estruturados) capturam apenas os erros *que você já conhece* — são construídos com o conhecimento atual do produto. **Monitoramento em produção** captura padrões emergentes do comportamento real de usuários que você não antecipou. Ambos são necessários e complementares; a ênfase relativa depende do volume e do tipo de aplicação.

## Como aplicar
1. **Evals:** construa um dataset de casos que o produto jamais deve errar, independentemente de mudanças. Use para verificar se mudanças de modelo/prompt não regridem comportamentos críticos.
2. **Monitoramento:** colete sinais implícitos (regenerar resposta, abandonar fluxo) e explícitos (thumbs up/down) para detectar padrões novos.
3. Em alto volume: impossível auditar todos os traces — use sinais de produção para priorizar o que revisar manualmente.
4. Só crie novos critérios de avaliação quando um padrão emergente for recorrente e importante — erros pontuais de ferramenta podem ser corrigidos sem criar um eval.
5. Cuidado com "semantic diffusion" do termo: benchmarks públicos ≠ product evals; LLM judge ≠ dataset de erro humano. Defina o que você quer dizer internamente.

## Insights por autor
### [[Aishwarya Naresh Reganti]]
- Analogia com "semantic diffusion" (Martin Fowler): "evals" significa coisas diferentes para data labelers, PMs e engenheiros — a confusão de terminologia paralisa times.
- Empresas que checam apenas benchmarks públicos (LMArena, Artificial Analysis) pensando que "estão fazendo evals" estão erradas: esses são *model evals*, não *product evals*.
- "A questão real: você quer um feedback loop acionável para seu produto de IA. Como você o constrói depende inteiramente do seu contexto."

### [[Kiriti Badam]]
- No Codex (OpenAI): "evals + monitoramento em produção + um pouco de vibes. Cada engenheiro tem sua lista pessoal de problemas difíceis que joga contra cada novo modelo."
- Sinal forte de produção: se usuários desligam uma feature após mudança de modelo, nenhum eval pré-deploy captura isso.
- "Se você tiver um conjunto concreto de evals no qual confia totalmente e achar que não precisa de mais nada, não vai funcionar."

> 🎧 [Why most AI products fail: Lessons from 50+ AI deployments at OpenAI, Google & Amazon (1:26:22)](https://www.youtube.com/watch?v=z7T1pCxgvlA)

## Conceitos relacionados
[[Framework CCCD]] · [[Não-determinismo em Produtos de IA]] · [[A-B Testing (Ronny Kohavi)]] · [[OEC - Overall Evaluation Criterion]]
