# hubcontexto-jus

Registry CDN do **Hub Contexto Jus** — `catalog.json` e Releases `.kongrupack`.

Este repositório **não** contém o código do site Vite nem do desktop Kongru. Serve só para distribuição pública de pacotes de contexto jurídico.

## Links

| Recurso | URL |
|---------|-----|
| Catálogo | https://raw.githubusercontent.com/kongru04-tech/hubcontexto-jus/main/catalog.json |
| Releases | https://github.com/kongru04-tech/hubcontexto-jus/releases |

## Formato `.kongrupack`

ZIP com:

- `metadata.json` — manifesto (pack_id, versão, modelo E5, contagem de chunks)
- `chunks.parquet` — texto + metadados + vetores (`intfloat/multilingual-e5-small`, 384d)

## Fase 2 (A)

Inclui um pack **demo técnico** (`kongru.demo.hub-f2`) para validar download via GitHub Releases. Os vetores do demo são placeholders — não usar em produção RAG.

## Licença

MIT para a estrutura deste registry. Textos jurídicos oficiais (quando publicados em packs reais) preservam o regime das fontes públicas.
