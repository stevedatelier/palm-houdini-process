# Palm

**Growth, color and a botanical identity. Maison d’Atelier.**

## Growth Tests

![Grass coverage with exposed pale surface](media/images/grass-coverage-02.webp)
![Dense grass coverage](media/images/grass-coverage-03.webp)
![Grass outline study](media/images/grass-outline-test.webp)

![Portfolio — palm technical](media/portfolio/palm-technical.webp)

The growth can get wild, but the mark still needs to read. Coverage is the main control: enough density to feel lush, enough exposed surface to keep the shape clear.

![Grass-only motion](media/gif/grass-only.gif)

<a href="media/video/grass-only.mp4">Grass-only movie</a> · <a href="docs/media-index.md#images">all five coverage studies</a>

## Sketches

![Growth sketch review](media/gif/growth-sketch-review.gif)

<sub>Growing-mushroom sketches. Creative director: Elise Fulcher.</sub>

![Supplied NATURAE foliage reference](media/images/reference-naturae.jpg)

<sub>Reference: likely <a href="https://vimeo.com/493513393">Naturae</a> by Ian Frederick. Sound by Flank Audio. Exact frame unconfirmed. <a href="docs/references.md">Source notes</a>.</sub>

<a href="media/video/growth-sketch-review.mp4">All five sketches as a still comparison</a>

The sketches are about rhythm. A uniform spread feels too even; the interest is in where the growth gathers and where it leaves a pause.

## Procedural Color

![Houdini attribute-driven color and render test](media/images/houdini-variant-color.webp)

Color variation uses the point attribute `variant`, with the Color SOP set to **Random from Attribute**. The `refine_variant` wrangles sit upstream of the color branches.

A small [VEX alternative](https://www.sidefx.com/docs/houdini/vex/functions/rand.html) for previewing colors by an existing integer `variant` attribute:

```vex
vector variant_color = rand(i@variant);
@Cd = variant_color;
```

Color changes the attitude of the mark. The brighter versions feel playful and artificial; the quieter ones put the attention back on the growth.

![Cyan variant](media/images/final-cyan.webp)
![Magenta variant](media/images/final-magenta.webp)

---
![Portfolio — palm technical](media/portfolio/palm-technical.webp)
![Portfolio — palm gallery](media/portfolio/palm-gallery.webp)

![Portfolio — palm cover](media/portfolio/palm-cover.webp)

