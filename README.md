# moving-interface-frozen-modes
Interactive visualization for “Frozen Surface Modes on a Moving Interface”. Explore 2D and 3D Fourier-space intersections between emitter spectra and dispersive modes, including frozen-mode group-velocity matching and Cherenkov-type phase matching for moving emitters and interfaces.

Interactive visualization accompanying the paper:

**Frozen Surface Modes on a Moving Interface**  
S. Azar, M. J. Bhaseen, A. V. Zayats, and F. J. Rodríguez-Fortuño

This repository hosts an interactive HTML visualization of the Fourier-space intersections and dispersion geometry discussed in the paper, with 2D and 3D views, adjustable relative velocity, emitter frequency, and medium model.

## Live interactive version

GitHub Pages:  
https://frarodfo.github.io/frozen-surface-modes/

## Contents

- `index.html` — single-file interactive visualization
- `plotly-2.35.2.min.js` — local Plotly library
- `math.min.js` — local MathJS library

## What the visualization shows

The app lets the reader explore:

- Fourier-space intersections in 2D and 3D
- emitter frame \(S\) and surface frame \(S'\)
- surface-plasmon and bulk-wave dispersion models
- the effect of relative velocity \(v/c\)
- the effect of emitter frequency \(\omega_0\)
- frozen-mode / group-velocity matching and Cherenkov-type phase matching

It is intended as an interactive companion to the dispersion figures and discussion in the manuscript.

## Usage

Open `index.html` in any modern browser.

No installation, build step, or local server is required.

The repository includes local copies of Plotly and MathJS, so the visualization works when opened directly from disk as a standalone file offline.

## Local and web use

The HTML can be used in two ways:

- **Locally:** open `index.html` directly in a browser
- **On the web:** host the same files with GitHub Pages

The repository includes local JavaScript files for Plotly and MathJS so that the visualization remains self-contained and works without relying on external CDNs. 

## Citation
If you use or refer to this interactive visualization, please cite the associated paper and the archived repository release.

### Paper
S. Azar, M. J. Bhaseen, A. V. Zayats, and F. J. Rodríguez-Fortuño,  
*Frozen Surface Modes on a Moving Interface*,  
`<journal / preprint information>`

### Interactive visualization
S. Azar, M. J. Bhaseen, A. V. Zayats, and F. J. Rodríguez-Fortuño,  
*Frozen Surface Modes — Interactive Visualization*,  
Zenodo, DOI

## Contact
Francisco J. Rodríguez-Fortuño  
francisco.rodriguez_fortuno@kcl.ac.uk
Department of Physics and London Centre for Nanotechnology  
King's College London
