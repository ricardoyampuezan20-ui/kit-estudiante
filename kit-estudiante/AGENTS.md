# Instrucciones para el agente

Este proyecto es el taller "Landing page con IA" del Diplomado en Caficultura
(Túquerres, Nariño). El equipo construye una sola landing page en `index.html`
usando skills publicadas por la comunidad en GitHub.

## Cómo trabajar aquí

- Responde siempre en español, con frases cortas. El equipo no es programador.
  Las skills están escritas en inglés; el resultado se entrega en español.
- El orden es fijo: diagnóstico, página, multimedia, redes, pulido.
- Las skills están en `.claude/skills/<nombre>/SKILL.md`. Cuando el equipo diga
  "usa la skill X", lee ese archivo completo, y los que él cite, antes de actuar.

| Paso | Skill | Repositorio de origen |
|---|---|---|
| 1 Diagnóstico | `customer-research` | github.com/coreyhaines31/marketingskills |
| 2 Página | `frontend-design` y `minimalist-ui` | github.com/anthropics/skills · github.com/Leonxlnx/taste-skill-classics |
| 4 Redes | `ig-carousel`, `ig-caption`, `ig-human` | github.com/Jakeschincariol/instagram-agent-skill |
| 5 Pulido | `slopmonster` | github.com/ItsssssJack/SlopMonster |

- El archivo de voz que piden las skills de Instagram es `voice.md`, en la raíz
  de esta carpeta (no en `~/.claude/instagram/`).
- Si una skill pide ejecutar un script de Python y no hay Python instalado,
  sigue sus reglas leyendo, sin el script, y avisa.
- Antes de cambiar un archivo, di en una línea qué vas a cambiar.

## Reglas de la entrega

Estas reglas son del taller y mandan sobre cualquier skill.

1. **Sin diagnóstico no hay página.** No construyas `index.html` si `BRIEF.md`
   no tiene una persona, un problema y 3 puntos de fricción. Un punto de
   fricción es el momento exacto en que la persona se frena, duda o se rinde, y
   tiene que poder observarse.
2. **Un solo archivo** `index.html` con el CSS y el JavaScript adentro. Las
   imágenes van en `img/` con rutas relativas.
3. **Seis secciones, en este orden:**
   1. Inicio: la promesa, la persona nombrada, botón de WhatsApp, imagen principal.
   2. El problema: los 3 puntos de fricción.
   3. La solución: una respuesta por cada fricción. Ruta A: capturas y enlace
      de la app. Ruta B: producto y precio en COP.
   4. Prueba: datos reales que se puedan comprobar.
   5. En redes: un carrusel de 6 láminas 4:5 con su texto.
   6. Cierre: botón de WhatsApp y la ficha "Cómo se hizo" (integrantes,
      herramientas de IA, skills usadas con el enlace de su repositorio, prompt
      principal).
4. **Primero celular.** Se diseña para 380 px de ancho. Nada obliga a
   desplazarse hacia los lados.
5. **Un solo llamado a la acción:** escribir por WhatsApp
   (`https://wa.me/57XXXXXXXXXX?text=...`). Va en el inicio, en el cierre y fijo
   abajo en celular. Sin formularios, carrito ni registro.
6. **Pocas palabras.** Si una sección necesita más de dos frases seguidas,
   sobra texto.
7. **Nada inventado.** Ni cifras, ni testimonios, ni premios, ni
   certificaciones. El dato que falte se escribe `[falta: dato]`.

## Archivos

- `BRIEF.md`: el diagnóstico del equipo.
- `voice.md`: la voz de la marca para las piezas de Instagram.
- `index.html`: la landing.
- `img/`: `hero.jpg`, `producto.jpg`, `clip.mp4`.
- `PROMPTS.md`: los 5 prompts del taller.
