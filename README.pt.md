# Cola de referência: expressões regulares · Regex Cheatsheet

> 🌍 [中文](README.md) · [Español](README.es.md)

Uma **cola de uma página só** para expressões regulares: 30 entradas, e cada uma responde a apenas três perguntas — **o que ela casa, um padrão pronto para copiar e etiquetas de uso**. Baseada na sintaxe comum de PCRE / Python / JavaScript; as diferenças entre motores estão indicadas onde cabem. Sem enrolação.

## Para quem é

Para desenvolvedores backend, engenheiros de operações (SRE/DevOps), quem trabalha com dados e qualquer pessoa que lide todo dia com logs e texto. Se toda vez que você escreve uma regex precisa consultar a documentação, esta cola ajuda a memorizar os padrões mais usados de uma vez.

## Como usar

1. Vá direto ao **[CHEATSHEET.md](CHEATSHEET.md)** — o corpo da referência; os padrões em inglês qualquer desenvolvedor entende.
2. Valide os padrões duvidosos no **[regex101.com](https://regex101.com/)**: escolha o motor certo (PCRE2 / Python / JavaScript) e teste um por um.
3. Percorra na ordem — metacaracteres → quantificadores → grupos → asserções → padrões práticos → armadilhas; os padrões práticos dá para copiar e adaptar.

## O que está incluído

| Categoria | Conteúdo |
|---|---|
| 🔤 Metacaracteres básicos | `.` `\d` `\w` `\s` e suas versões negadas em maiúscula, `^` `$` `\b` (6) |
| 🔁 Quantificadores | `*` `+` `?` `{n,m}`, guloso vs. preguiçoso (3) |
| 🧩 Classes de caracteres e alternância | `[...]` `[^...]` `|` (3) |
| 📦 Grupos e capturas | `(...)`, capturas nomeadas, grupos não-capturadores, retro-referências (4) |
| 👀 Asserções | *lookahead* `(?=)` `(?!)`, *lookbehind* `(?<=)` `(?<!)` (4) |
| 🛠️ Padrões práticos | e-mail, URL, telefone, IPv4, data, tags HTML, remover espaços (7) |
| 🔄 Truques de substituição | retro-referências na substituição, diferenças entre motores (1) |
| ⚠️ Armadilhas | *backtracking* catastrófico, não parseie HTML com regex (2) |

Todos os padrões são sintaxe real e válida; as diferenças entre motores estão indicadas.

## Nota sobre motores

- A base é **PCRE** (PHP, Nginx, `grep -P`);
- As diferenças do `re` do Python e do JavaScript estão indicadas em cada entrada (p. ex. *lookbehind*, sintaxe de capturas nomeadas);
- Para validar on-line use https://regex101.com/, escolhendo o motor no canto superior esquerdo.

## Contribuições são bem-vindas

Achou um padrão errado, uma forma melhor de escrevê-lo ou uma tradução a melhorar? *Pull requests* são bem-vindos. Mantenha o formato (o que casa / padrão / etiquetas) e **valide cada padrão no regex101 com o motor correspondente antes de enviar**.

## Licença

MIT © 2026 Guangyi Zhao. Veja [LICENSE](LICENSE).
