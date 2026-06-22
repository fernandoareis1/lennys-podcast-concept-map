---
tipo: framework
nivel: 3
fluxo: Experimentação & Dados
autores: [Aishwarya Naresh Reganti, Kiriti Badam]
---
# CCCD — Calibração e Desenvolvimento Contínuos
**Fluxo:** [[05 - Experimentação & Dados]] · **Tema:** [[Experimentação — AB testing & cultura]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Aishwarya Naresh Reganti]], [[Kiriti Badam]]

## Ideia central
CCCD (Continuous Calibration / Continuous Development) é o ciclo de vida iterativo adequado para produtos de IA — análogo ao CI/CD do software tradicional, mas adaptado à natureza não-determinística de agentes e LLMs. O ciclo tem dois laços: (1) **Desenvolvimento contínuo** — escopar capacidade → curar dataset → montar aplicação → definir métricas de avaliação → fazer deploy; (2) **Calibração contínua** — analisar comportamento em produção → identificar padrões de erro emergentes → aplicar correções → expandir métricas → avançar para o próximo nível de agência.

## Como aplicar
1. Antes de construir: monte um dataset pequeno de pares input–output esperado — alinha o time em como o produto deve se comportar.
2. Defina **métricas de avaliação** (não evals genéricas): dimensões específicas do que importa para aquele produto.
3. Faça deploy da versão mais simples possível (alta controle humano, baixa agência).
4. Monitore sinais implícitos (regeneração de resposta, abandono, tempo até ação) e explícitos (thumbs up/down).
5. Quando o comportamento se estabiliza — distribuição de dados não muda mais — avance para o próximo nível de agência.
6. Repita o ciclo; cada model upgrade zera a calibração.

## Insights por autor
### [[Aishwarya Naresh Reganti]]
- Surgiu de uma falha real: construíram um agente de suporte end-to-end para um cliente e tiveram de desligá-lo porque os hotfixes se acumulavam sem controle — sem flywheel estruturado.
- "Não é sobre ser a primeira empresa a ter um agente. É sobre ter construído os flywheels certos para melhorar com o tempo."
- Métricas de avaliação ≠ evals: evals capturam erros que você já sabe; monitoramento de produção captura padrões que você ainda não imaginou.
> 🎧 [Why most AI products fail (1:26:22)](https://www.youtube.com/watch?v=z7T1pCxgvlA)

### [[Kiriti Badam]]
- No Codex (OpenAI): usam evals + monitoramento de produção + vibes — nenhum isolado resolve; o ciclo é contínuo.
- Sinal de que é hora de avançar de estágio: "você não está mais recebendo novas informações; a distribuição de dados estabilizou."
> 🎧 [Why most AI products fail (1:26:22)](https://www.youtube.com/watch?v=z7T1pCxgvlA)

## Conceitos relacionados
[[Non-determinismo em produtos de IA]] · [[Humans in the Loop (algoritmos)]] · [[A-B Testing (Ronny Kohavi)]] · [[Assumption Testing]]
