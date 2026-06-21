---
tipo: framework
nivel: 3
fluxo: Experimentação & Dados
autores: [Aishwarya Naresh Reganti, Kiriti Badam]
---
# CC — Calibração e Desenvolvimento Contínuo
**Fluxo:** [[05 - Experimentação & Dados]] · **Tema:** [[Experimentação — AB testing & cultura]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Aishwarya Naresh Reganti]], [[Kiriti Badam]]

## Ideia central
O **CC/CD** (Continuous Calibration / Continuous Development) é o ciclo de vida de desenvolvimento específico para produtos de IA — análogo ao CI/CD do software tradicional, mas com uma etapa a mais: calibração contínua do comportamento emergente em produção. A diferença crítica: evals capturam apenas erros **antecipados**; produção revela padrões que você não imaginou. Ambos são necessários.

## Como aplicar
**Loop de Desenvolvimento Contínuo:**
1. Escopar capacidade e curar dataset pequeno com inputs esperados e outputs desejados.
2. Configurar aplicação e definir métricas de avaliação específicas (não genéricas).
3. Deploy e execução das métricas.

**Loop de Calibração Contínua:**
4. Analisar comportamentos emergentes via sinais implícitos (regeneração de resposta, thumbs down, edições do humano) e explícitos (feedback).
5. Identificar padrões de erro não previstos.
6. Aplicar correções (algumas não precisam de nova eval; outras exigem expandir o dataset).
7. Atualizar métricas de avaliação para capturar os novos padrões descobertos.
8. Subir de nível de agência (ver [[Escada de Agência-Controle em IA]]) somente quando a calibração estabilizar.

## Insights por autor
### [[Aishwarya Naresh Reganti]]
- "Evals capturam apenas os erros que você já antecipou. Produção é onde você descobre o que não imaginou — por isso calibração contínua é insubstituível."
- Sobre *semantic diffusion* do termo "evals": data labeling companies, PMs e engenheiros de ML usam "evals" com significados radicalmente diferentes. O que importa é o ciclo de feedback acionável, não o nome.
- "Se alguém te vende 'agentes em um clique que mostram ganhos em 3 dias', desconfie. Até substituir um workflow crítico com ROI real leva 4–6 meses, mesmo com boa infraestrutura."
- O loop de desenvolvimento também alinha o time: antes de construir, todos precisam concordar com "o que o produto deve fazer" — e isso frequentemente revela desacordos escondidos.

### [[Kiriti Badam]]
- "No Codex (OpenAI) usamos evals para garantir que mudanças não quebram o core, mas também monitoramos sinais de clientes — feedback em redes sociais, regeneração de resposta, A/B test de mudança de modelo."
- "Produção monitoring vs evals: não há razão para confiar em um extremo só. São ferramentas complementares."
- Sinais implícitos no Codex: se o usuário desativa o produto de code review após uma mudança de modelo, isso é sinal claro de regressão — mesmo sem eval explícita para aquele caso.

> 🎧 [Why most AI products fail | Aishwarya + Kiriti (1:26:22)](https://www.youtube.com/watch?v=z7T1pCxgvlA)

## Conceitos relacionados
[[Não-Determinismo em Produtos de IA]] · [[Escada de Agência-Controle em IA]] · [[A maioria das ideias falha no teste]] · [[A-B Testing (Ronny Kohavi)]] · [[Decidir com poucos dados é melhor que com zero]]
