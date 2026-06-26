---
tipo: framework
nivel: 3
fluxo: Ativação & Retenção
autores: [Hila Qu]
---
# Momento Aha — Como Encontrar e Validar
**Fluxo:** [[07 - Ativação & Retenção]] · **Tema:** [[Retenção — Ativação & onboarding]] · **Camada:** L3
**Tipo:** Framework · **Fontes:** [[Hila Qu]]

## Ideia central
O "aha moment" — primeiro instante em que o usuário experiencia o valor real do produto — é a maior alavanca de ativação e retenção. Mas a maioria das empresas não sabe qual é o seu. O processo para encontrá-lo é de duas fases: **correlação** → **causalidade**.

## Passo a passo

### Fase 1: Correlação
1. **Brainstorm de ações de alto valor** — o time lista 8-10 ações que indicam que o usuário está recebendo valor (ex.: "fez o primeiro merge de PR", "rodou o primeiro pipeline", "convidou um colega")
2. **Análise de correlação dupla** — para cada ação, calcule:
   - Taxa de conversão em 90 dias de quem realizou a ação vs. média
   - Taxa de retenção em 30 dias de quem realizou a ação vs. média
3. **Selecione os candidatos** — ações que elevam *ambas* (conversão E retenção) são candidatos ao aha moment; se só uma sobe, o sinal é incompleto

### Fase 2: Causalidade (obrigatória)
4. **Lance experimentos** — crie variações que forçam mais usuários a realizarem as ações candidatas
5. **Valide na métrica de negócio** — se conversão e retenção sobem no grupo experimental, a causalidade é confirmada

> **Por que separar as fases?** Correlação mostra que "quem faz X converte mais", não que "fazer X causa conversão". Usuários motivados fazem mais coisas. Sem o experimento, você pode otimizar algo que é consequência, não causa.

## Exemplo: GitLab
Candidatos iniciais: merge de PR, execução de pipeline, setup de CI/CD. Problema: GitLab é uma plataforma com múltiplos workflows — nenhuma ação única cobria todos os usuários.

Solução: **aha moment composto** — "2 usuários + 2 features nos primeiros 14 dias"
- **2 usuários**: o primeiro usuário está confiante o suficiente para convidar um colega → forte sinal de valor percebido
- **2 features**: colaboração em plataforma → não apenas uso individual, mas uso do produto como produto de time
- **14 dias**: tempo realista para produto complexo B2B, sem ser permissivo demais

## Variações por tipo de produto
- **B2C simples** (Facebook, Zynga): 1 ação clara, primeiros dias. Ex.: "10 amigos em 7 dias"
- **B2B plataforma**: ação composta, janela de tempo maior (14-30 dias)
- **Produto de time**: componente de "invite" quase sempre sinaliza valor

## Insights por autor
### [[Hila Qu]]
- "O aha moment é o momento em que o usuário experiencia o valor do seu produto pela primeira vez. É onde está a maior oportunidade — o usuário já superou tantas barreiras, não o decepcione agora."
- "Correlação não prova causalidade. Usuários motivados fazem mais de tudo. O experimento é o passo obrigatório para validar que *fazer* a ação *causa* conversão."
- "Para GitLab, optamos por 2 usuários + 2 features em 14 dias porque somos uma plataforma. Os 2 usuários capturam o componente de colaboração que é o coração do produto."
> 🎧 [The ultimate guide to adding a PLG motion (0:39:00)](https://www.youtube.com/watch?v=7l1fIxk7SnA)

## Conceitos relacionados
[[Ativação via onboarding]] · [[Auditoria de Funil PLG]] · [[Product-Led Growth (PLG)]] · [[Usuário lazy, vain e selfish]] · [[Primeiros 30 Segundos — Onboarding Mágico]]
