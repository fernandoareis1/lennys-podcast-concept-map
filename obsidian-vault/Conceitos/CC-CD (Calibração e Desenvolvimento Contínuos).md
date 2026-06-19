---
tipo: framework
nivel: 3
fluxo: Experimentação & Dados
autores: [Aishwarya Naresh Reganti, Kiriti Badam]
---
# CC-CD (Calibração e Desenvolvimento Contínuos)

**Fluxo:** [[05 - Experimentação & Dados]] · **Tema:** [[Experimentação — AB testing & cultura]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Aishwarya Naresh Reganti]] · [[Kiriti Badam]]

## Ideia central
O **Continuous Calibration / Continuous Development** é o análogo de CI/CD para produtos de AI. Em software clássico, CI/CD integra código → roda testes unitários → faz deploy. Em AI, o ciclo é: desenvolver com dados curados → deployar → **calibrar comportamento emergente** → absorver o novo aprendizado → desenvolver a próxima versão. A diferença central: você não consegue escrever todos os testes antes de ver o produto em produção, porque usuários criam padrões de uso que você não antecipou.

## Como aplicar

### Loop Direito: Desenvolvimento Contínuo
1. **Escopo de capacidade:** defina exatamente o que o sistema deve fazer (e o que não deve). PMs e SMEs (especialistas no domínio) são críticos aqui — muitas vezes a equipe descobre que não está alinhada sobre como o produto deveria se comportar.
2. **Curadoria de dados:** monte um dataset de inputs esperados + outputs desejados. Não precisa ser exaustivo — só suficiente para começar e para revelar desalinhamentos internos.
3. **Configure o aplicativo** e defina métricas de avaliação (não apenas "evals", mas dimensões específicas de qualidade que importam para esse produto).
4. **Deploy** com escopo de agência baixo (veja [[Troca Agência-Controle em IA]]).
5. **Rode as métricas de avaliação** e observe comportamento real.

### Loop Esquerdo: Calibração Contínua
1. **Analise comportamento:** o que os usuários estão fazendo que você não antecipou?
2. **Identifique padrões de erro:** erros sistêmicos (ex: agente sempre dando reembolso indevido) vs. erros pontuais (tool calling mal configurado → corrija e siga em frente sem escrever eval para isso).
3. **Aplique correções** (prompt, dados, configuração de tools, lógica determinística).
4. **Adicione métricas de avaliação novas** apenas para padrões emergentes relevantes — não tente cobrir tudo com judges de LLM; logs de produção + sinais implícitos são frequentemente mais informativos.
5. Repita com agência progressivamente maior conforme calibração converge.

### Sinais de que você pode passar para a próxima versão
- Dias consecutivos de calibração sem novos padrões de comportamento.
- Taxa de aceitação de sugestões pelo humano está alta e estável.
- Padrões de falha são conhecidos e contidos.

### Sobre evals
CC-CD não substitui evals — reposiciona o lugar delas. Evals capturam erros que você **já conhece**; calibração de produção captura erros que você **não previu**. Você precisa dos dois, mas confiar só em evals é confiar só no que você já sabia.

## Insights por autor
### [[Aishwarya Naresh Reganti]]
- "Evaluation metrics catch only the errors that you're already aware of. There can be a lot of emerging patterns that you understand only after you put things in production."
- "The idea is just behavior calibration and not losing user trust as you do that behavior calibration."
- Sobre quando subir de nível: "If you're calibrating every one or two days and you're not seeing new data distribution patterns, the amount of information you gain is very low — that's when you know you can go to the next stage."

### [[Kiriti Badam]]
- "I don't think if anybody's coming and saying 'I have this concrete set of evals that I can bet my life on and I don't need to think about anything else' — it's not going to work."
- No Codex/OpenAI: evals para garantir regressões, mas também monitoramento intenso de uso real do produto pelos clientes.

> 🎧 [Why most AI products fail | Aishwarya & Kiriti (00:45)](https://www.youtube.com/watch?v=z7T1pCxgvlA)

## Conceitos relacionados
[[Não-determinismo em Produtos de IA]] · [[Troca Agência-Controle em IA]] · [[A-B Testing (Ronny Kohavi)]] · [[A maioria das ideias falha no teste]] · [[Assumption Testing]]
