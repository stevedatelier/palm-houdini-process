# Palm

**Growth, color and a botanical identity. Maison d’Atelier.**

## Growth Tests

![Grass coverage with exposed pale surface](media/images/grass-coverage-02.webp)
![Dense grass coverage](media/images/grass-coverage-03.webp)
![Grass outline study](media/images/grass-outline-test.webp)

![Portfolio — palm technical](media/portfolio/palm-technical.webp)

Coverage tests for the Palm mark. The balance is between dense growth and enough breathing room for the shape to work.

![Grass-only motion](media/gif/grass-only.gif)

<a href="media/video/grass-only.mp4">Grass-only movie</a> · <a href="docs/media-index.md#images">all five coverage studies</a>

## Sketching

![Growth sketch review](media/gif/growth-sketch-review.gif)

![Supplied NATURAE foliage reference](media/images/reference-naturae.jpg)

<sub>Reference: likely <a href="https://vimeo.com/493513393">Naturae</a> by Ian Frederick. Sound by Flank Audio. Exact frame unconfirmed. <a href="docs/references.md">Source notes</a>.</sub>

<a href="media/video/growth-sketch-review.mp4">All five sketches as a still comparison</a>

A short comparison of the growth sketches.

## Procedural Color

![Houdini attribute-driven color and render test](media/images/houdini-variant-color.webp)

Color variation uses the point attribute `variant`, with the Color SOP set to **Random from Attribute**. The `refine_variant` wrangles sit upstream of the color branches.

A small [VEX alternative](https://www.sidefx.com/docs/houdini/vex/functions/rand.html) for previewing colors by an existing integer `variant` attribute:

```vex
vector variant_color = rand(i@variant);
@Cd = variant_color;
```

The brighter palettes give the project a playful side. The quieter versions leave more room for the growth itself.

![Cyan variant](media/images/final-cyan.webp)
![Magenta variant](media/images/final-magenta.webp)

---
![Portfolio — palm technical](media/portfolio/palm-technical.webp)
![Portfolio — palm gallery](media/portfolio/palm-gallery.webp)

![Portfolio — palm cover](media/portfolio/palm-cover.webp)

