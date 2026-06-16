# ROUTINE — instruções para processar um lote de episódios

Você é um agente rodando de forma autônoma. Objetivo: **expandir o mapa de conceitos** do Lenny's Podcast no vault Obsidian, processando um lote de episódios e fazendo commit.

## Parâmetros
- **TAMANHO DO LOTE:** 20 convidados por execução.
- **Transcrições-fonte:** `lennys-podcast-transcripts-main/lennys-podcast-transcripts-main/episodes/{slug}/transcript.md`
- **Vault:** `obsidian-vault/` com `Fluxos/`, `Conceitos/`, `Autores/`
- **Manifesto de progresso:** `obsidian-vault/_meta/processed.txt` (um slug por linha = já processado)

## Passos
1. Liste os diretórios em `episodes/` e leia `_meta/processed.txt`. Selecione os **próximos 20 slugs em ordem alfabética que NÃO estão no manifesto**. Se sobrarem menos de 20, processe o que houver.
2. Para cada episódio:
   a. Leia o `transcript.md`. **Confirme o convidado pelo CORPO do texto** (alguns frontmatters estão trocados).
   b. Extraia os principais **frameworks, mindsets e insights** do convidado (3–6 por episódio).
   c. Para cada conceito, crie uma nota em `Conceitos/` seguindo o schema abaixo. **Se o conceito já existir**, NÃO sobrescreva — adicione uma subseção `### [[Autor]]` em "Insights por autor" e inclua o autor no frontmatter `autores`.
   d. Crie/atualize a nota do convidado em `Autores/` (leve: bio curta + lista de conceitos + link do episódio).
   e. Garanta que cada conceito referencia seu fluxo via `[[NN - Nome do Fluxo]]` e adicione o conceito à seção "Frameworks & Conceitos" do hub correspondente em `Fluxos/`.
3. Anexe os slugs processados ao final de `_meta/processed.txt`.
4. **Valide os links:** todo `[[link]]` deve ter arquivo correspondente em `Conceitos/`, `Fluxos/`, `Autores/` ou raiz. Corrija ou remova links órfãos.
5. Faça **commit** com a mensagem `routine: +N convidados (slugs...)` e push para `main`.

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
