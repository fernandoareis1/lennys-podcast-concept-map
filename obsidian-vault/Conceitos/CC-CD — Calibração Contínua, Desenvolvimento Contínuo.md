---
tipo: framework
nivel: 3
fluxo: Experimentação & Dados
autores: [Aishwarya Naresh Reganti, Kiriti Badam]
---
# CC/CD — Calibração Contínua, Desenvolvimento Contínuo
**Fluxo:** [[05 - Experimentação & Dados]] · **Tema:** [[Experimentação — Aprender com pouco e qualitativo]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Aishwarya Naresh Reganti]] · [[Kiriti Badam]]

## Ideia central
Analogia deliberada com CI/CD do desenvolvimento de software, o CC/CD é o ciclo de vida iterativo para produtos de IA. Em vez de "integrar e deployar", o loop é: **definir escopo → curar dados → configurar aplicação → desenhar métricas de avaliação → deployar → calibrar comportamento → detectar padrões novos → aplicar fixes → repetir**. O objetivo não é ter um produto perfeito no lançamento, mas garantir que o comportamento é observável, corrigível e evolui com segurança — sem destruir a experiência do usuário no processo.

## Como aplicar
1. **Lado "Desenvolvimento Contínuo":** antes de buildar, monte um dataset representativo de inputs esperados e outputs desejados. Use esse exercício para alinhar PMs, engenheiros e especialistas de domínio sobre como o produto deve se comportar.
2. Configure o sistema e defina **métricas de avaliação** (não apenas "evals genéricas" — dimensões específicas que importam para o seu caso).
3. **Lado "Calibração Contínua":** após o deploy, monitore em produção. Sinais implícitos (regeneração de resposta, abandono, thumbs down) revelam padrões que evals pré-definidas não capturam.
4. Ao detectar novos padrões de falha: (a) aplique fix pontual se for erro isolado, (b) crie nova métrica de avaliação se o padrão se repetir.
5. **Critério para avançar de degrau de autonomia:** quando o ciclo de calibração parar de revelar novos padrões de comportamento inesperado.

## Insights por autor
### [[Aishwarya Naresh Reganti]] e [[Kiriti Badam]]
- A motivação: tentaram buildar um agente de suporte "end-to-end" e precisaram desligar o produto porque acumulavam hot fixes sem conseguir mapear todos os problemas emergentes.
- "Métricas de avaliação capturam apenas os erros que você já conhece. Padrões emergentes só aparecem quando você está em produção."
- Exemplo concreto (suporte): V1 = agente só faz routing de tickets (aprende taxonomia e dados); V2 = agente drafta resposta (humano edita e você loga o delta = feedback grátis); V3 = agente resolve de ponta a ponta.
- Eventos externos (ex: troca de modelo GPT-4o → GPT-5, mudança de comportamento de usuários) reiniciam a calibração — volte ao início do loop.

> 🎧 [Why most AI products fail (1:26:22)](https://www.youtube.com/watch?v=z7T1pCxgvlA)

## Conceitos relacionados
[[Trade-off Agência-Controle]] · [[Non-determinismo em Produtos de IA]] · [[Assumption Testing]] · [[Decidir com poucos dados é melhor que com zero]] · [[Experimentação — AB testing & cultura]]
