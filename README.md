# hubcontexto-jus

Registry CDN do **Hub Contexto Jus** — `catalog.json` e Releases `.kongrupack`.

Este repositório **não** contém o código do site Vite nem do desktop Kongru. Serve só para distribuição pública de pacotes de contexto jurídico.

## Links

| Recurso | URL |
|---------|-----|
| Catálogo | https://raw.githubusercontent.com/kongru04-tech/hubcontexto-jus/main/catalog.json |
| Releases | https://github.com/kongru04-tech/hubcontexto-jus/releases |

## Pacotes atuais (F2.5)

| Pack | Chunks | Embedding |
|------|--------|-----------|
| Súmulas Vinculantes do STF | 62 | E5-small real |
| Súmulas do STJ | 676 | E5-small real |
| Demo Hub F2 | 3 | placeholder (regressão CDN) |

Textos derivados de datasets abertos (coleção Hugging Face `celsowm`); embeddings gerados com `intfloat/multilingual-e5-small`. Confirme sempre a vigência nas fontes oficiais.

## Formato `.kongrupack`

ZIP com:

- `metadata.json` — manifesto (pack_id, versão, modelo E5, contagem de chunks)
- `chunks.parquet` — texto + metadados + vetores (`intfloat/multilingual-e5-small`, 384d)

## Licença

MIT para a estrutura deste registry. Textos jurídicos oficiais preservam o regime das fontes públicas.
