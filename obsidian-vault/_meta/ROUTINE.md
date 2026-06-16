# ROUTINE — instruções para processar um lote de episódios

Você é um agente rodando de forma autônoma. Objetivo: **expandir o mapa de conceitos** do Lenny's Podcast no vault Obsidian, processando um lote de episódios e fazendo commit.

## Parâmetros
- **TAMANHO DO LOTE:** 20 convidados por execução.
- **Transcrições-fonte:** `lennys-podcast-transcripts-main/lennys-podcast-transcripts-main/episodes/{slug}/transcript.md`
- **Vault:** `obsidian-vault/` com `Fluxos/`, `Conceitos/`, `Autores/`
- **Manifesto de progresso:** `obsidian-vault/_meta/processed.txt` (um slug por linha = já processado)

## Passos
1. Liste os diretórios em `episodes/` e leia `_meta/processed.txt`. Selecione os **próximos slugs em ordem alfabética que NÃO estão no manifesto** (até 20 nesta execução).
2. Processe **UM convidado de cada vez**. Para CADA convidado:
   a. Leia o `transcript.md`. **Confirme o convidado pelo CORPO do texto** (alguns frontmatters estão trocados).
   b. Extraia os principais **frameworks, mindsets e insights** (3–6).
   c. Crie/atualize notas em `Conceitos/` (schema abaixo). **Se o conceito já existir**, NÃO sobrescreva — adicione uma subseção `### [[Autor]]` em "Insights por autor" e inclua o autor no frontmatter `autores`.
   d. Crie/atualize a nota do convidado em `Autores/` (leve: bio + lista de conceitos + link do episódio).
   e. Adicione cada conceito ao fluxo via `[[NN - Nome do Fluxo]]` e à seção "Frameworks & Conceitos" do hub em `Fluxos/`.
   f. Anexe o slug a `_meta/processed.txt`.
   g. Valide que os `[[links]]` criados têm arquivo correspondente em `Conceitos/`/`Fluxos/`/`Autores/`/raiz (corrija órfãos).
   h. **COMMIT + PUSH IMEDIATO deste convidado:** `git add -A && git commit -m "routine: +1 (slug)" && git push origin main`.
3. Repita o passo 2 até processar 20 convidados **ou** até a sessão estar acabando.
   ⚠️ **NUNCA acumule.** Cada convidado deve ser commitado/pushed ANTES de ir ao próximo, para que o progresso sobreviva a qualquer interrupção (timeout, limite de contexto, pausa).

## Schema da nota de conceito (PT-BR)
```markdown
---
tipo: framework | mindset | tecnica | insight | conceito
fluxo: <Nome do Fluxo>
autores: [Nome]
---
# <Nome do Conceito>

**Fluxo:** [[NN - Nome do Fluxo]]
**Tipo:** ...
**Fontes:** [[Nome do Autor]]

## Ideia central
2–4 linhas.

## Como aplicar
passos práticos (quando fizer sentido).

## Insights por autor
### [[Nome do Autor]]
- ponto + citação curta
> 🎧 [Título do episódio (duração)](youtube_url)

## Conceitos relacionados
[[...]] · [[...]]
```

## Os 10 fluxos (taxonomia fixa)
01 Discovery & Pesquisa · 02 Estratégia & Visão · 03 Priorização & Roadmap · 04 Design & UX · 05 Experimentação & Dados · 06 Growth & Aquisição · 07 Ativação & Retenção · 08 Monetização & Pricing · 09 Liderança & Times · 10 Founder & Carreira

## Princípios
- **Eixo = conceito, não autor.** O autor é fonte/citação.
- Tudo em **PT-BR**.
- Não invente citações; baseie-se no que está na transcrição.
- Prefira **mesclar** conceitos repetidos (acumular insights de vários autores) a duplicar notas.
