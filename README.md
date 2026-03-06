IFS Fractal Generator and Animator
======

> "In mathematics, iterated function systems or IFSs are a method of constructing fractals; the resulting constructions are always self-similar."
> -- Wikipedia (<http://en.wikipedia.org/wiki/Iterated_function_system>)

An interactive WebGL fractal generator and animator which uses Iterated Function Systems (IFS) to generate the fractals.

Inspired by [this paper](http://www.inf.uni-konstanz.de/gk/pubsys/publishedFiles/WiSa04.pdf).

Originally created by **sirxemic** – see the original project and demo at <http://sirxemic.github.io/ifs-animator>.  
This fork focuses on a modernized UI and a richer preset experience, while keeping the core IFS implementation intact.

## Demo

You can still use the original demo above for reference; the forked version keeps the same interaction model with an updated layout.

## Features in this fork

- **Modern layout and visuals**
  - White, gradient background with a card-like fractal viewport.
  - Responsive split layout: large fractal canvas on the left, controls in a right-hand sidebar (stacked on smaller screens).
  - Refreshed toolbar and sidebar styling for a more contemporary look.

- **Preset “Frame Properties”**
  - New **Presets** panel in the sidebar with a dropdown and **Apply preset** button.
  - Predefined IFS frame configurations for:
    - Sierpinski triangle  
    - Sierpinski carpet  
    - Koch snowflake  
    - Cantor set  
    - Dragon curve  
    - Pythagoras tree  
    - Hilbert curve (approximate IFS-style variant)  
    - Peano curve (approximate)  
    - Pascal’s triangle / Sierpinski variation  
    - Mandelbrot-style IFS  
    - Julia-style IFS  
    - Lorenz-attractor-style IFS  
    - Menger-sponge-style IFS (2D projection)  
    - L-system-style tree  
    - Weierstrass-style rough curve  
  - Applying a preset:
    - Replaces the current IFS frames with a preset configuration.
    - Adjusts brightness per preset and re-centers the fractal using the existing `Fit to screen` logic.

- **Non-intrusive changes**
  - Core IFS math, animation, and rendering code are unchanged from the original project.
  - All additions live in the UI/layout layer plus a preset configuration object.
  - The “Fork me on GitHub” ribbon has been removed to keep the canvas area clean.

## Controls (unchanged from original)

Most controls should be pretty self-explanatory, except for the canvas itself:

- Move the frames by dragging their origins with the left mouse button.
- Rotate and scale the frames by dragging the end points with the left mouse button. Hold shift to just scale.
- Drag the points of the frames with the right mouse button to skew them.
- Use left mouse button, right mouse button and scroll wheel respectively to pan, rotate and zoom the scene.

## Example fractals (original links)

- [Sierpinski Triangle](http://sirxemic.github.io/ifs-animator/#1.1|100|0.9719|0|0|0.9719|-0.4765|-0.4991|100|3|0.5|0|0|0.5|0.25|0.5|95|32|71|149|0.5|0|0|0.5|0.5|0|35|26|84|80|0.5|0|0|0.5|0|0|52|61|15|55|)
- [Barnsley Fern](http://sirxemic.github.io/ifs-animator/#1.87|100|0.0914|0.0181|-0.0181|0.0914|-0.2166|-0.4614|100|4|0.85|0.04|-0.04|0.85|0|1.6|74.2637|84.6678|0.9183|89|0.2|-0.26|0.23|0.22|0|1.6|72.8376|76.4132|45.4947|74|0.01|0|0|0.16|0|0|83|56|4|94|-0.15|0.28|0.26|0.24|0|0.44|42|7|57|58|)
- [The Dragon Curve](http://sirxemic.github.io/ifs-animator/#1.24|100|0.6498|0|0|0.6498|-0.3187|-0.0122|100|2|0.5|-0.5|0.5|0.5|0|0|8|20|66|87|-0.5|0.5|-0.5|-0.5|1|0|90|99|95|122|)