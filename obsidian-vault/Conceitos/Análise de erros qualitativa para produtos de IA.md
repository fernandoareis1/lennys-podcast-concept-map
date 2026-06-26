---
tipo: framework
nivel: 3
fluxo: Experimentação & Dados
autores: [Hamel Husain, Shreya Shankar]
---
# Análise de erros qualitativa para produtos de IA
**Fluxo:** [[05 - Experimentação & Dados]] · **Tema:** [[Experimentação — Aprender com pouco e qualitativo]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Hamel Husain]] · [[Shreya Shankar]]

## Ideia central
Antes de criar qualquer eval automatizado, o PM ou especialista de domínio precisa **olhar os dados** — logs de interação (traces) da aplicação de IA — e identificar manualmente o que está errado. O processo usa técnicas da análise qualitativa (ciências sociais) aplicadas a aplicativos de LLM:

1. **Error analysis / Open coding**: amostrar ~100 traces, anotar informalmente o primeiro erro visível em cada um (sem tentar categorizar ainda).
2. **Axial coding**: usar um LLM para agrupar as anotações em categorias acionáveis de falha (ex.: "erro de handoff humano", "alucinação de feature inexistente").
3. **Contagem**: pivot table simples para descobrir quais falhas são mais frequentes — leva do caos a prioridades claras.
4. **Saturação teórica**: parar quando novos traces não revelam novos tipos de erro.

O ponto central: nenhum LLM consegue fazer essa análise inicial no lugar do humano, porque o humano traz o contexto de negócio necessário para reconhecer o que é uma falha real (ex.: um agente que diz que tem tour virtual quando a empresa não oferece isso).

## Como aplicar
1. Acesse sua ferramenta de observabilidade (LangSmith, Braintrust, Phoenix Arize, etc.) e amostre traces recentes.
2. Para cada trace, escreva uma nota curta e descritiva do primeiro problema que você encontrar — sem tentar ser perfecto, apenas descritivo.
3. Exporte as notas para um CSV e peça a um LLM para criar "axial codes" (categorias de falha) — revise e renomeie categorias genéricas demais.
4. Use fórmulas de planilha + LLM para categorizar automaticamente cada nota em uma das categorias.
5. Construa um pivot table para contar a frequência de cada categoria de falha.
6. Decida quais falhas merecem um eval automatizado (vs. simples correção de prompt).

## Insights por autor
### [[Hamel Husain]]
- "Quando as pessoas fazem esse processo de olhar os dados, ficam imediatamente viciadas. Você aprende muito sobre sua aplicação em pouco tempo."
- "Dumb is sometimes a good way to get started." — a técnica de contagem simples é subestimada; é análise de dados básica mas poderosa.
- "As pessoas vão direto para os testes como, 'vou escrever uns testes', e é aí que as coisas saem dos trilhos. Você precisa primeiro fazer análise de dados para saber o que merece teste."
- Benevolent dictator: escolha uma pessoa com expertise de domínio para conduzir o processo — comitês tornam isso caro e lento.

> 🎧 [Why AI evals are the hottest new skill for product builders | Hamel Husain & Shreya Shankar (1:46:33)](https://www.youtube.com/watch?v=BsWxPI9UM4c) · 2025-09-25

### [[Shreya Shankar]]
- Open coding e axial coding vêm das ciências sociais — não são invenções deles. "Se alguém te traz uma forma de fazer algo inteiramente nova, sem embasamento em teoria, seja cético."
- **Saturação teórica**: pare de olhar traces quando não estiver mais aprendendo tipos novos de problema — às vezes 15 traces bastam, às vezes são 60.
- Um LLM pode categorizar os open codes nas categorias axiais automaticamente — mas as notas precisam ser descritivas, não vagas ("janky" não ajuda; "não confirmou transferência de chamada com o usuário" sim).
- Inclua sempre uma categoria "nenhuma das acima" para o LLM categorizar — isso revela lacunas no seu sistema de categorias.

> 🎧 [Why AI evals are the hottest new skill for product builders | Hamel Husain & Shreya Shankar (1:46:33)](https://www.youtube.com/watch?v=BsWxPI9UM4c) · 2025-09-25

## Conceitos relacionados
[[Era dos evals — o eval é o PRD do modelo]] · [[LLM como Juiz — avaliação automatizada de qualidade]] · [[Non-determinismo em Produtos de IA]] · [[CC-CD — Calibração Contínua, Desenvolvimento Contínuo]]
