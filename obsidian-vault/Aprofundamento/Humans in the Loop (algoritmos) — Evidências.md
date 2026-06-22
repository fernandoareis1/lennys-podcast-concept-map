---
tipo: aprofundamento
nivel: 4
fluxo: Experimentação & Dados
conceito_pai: Humans in the Loop (algoritmos)
autores: [Adriel Frederick, Aishwarya Naresh Reganti, Kiriti Badam]
---
# 📜 Humans in the Loop (algoritmos) — Evidências
**↑ Card:** [[Humans in the Loop (algoritmos)]] · **Tema:** [[Experimentação — AB testing & cultura]] · **Camada:** L4
**Fontes:** [[Adriel Frederick]] (1:07:26) · [[Aishwarya Naresh Reganti]] (1:26:22) · [[Kiriti Badam]] (1:26:22)

---

## [[Adriel Frederick]] — Algoritmos de pricing no Lyft
*(Episódio: Humanizing product development — [1:07:26](https://www.youtube.com/watch?v=uMhBej6-Ey4))*

O time do Lyft construiu um algoritmo de pricing tecnicamente excelente — mas que não deixava operadores humanos ajustar preços com flexibilidade. O algoritmo otimizava o curto prazo sem "ver" eventos que o humano enxergava: nevascas em Chicago, mudanças de concorrentes, novas regulamentações.

> "Quando você trabalha em produtos pesados em algoritmos, seu trabalho é definir pelo que o algoritmo é responsável, pelo que as pessoas são responsáveis, e o framework para tomar decisões."

O resultado prático: tiveram que reconstruir o sistema do zero para inserir o humano no loop. A lição: separar explicitamente as decisões que o algoritmo pode otimizar (execução em tempo real, volume alto, regras claras) das que exigem julgamento estratégico ou contextual (objetivos, restrições, timing, efeitos de longo prazo).

**Mecânica prática:**
- Liste todas as decisões recorrentes no produto.
- Separe: "o algoritmo pode otimizar isso" vs. "isso requer contexto estratégico/humano".
- Para as decisões humanas: projete a interface — quais dados essa pessoa precisa ver, quais controles ela precisa ter.

---

## [[Aishwarya Naresh Reganti]] + [[Kiriti Badam]] — Trade-off Agência-Controle em Agentes de IA
*(Episódio: Why most AI products fail — [1:26:22](https://www.youtube.com/watch?v=z7T1pCxgvlA))*

Em produtos de IA agenticos, a divisão humano/algoritmo deixa de ser uma configuração estática e vira um **espectro dinâmico de agência** que deve aumentar gradualmente conforme o sistema ganha confiança.

> "Toda vez que você entrega capacidade de decisão a sistemas agênticos, você está relinquindo alguma quantidade de controle. Você quer ter certeza de que o agente ganhou essa capacidade ou construiu confiança ao longo do tempo." — Aishwarya

> "Quando você começa com alta controle humano e baixa agência, você também se força a pensar: qual é o problema que estou resolvendo?" — Kiriti

**Estudo de caso: agente de suporte ao cliente (Aishwarya)**

A equipe de Aishwarya construiu um agente end-to-end de suporte para um cliente — e teve que desligar o produto porque os hotfixes se acumulavam: sem visibilidade de comportamento e sem flywheel, cada erro novo era uma crise.

A versão reformulada seguiu 3 estágios:

| Versão | Agência | Controle | O que o agente faz | O que o humano faz |
|---|---|---|---|---|
| V1 · Roteamento | Baixa | Alta | Classifica e roteia o ticket para o departamento certo | Aprova/corrige o roteamento |
| V2 · Copiloto | Média | Média | Gera rascunho de resposta com base em SOPs | Edita e envia; o delta usado vira error analysis |
| V3 · Resolução autônoma | Alta | Baixa | Resolve o ticket + aciona ferramentas (ex.: emitir reembolso) | Monitora via dashboard |

**Por que o log do V2 é tão valioso:** o quanto do rascunho foi usado pelo agente humano é um proxy direto de qualidade — error analysis quase de graça, sem construir um judge separado.

**Dados de campo:** 74–75% das empresas entrevistadas por Matei Zaharia (UC Berkeley/Databricks) citaram **confiabilidade** como principal obstáculo para expor usuários a produtos de IA. Isso explica por que a maioria dos produtos de IA está no quadrante de produtividade (baixa agência) e não em agentes end-to-end.

**Sinal de quando avançar de estágio:**
> "Quando a distribuição de dados se estabiliza e você para de receber novas informações — a quantidade de aprendizado que você ganha é muito baixa. Esse é o sinal de que você pode avançar para o próximo nível de agência."

**Cuidado com model upgrades:** cada novo modelo (ex.: GPT-4o → GPT-5) tem propriedades diferentes; o sistema precisa ser recalibrado do zero para o novo modelo — o trade-off agência-controle não é uma decisão definitiva.

---

## Síntese cross-autores

| Dimensão | Adriel Frederick (algoritmos de produto) | Aishwarya + Kiriti (agentes de IA) |
|---|---|---|
| Natureza do sistema | Algoritmo de ML em feature determinística | Agente LLM não-determinístico |
| Ponto de controle humano | Interface operacional de ajuste estratégico | Estágio da cadeia de decisão do agente |
| Principal risco sem controle | Otimização de curto prazo às custas de objetivos maiores | Erros em cascata + corrosão de confiança do usuário |
| Mecanismo de aprendizado | Feedback direto do operador | Log de comportamento humano no laço de sugestão |
| Sinal de que funciona | KPI de negócio atendido com flexibilidade | Distribuição de dados estabilizada; usuário satisfeito |

**Convergência:** independente de algoritmo clássico ou LLM, o princípio é o mesmo — **o humano define direção e restrições; a máquina executa em escala**. A diferença é que com agentes a fronteira é fluida e precisa ser gerenciada dinamicamente, não fixada em design.
