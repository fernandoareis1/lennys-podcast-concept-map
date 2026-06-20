---
tipo: framework
nivel: 3
fluxo: Experimentação & Dados
autores: [Aishwarya Naresh Reganti, Kiriti Badam]
---
# CC/CD Framework
**Fluxo:** [[05 - Experimentação & Dados]] · **Tema:** [[Experimentação — AB testing & cultura]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Aishwarya Naresh Reganti]] · [[Kiriti Badam]]

## Ideia central
O **Continuous Calibration / Continuous Development** (CC/CD) é o equivalente do CI/CD para produtos de AI. O ciclo tem dois braços: (1) **Continuous Development** — escopo de capacidade → curadoria de dados → design de métricas de avaliação → deploy; (2) **Continuous Calibration** — monitoramento em produção → análise de padrões de erro inesperados → aplicação de fixes → design de novas métricas → volta ao deploy. O diferencial é que você parte de baixa agência e vai aumentando à medida que calibra o comportamento.

## Como aplicar
1. **Scoping:** antes de construir, alinhe o time em um dataset de exemplos de input/output esperados. Isso revela divergências de expectativa entre PM, engenheiro e SME.
2. **Deploy com baixa agência:** comece pelo V1 com alto controle humano (ver [[Agency-Control Trade-off]]).
3. **Monitorar sinais implícitos:** além de thumbs up/down, log regenerações, abandonos, edições de sugestões — são sinais que o usuário não aprovou a resposta.
4. **Analisar padrões emergentes:** categorize os erros em produção. Só crie LLM judge para padrões recorrentes; erros pontuais podem ser corrigidos diretamente.
5. **Critério para avançar ao próximo nível de agência:** quando você para de ver novas distribuições de dados — o comportamento dos usuários estabilizou — é sinal de que o sistema está calibrado para aquele escopo.
6. **Recalibrar após eventos externos:** mudança de modelo (ex.: migrar de GPT-4o para GPT-5) ou mudança de comportamento do usuário reinicia o ciclo.

## Insights por autor
### [[Aishwarya Naresh Reganti]]
- O gatilho para criar o framework foi um produto de customer support que precisou ser desligado por acúmulo de hot-fixes após ter começado como agente end-to-end desde V1.
- O Air Canada teve que honrar juridicamente uma política de reembolso inventada pelo seu chatbot — um caso real de falha por excesso de agência sem calibração.
- "Não é sobre ser a primeira empresa a ter um agente. É sobre ter construído os flywheels certos para melhorar ao longo do tempo."
- Evals capturam apenas erros que você já antecipou; monitoramento em produção captura padrões emergentes que você não previu.

### [[Kiriti Badam]]
- No Codex (OpenAI): usam evals para garantir que mudanças de modelo não quebram comportamentos core, **e** monitoramento de produção para capturar novos padrões de uso.
- Sinal prático de que uma resposta está ruim: o usuário não dá thumbs down, mas regenera — esse sinal implícito é mais confiável que o explícito.
- Falsa dicotomia do setor: "evals OR monitoramento de produção". A resposta correta é: **ambos, para fins diferentes**.

> 🎧 [Why most AI products fail (45:41–58:07)](https://www.youtube.com/watch?v=z7T1pCxgvlA)

## Conceitos relacionados
[[Agency-Control Trade-off]] · [[Non-determinismo em Produtos AI]] · [[Humans in the Loop (algoritmos)]] · [[Experimentação — AB testing & cultura]] · [[A maioria das ideias falha no teste]]
