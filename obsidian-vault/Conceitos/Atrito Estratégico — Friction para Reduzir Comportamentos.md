---
tipo: framework
nivel: 3
fluxo: Experimentação & Dados
autores: [Kristen Berman]
---
# Atrito Estratégico — Friction para Reduzir Comportamentos

**Fluxo:** [[05 - Experimentação & Dados]] · **Tema:** [[Experimentação — AB testing & cultura]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Kristen Berman]]

## Ideia central
O atrito não é sempre inimigo do produto. **Para aumentar um comportamento: remova atrito. Para reduzir um comportamento indesejado: adicione atrito estrategicamente.** A ciência comportamental mostra que pequenas interrupções — um label, uma pergunta de confirmação, um delay de segundos — podem reduzir comportamentos nocivos sem bloquear o usuário.

**O princípio:**
- Comportamento humano é sensível ao custo de ação, não apenas à motivação
- Quando o custo sobe (mesmo marginalmente), a taxa de comportamento cai
- Isso vale tanto para comportamentos desejados (reduza custo) quanto para indesejados (aumente custo)

**Experimento TikTok — desinformação:**
- Problema: usuários compartilham vídeos com desinformação sem ler o conteúdo
- Intervenção: label no vídeo + popup "Você tem certeza?" antes de compartilhar
- Resultado: **-24% nas partilhas de desinformação**
- Mecanismo: a interrupção quebra o "estado quente" (hot state) — TikTok é uma plataforma de velocidade, e desacelerar 2 segundos já muda a decisão
- Sem bloquear, sem censurar — apenas tornar a ação consciente

**Estudo do elevador:**
- Delay de 16 segundos no elevador → pessoas usam as escadas
- O atrito não precisa ser grande: 16 segundos é suficiente para mudar comportamento
- Implicação de produto: delays estratégicos em ações irreversíveis (deletar conta, compartilhar, postar) funcionam como "safety net" comportamental

**Hot state vs. Cold state:**
- "Estado quente": alta ativação, reação rápida, pouca deliberação (scroll do TikTok, raiva no Twitter)
- "Estado frio": calma, deliberação, alinhamento com valores de longo prazo
- Atrito estratégico faz a transição de hot para cold no momento certo
- Produto no estado quente + decisão de longo prazo = receita para arrependimento

## Como aplicar
1. Mapeie os comportamentos que você quer *reduzir* no produto (compartilhar sem ler, deletar conta por impulso, gastar acima do orçamento, mensagem agressiva)
2. Para cada um: qual é o menor atrito possível que quebraria o hot state?
3. Teste: label informativo → pergunta de confirmação → delay → etapa adicional (ordem crescente de atrito)
4. Meça impacto nos comportamentos alvo E nos comportamentos saudáveis — não quer suprimir o que quer incentivar
5. Atrito deve ser visível e compreensível para o usuário — dark patterns geram atrito mas também geram raiva e churn
6. Combine com nudges positivos: atrito no indesejado + facilidade no desejado = dupla intervenção

## Insights por autor
### [[Kristen Berman]]
- "Atrito é uma das ferramentas mais poderosas e mais subutilizadas em produto — porque times acreditam que menos atrito é sempre melhor"
- TikTok foi cliente da Irrational Labs. O experimento de misinformation foi conduzido com ceticismo interno ("nossos usuários vão odiar o popup") mas os dados foram inequívocos
- O TikTok é o ambiente mais difícil para quebrar hot state — alta velocidade, conteúdo infinito, dopamina em loop. Se funciona lá, funciona em qualquer lugar
- Analogia elevador: "Não precisamos de grande esforço para mudar comportamento. Às vezes, só precisamos de 16 segundos."
- Kristen avisa: atrito estratégico não funciona quando é percebido como manipulação. Transparência sobre o motivo ("isso te dá um segundo para reconsiderar") aumenta aceitação

> 🎧 [Kristen Berman: Using behavioral science to build better products](https://www.youtube.com/watch?v=u53fplD_C30)

## Conceitos relacionados
[[Framework 3 Bs — Comportamento, Barreiras e Benefícios]] · [[Diagnóstico Comportamental — Jornada com Psicologias]] · [[Perguntas de Onboarding como Ativação de Benefício]] · [[A-B Testing (Ronny Kohavi)]] · [[Friction Logging]]
