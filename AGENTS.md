# AGENTS.md — Wow RPG Lore (Campaign Vault)

Repositorio de campaña de D&D ambientada en el mundo de Warcraft (World of Warcraft), pensado para usarse como vault de **Obsidian**. No es código: es material de juego (lore, lugares, personajes, facciones, sesiones).

## Propósito

Ferran (el DM) pasa textos largos con información de campaña. Yo me encargo de **distribuir, estructurar y enlazar** esa información en las carpetas y notas correctas para que sea legible, escaneable y fácil de navegar en Obsidian.

## Estructura de carpetas

| Carpeta | Contenido |
|---|---|
| `00_Pre_Campanya/` | One-shot de testeo (Azeroth clásico, oficial). **Sin wikilinks** salvo imágenes. Separada del canon de la campaña: no cruza enlaces con `01`-`06`. |
| `01_Sesiones/` | Guiones narrativos por sesión: escenas, entradas, descripciones leídas en voz alta, secuencias de eventos. |
| `02_Places/` | Notas de lugares: ambientación, características, personajes asociados, lugares de interés. |
| `03_Personages/` | Fichas de personajes (NPC principalmente, pero también aliados/enemigos clave). |
| `04_Lore_and_Items/` | Lore general, objetos mágicos, artefactos, rituales, pruebas. |
| `05_imagenes/` | Imágenes generadas (escenarios, retratos, mapas). No editar salvo petición. |
| `06_Facciones/` | Notas de facciones y organizaciones políticas/religiosas. |
| `Ideas sueltas.md` | Notas rápidas sin clasificar. Cuando una idea madure o se use, moverla a su carpeta definitiva. |

## Convenciones de formato

- **Idioma:** Todo el contenido del repo en castellano.
- **Wikilinks:** Usar `[[Nombre de la Nota]]` para enlazar notas relacionadas. No rodees los wikilinks con backticks.
- **Nombre de archivos:** Nombre de la entidad en castellano (ej. `Jaina Valiente.md`, `Lordaeron.md`, `El Foso de las Mareas.md`). Un archivo por entidad.
- **Texto para leer en voz alta:** Entre bloques de cita con `>` (el estilo existente usa `> >`), con la etiqueta **Texto de Ambientación (Para leer en voz alta):** y el cuerpo en *cursiva*.
- **Secciones:** Separar con encabezados y emojis temáticos según el tipo de nota (ver plantillas abajo).
- **Información solo del DM:** Marcar siempre con el emoji `🎭` y la etiqueta **Secretos (¡Solo DM!)**. Nunca mezclar secretos con información que pueda leer el jugador sin avisar.
- **Contenido pendiente:** Usar el patrón `Por escribir` o `(Por expandir — ...)` para huecos a rellenar más adelante. No inventar contenido: si Ferran no lo ha dicho, no se escribe.

## Plantillas por tipo de nota

### Lugares y facciones (`02_Places/`, `06_Facciones/`)

```
> > **Texto de Ambientación (Para leer en voz alta):** _..._
> >
> > **Características Clave:**
> > - ...
> >
> > **Personajes Notables:**
> > - [[Personaje]] - ...
> >
> > **Lugares de Interés:**
> > - ...
> >
> > **🎭 Secretos ... (¡Solo DM!):**
> > - ...
```

### Personajes (`03_Personages/`)

```
**Ubicación:** [[Nota]] **Facción:** [[Nota]] **Raza:** ...

#### 👁️ Apariencia y Actitud
- ...
#### 🎭 Guía de Interpretación (Para el DM)
- ...
#### 🗣️ ¿Qué sabe y puede contar?
- ...
```

### Sesiones (`01_Sesiones/`)

Narrativa en prosa, enlazando notas de lugares/personajes con `[[...]]` la primera vez que aparecen. Terminar con las opciones o ganchos que quedan abiertos para los jugadores.

## Flujo de trabajo al recibir texto largo

1. **Leer y entender** el texto completo antes de tocar nada.
2. **Detectar entidades:** lugares, personajes, facciones, objetos, eventos de sesión.
3. **Distribuir:** crear o actualizar la nota correcta en la carpeta adecuada; enlazarla con `[[...]]` a las notas relacionadas (y enlazar de vuelta cuando proceda).
4. **Estructurar:** dividir en las secciones de la plantilla que aplique. Texto largo para leer en voz alta => bloque de cita. Información de fondo => listas y viñetas.
5. **Respetar lo que ya existe:** no reescribir notas previas por el simple placer de pasarlas al nuevo formato; conservar el contenido de Ferran y su estilo.
6. **Separar el secreto del jugador:** lo que solo conoce el DM va a la sección `🎭 ... (¡Solo DM!)` o, si aplica, a una nota diferenciada.
7. **Consolidar `Ideas sueltas.md`:** si el texto resuelve o materializa una idea, moverla a la nota definitiva.

## Git

- **Rama:** `main` es la única rama. Commits directos a `main` y `push` a `origin`.
- **Mensajes de commit en castellano,** descriptivos y en la línea del historial existente (ej. "Añade las 4 facciones del tablero político...", "Crea notas esqueleto...", "Corrige errata...").
- **Un commit por bloque de trabajo coherente** (ej. una sesión, una facción, un conjunto de notas esqueleto).
- Hacer `pull` antes de trabajar si el repo tiene movimientos externos.
- Al terminar cada bloque de trabajo, commitear siempre y hacer `push` a `origin/main`.

## Reglas duras

- No inventar lore. Si la información es ambigua o falta, dejar hueco con `Por escribir` y/o preguntar a Ferran.
- No usar backticks alrededor de los `[[wikilinks]]`.
- Todo el contenido y los commits en castellano.
- Preservar los emojis de sección existentes (👁️ 🎭 🗣️) y los bloqueos de ambiental `> >`.
