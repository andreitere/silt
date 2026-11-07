# Silt

A flow-field print studio. Particles are carried by the curl of a scalar
potential — a divergence-free field — so the ink keeps its ribbons instead of
averaging into mud. Colour is a passive scalar seeded by position, then
advected: broad bands of risograph ink that fold and marbel as they travel.

Everything is one file. No build step, no dependencies, no network at runtime
(fonts are embedded).

Open `index.html` in a browser.

## Controls

- **Move** to stir the field; **hold** to make an eddy.
- **Double-click** to drop a shockwave.
- **Drag** while holding to inject pigment.
- **New plate** reseeds the field and reprints.
- **Save print** exports a 2400 × 1600 PNG with paper margins and an edition line.
- **Hide panel** (or `H`) gives you the plate alone.

Keys: `Space` hold/release the flow · `R` new plate · `S` save · `1–5` inks ·
`M` cycle symmetry · `H` hide panel.

## Notes

- Ink weight is per-stroke alpha; lift is how fast old ink leaves the paper.
  Their ratio sets the density the plate settles into.
- Symmetry recomposes the plate and scales the particle budget so the ink
  doesn't quadruple in the corners.
- Motion respects `prefers-reduced-motion` for the interface; the artwork itself
  is the content.
