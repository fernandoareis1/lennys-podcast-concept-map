---
tipo: framework
nivel: 3
fluxo: Estratégia & Visão
autores: [Aishwarya Naresh Reganti, Kiriti Badam]
---
# Escada de Agência-Controle em IA
**Fluxo:** [[02 - Estratégia & Visão]] · **Tema:** [[Estratégia — Estratégia de produto]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Aishwarya Naresh Reganti]], [[Kiriti Badam]]

## Ideia central
Não entregue autonomia total à IA no dia 1. Construa confiança progressivamente: cada versão do produto aumenta a agência da IA e reduz o controle humano **somente depois** de coletar evidências de confiabilidade. A escada de agência-controle é o principal antídoto contra erosão de confiança do usuário e decisões perigosas de agentes.

## Como aplicar
Para cada caso de uso, defina 3 versões progressivas:
- **V1 — Alto controle, baixa agência:** IA só sugere; humano decide e executa. O log do comportamento humano gera análise de erros de graça.
- **V2 — Controle médio, agência média:** IA gera rascunho; humano aprova ou edita antes de agir.
- **V3 — Baixo controle, alta agência:** IA age autonomamente em casos de baixo risco; humanos monitoram.

**Critério para subir de nível:** quando você parar de ver novos padrões de dados e o comportamento dos usuários estabilizar. Não existe regra quantitativa universal — é calibração qualitativa.

Nota: eventos externos (nova versão de modelo, mudança de comportamento do usuário) podem reverter o nível — recalibre.

## Insights por autor
### [[Aishwarya Naresh Reganti]]
- Exemplo clínico: pré-autorização de exame de sangue → IA pode decidir (baixo risco). Cirurgia invasiva → humano decide (alto risco). Você define quais casos estão em cada faixa.
- "A ideia maior é calibração de comportamento. É quase impossível prever como o sistema vai se comportar — então você não arranha a experiência do usuário enquanto calibra."
- Air Canada: agente alucionou uma política de reembolso não existente; a empresa foi obrigada a cumpri-la legalmente. Resultado de pular a escada de agência-controle.
- Logging de V1/V2: "Você registra o que o humano faria. Isso vira flywheel de melhoria contínua do sistema."

### [[Kiriti Badam]]
- Exemplo suporte (OpenAI): V1 = classificar e rotear ticket; V2 = gerar rascunho de resposta (copiloto); V3 = resolver o ticket de ponta a ponta autônomamente.
- "Se você for direto para o V3, terá 100 tipos de erro simultâneos e não conseguirá consertar nenhum."
- Dados bagunçados (taxonomias duplicadas, regras não documentadas) aparecem em V1 — é muito mais fácil de corrigir ali do que num agente autônomo de múltiplas etapas.

> 🎧 [Why most AI products fail | Aishwarya + Kiriti (1:26:22)](https://www.youtube.com/watch?v=z7T1pCxgvlA)

## Conceitos relacionados
[[Não-Determinismo em Produtos de IA]] · [[CC — Calibração e Desenvolvimento Contínuo]] · [[Empowered Teams vs Feature Teams]] · [[Roadmap como momentos de struggle]]
