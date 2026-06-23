---
tipo: tecnica
nivel: 3
fluxo: Estratégia & Visão
autores: [Chip Huyen]
---
# RAG — Qualidade de Dados como Diferencial
**Fluxo:** [[02 - Estratégia & Visão]] · **Tema:** [[Estratégia — Estratégia de produto]] · **Camada:** L3
**Tipo:** Técnica · **Fontes:** [[Chip Huyen]]

## Ideia central
RAG (Retrieval-Augmented Generation) é simples em conceito: forneça ao modelo contexto relevante para que ele responda melhor. A ideia remonta a 2017 — para muitas perguntas, o modelo responde muito melhor quando tem informações de contexto do que quando não tem.

O que a maioria dos times erra: agonizam sobre qual banco de dados vetorial usar enquanto ignoram a dimensão que mais importa — a qualidade da preparação dos dados. Segundo Chip, em praticamente todas as empresas que analisou, o principal ganho em soluções RAG veio de melhor preparação de dados, não de escolha de banco de dados.

**O que é preparação de dados para RAG:**
- **Chunking correto** — tamanho ideal dos fragmentos de texto: muito grande = pouca granularidade; muito pequeno = contexto insuficiente
- **Metadata e contexto adicional** — enriquecer cada chunk com resumo, tags, perguntas hipotéticas que aquele chunk responde
- **Rewrite para AI** — documentação escrita para humanos frequentemente falha com AI; reescrever no formato pergunta-resposta ou adicionar camadas de anotação melhora drasticamente a recuperação
- **Resolução de referências** — se um documento diz "daqui em diante, X significa Y" e depois X aparece em outro chunk sem Y, o modelo não vai conseguir conectar

**A analogia de Sherlock Holmes:** mesmo o raciocínio estatístico básico de linguagem (Sherlock usando frequência de letras para decodificar símbolos) aplica o mesmo princípio — padrões emergem do contexto, e contexto de qualidade é o diferencial.

## Como aplicar
1. **Priorize dados antes do banco** — escolha banco de dados vetorial com base em requisitos reais (latência, padrão read/write-heavy). Para qualidade de resposta, foque 80% do esforço na preparação dos dados.
2. **Reescreva docs para AI** — documentação técnica assume conhecimento de contexto que AI não tem. Adicione anotações: o que esse termo significa em escala, qual é o contexto dessa função, qual seria a pergunta que esse chunk responde.
3. **Perguntas hipotéticas por chunk** — para cada fragmento de dado, gere as perguntas que aquele chunk pode responder. Use AI para isso. Melhora drasticamente a recuperação por similaridade semântica.
4. **Pense end-to-end, não por componente** — em RAG agentico, avalie cada etapa: as queries de busca são diversas? Os resultados são relevantes? Há breadth e depth suficiente?
5. **Não confunda "componente otimizado" com "sistema funcionando"** — AI é boa em tarefas isoladas bem definidas, mas falha quando o problema atravessa componentes. Pensamento sistêmico (entender como componentes interagem) é onde humanos ainda têm vantagem.

## Insights por autor
### [[Chip Huyen]]
- "Preparação de dados para RAG é extremamente importante. Na grande maioria das empresas que analisei, o maior ganho de performance em suas soluções RAG vem de melhor preparação de dados — não de agonizar sobre qual banco de dados vetorial usar."
- "Documentação é escrita para humanos lerem, e leitura de AI é diferente. Humanos têm senso comum e contexto que AI não tem. Às vezes é necessária uma camada de anotação para AI."
- "Para um chunk de documento, você pode gerar perguntas hipotéticas que aquele chunk ajuda a responder. Quando chega uma query, você verifica se ela corresponde a alguma das perguntas hipotéticas. É uma abordagem muito interessante."

## Conceitos relacionados
[[O que realmente melhora apps de IA]] · [[Era dos evals — o eval é o PRD do modelo]] · [[Pós-treinamento como nova fronteira]] · [[Produto como organismo]]
