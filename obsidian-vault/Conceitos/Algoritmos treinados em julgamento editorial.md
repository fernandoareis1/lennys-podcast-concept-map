---
tipo: framework
nivel: 3
fluxo: Experimentação & Dados
autores: [Alex Hardiman]
---
# Algoritmos treinados em julgamento editorial
**Fluxo:** [[05 - Experimentação & Dados]] · **Tema:** [[Experimentação — AB testing & cultura]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Alex Hardiman]]

## Ideia central
Em vez de treinar algoritmos de recomendação puramente em sinais de engajamento (cliques, tempo de sessão), o NYT treina seus algoritmos em **julgamento editorial**: scores de importância atribuídos pelos próprios jornalistas, que codificam qualidade e relevância da cobertura. Isso permite escalar julgamento humano de alta qualidade a milhões de leitores, ao contrário do Facebook (que só podia usar engagement como proxy). O resultado é um feed que é *ao mesmo tempo* editorialmente curado e personalizado — arte + ciência.

## Como aplicar
1. Identifique quem na sua empresa tem expertise para avaliar *qualidade* do conteúdo ou da ação (não apenas popularidade).
2. Estruture esse expertise em signals mensuráveis: notas de importância, tags de qualidade, selos de confiança, etc.
3. Treine ou ajuste seus algoritmos nesses signals editoriais como *features adicionais* ao lado de signals de engajamento.
4. Crie um processo contínuo para que especialistas de domínio atualizem e refinam esses signals conforme o contexto evolui.
5. Monitore se o algoritmo está "driblando" os signals editoriais ao otimizar engagement — isso pode acontecer e precisa de guardrails.

## Insights por autor
### [[Alex Hardiman]]
- "No Facebook, só podíamos treinar com sinais de engajamento. Não dava para treinar com base na qualidade da informação em si."
- NYT tem 2000+ jornalistas estruturando seu expertise em signals que alimentam decisão algorítmica.
- "PMs de produto estão se tornando muito mais editorialmente atentos, e estamos conseguindo que editores se tornem mais voltados a produto."
- O risco do puro engagement como métrica: distribuição de desinformação, viralização sem critério de veracidade — o aprendizado da crise de 2016 no Facebook.
> 🎧 [An inside look at how the New York Times builds product (1:07:21)](https://www.youtube.com/watch?v=y3-cwoHMwQs)

## Conceitos relacionados
[[Humans in the Loop (algoritmos)]] · [[Experimentação — AB testing & cultura]] · [[Missão como prioridade máxima]] · [[OEC - Overall Evaluation Criterion]]
