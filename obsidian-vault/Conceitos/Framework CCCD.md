---
tipo: framework
nivel: 3
fluxo: Experimentação & Dados
autores: [Aishwarya Naresh Reganti, Kiriti Badam]
---
# Framework CCCD — Calibração Contínua e Desenvolvimento Contínuo
**Fluxo:** [[05 - Experimentação & Dados]] · **Tema:** [[Experimentação — AB testing & cultura]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Aishwarya Naresh Reganti]], [[Kiriti Badam]]

## Ideia central
Inspirado no CI/CD do desenvolvimento de software, o CCCD é o ciclo iterativo para construir produtos de IA sem perder a confiança do usuário. Dois loops paralelos: **Desenvolvimento Contínuo** (escopo mínimo → curar dados esperados → configurar app → definir métricas de avaliação → avaliar → implantar) e **Calibração Contínua** (monitorar produção → detectar padrões emergentes → aplicar correções → criar novas métricas). A regra central: comece sempre em **baixa agência / alto controle humano** e progrida somente quando o comportamento do sistema estiver estável.

## Como aplicar
1. **V1 — agência mínima:** o agente só *classifica* ou *sugere*, sem executar. Humanos mantêm decisão final.
2. Colete feedback implícito (regenerar resposta = insatisfação) e explícito (avaliações de humanos).
3. Identifique padrões de erro emergentes — os não cobertos pelos seus evals iniciais.
4. Sinal de "pronto para avançar": sessões de calibração retornam cada vez menos informação nova; distribuição de inputs estabilizou.
5. Eleve para V2 (agente sugere + executa sob supervisão) e repita o ciclo. V3 = autonomia plena apenas após confiança provada.
6. Logue o que humanos fazem (e modificam) para alimentar o flywheel automaticamente.

## Insights por autor
### [[Aishwarya Naresh Reganti]]
- Originou-se de um projeto de suporte ao cliente que teve de ser desligado por excesso de hot-fixes: sem calibração incremental os erros se acumularam além do controlável.
- Exemplo real — Air Canada: agente alucionou uma política de reembolso e a empresa teve de honrá-la por questões legais.
- "Não é sobre ser o primeiro a ter um agente. É sobre ter construído os flywheels certos para melhorar ao longo do tempo."
- Eventos externos (ex: depreciação de um modelo de LLM) reiniciam a calibração — o processo nunca acaba.

### [[Kiriti Badam]]
- Exemplo em customer support: V1 = roteamento de tickets; V2 = rascunho de resposta para o agente humano aprovar; V3 = resolução autônoma. Cada versão gera logs de comportamento humano como erro-análise gratuita.
- "Quando você começa pequeno e com alto controle humano, você é forçado a pensar: qual é o problema que vou resolver?"
- 74–75% das empresas entrevistadas em pesquisa (UC Berkeley/Databricks) listaram *confiabilidade* como principal obstáculo para implantar IA.

> 🎧 [Why most AI products fail: Lessons from 50+ AI deployments at OpenAI, Google & Amazon (1:26:22)](https://www.youtube.com/watch?v=z7T1pCxgvlA)

## Conceitos relacionados
[[Não-determinismo em Produtos de IA]] · [[Evals vs. Monitoramento em Produção]] · [[Humans in the Loop (algoritmos)]] · [[Decidir com poucos dados é melhor que com zero]]
