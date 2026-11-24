# Lithos Terrain: product page

The product page and documentation for **Lithos Terrain**, a procedural terrain engine with its own node editor for
Blender 5.2+: build terrains node by node, erode them with physically based simulations, start from 135 ready-made
terrains or a single Landscape node, and export every map for any engine.

This repository holds only the description, the media and the docs. The add-on itself is sold on Superhive and is not
included here.

- Product page: `index.html`, at https://blenderprocedural.github.io/lithos-terrain/
- Documentation: `docs.html`, at https://blenderprocedural.github.io/lithos-terrain/docs.html
- `images/`: the store images, the page images and the video posters; `media/`: the feature loops (MP4 and GIF)
- Inter is bundled in `fonts/`, so the pages make no external requests

## Embedding

Inside an iframe the page scales with the frame's width (the whole layout is in `rem`, and `1rem` is 1/52 of the
frame width), so its height is a fixed multiple of its width. The `aspect-ratio` style keeps the iframe exactly as tall
as the page at any column width; `height` is only a fallback. Links to other pages open in a new tab, and the page
posts its height to the parent as `{type: "lithosterrain-height", height}`.

```html
<iframe src="https://blenderprocedural.github.io/lithos-terrain/" title="Lithos Terrain" width="100%" height="HEIGHT"
  frameborder="0" style="width:100%;height:auto;aspect-ratio:832/HEIGHT;border:0;display:block"></iframe>
```

`HEIGHT` is the page height at 832 px (see `superhive/listing/description_iframe.html` in the project for the measured
value). Add `?embed=1` to the URL to preview the scaled layout outside an iframe.

## License

All renders, videos, text and code in this repository are © BlenderProcedural. All rights reserved.
