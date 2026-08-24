# good-design

Una skill que evita que una web parezca hecha por IA.

![La misma landing sin la skill y con ella](docs/antes-despues.png)

*La misma landing, el mismo encargo. A la izquierda lo que sale por defecto: degradado
morado-azul, cristal por todas partes, emojis de icono, todo centrado, tres tarjetas
idénticas y "10K+ usuarios felices". A la derecha, con la skill: retícula suiza, fondo
plano, un solo acento, y cifras que dicen algo en vez de adornar.*

Le da al modelo la lista de delatores (degradado morado-azul, glassmorphism en todo,
emojis como iconos, todo centrado, tres tarjetas iguales, `Inter` para absolutamente
todo) y, más importante, qué hacer en su lugar: una escala tipográfica de verdad,
medida de 60-75 caracteres, un solo acento usado poco, contraste 4.5:1.

Es un solo `SKILL.md`. No necesita scripts, binarios ni permisos.

## Instalar

**Antigravity CLI**

    git clone https://github.com/iaguito22/good-design ~/.gemini/config/skills/good-design

**Claude Code**

    git clone https://github.com/iaguito22/good-design ~/.claude/skills/good-design

Reinicia la sesión. Se activa sola cuando pides una landing, un portfolio, un panel
o cualquier interfaz que una persona vaya a mirar, y también cuando dices que algo
"parece hecho con IA", "parece vibecoded" o "es genérico". Para forzarla:
`/good-design`.

## Licencia

MIT.
