# Hoja de referencia: expresiones regulares · Regex Cheatsheet

> 🌍 [中文](README.md) · [Português](README.pt.md)

Una **hoja de referencia de una sola página** para expresiones regulares: 30 entradas, y cada una responde solo tres preguntas — **qué coincide, un patrón listo para copiar y etiquetas de uso**. Basada en la sintaxis común de PCRE / Python / JavaScript; las diferencias entre motores están indicadas donde corresponde. Sin relleno.

## Para quién es

Para desarrolladores backend, ingenieros de operaciones (SRE/DevOps), quienes trabajan con datos y cualquiera que lidie a diario con logs y texto. Si cada vez que escribes una expresión regular tienes que consultar la documentación, esta hoja te ayuda a memorizar los patrones más usados de una vez.

## Cómo usarla

1. Ve directo a **[CHEATSHEET.md](CHEATSHEET.md)** — el cuerpo de la referencia; los patrones en inglés los entiende cualquier desarrollador.
2. Verifica los patrones dudosos en **[regex101.com](https://regex101.com/)**: elige el motor correcto (PCRE2 / Python / JavaScript) y pruébalos uno por uno.
3. Recórrela en orden — metacaracteres → cuantificadores → grupos → aserciones → patrones prácticos → trampas comunes; los patrones prácticos se pueden copiar y adaptar.

## Qué incluye

| Categoría | Contenido |
|---|---|
| 🔤 Metacaracteres básicos | `.` `\d` `\w` `\s` y sus versiones negadas en mayúscula, `^` `$` `\b` (6) |
| 🔁 Cuantificadores | `*` `+` `?` `{n,m}`, codicioso vs. perezoso (3) |
| 🧩 Clases de caracteres y alternancia | `[...]` `[^...]` `|` (3) |
| 📦 Grupos y capturas | `(...)`, capturas con nombre, grupos no capturadores, retrorreferencias (4) |
| 👀 Aserciones | *lookahead* `(?=)` `(?!)`, *lookbehind* `(?<=)` `(?<!)` (4) |
| 🛠️ Patrones prácticos | email, URL, teléfono, IPv4, fecha, etiquetas HTML, quitar espacios (7) |
| 🔄 Trucos de reemplazo | retrorreferencias en reemplazos, diferencias entre motores (1) |
| ⚠️ Trampas comunes | retroceso catastrófico, no analices HTML con regex (2) |

Todos los patrones son sintaxis real y válida; las diferencias entre motores están indicadas.

## Nota sobre motores

- La base es **PCRE** (PHP, Nginx, `grep -P`);
- Las diferencias de Python `re` y JavaScript se indican en cada entrada (p. ej. *lookbehind*, sintaxis de capturas con nombre);
- Para verificar en línea usa https://regex101.com/, eligiendo el motor arriba a la izquierda.

## Contribuciones bienvenidas

¿Un patrón incorrecto, una forma mejor de escribirlo o una traducción mejorable? Los *pull requests* son bienvenidos. Mantén el formato (qué coincide / patrón / etiquetas) y **verifica cada patrón en regex101 con el motor correspondiente antes de enviarlo**.

## Licencia

MIT © 2026 Guangyi Zhao. Ver [LICENSE](LICENSE).
