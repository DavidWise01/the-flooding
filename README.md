# THE FLOODING — attention as diffusion

Attention rows sum to 1 — so an attention matrix **is** a random-walk transition
matrix, and diffusion is just the matrix raised to powers, `Aᵗ`. Pour water at one
token and watch it flow along **real BERT attention**: it **pools fast** inside a
cluster (same sees same), **trickles slow** through the necks between them. Valleys
and plateaus, made literally visible as flow. No modeling.

A single offline HTML file: system fonts only, zero network, a soft-GL 3D
diffusion-map projected by hand onto a 2D canvas, **fail-loud** diagnostics.

## What you're watching

- **2D — the flooding.** Pour at a source token; each step the water flows to
  wherever that token attends (`Aᵗ`). By `t≈16` it reaches its stationary
  distribution (dashed line). The *rate* of filling, before equilibrium, is the
  geometry. Toggle **FIELD GUIDE** to see every token's three property bars.
- **3D — the settled landscape.** Tokens placed by diffusion distance (pools
  cluster together), colored by water body, flooded by water level as it spreads.

## The taxonomy — measured, then named

Each token-basin is classified by three **measured** diffusion properties:
**movement** (escape rate `1 − Aᵢᵢ`), **depth** (stationary level `πᵢ`), and
**scale** (tributary count). Those three place each token at one of six water
bodies — *pond, pool, swamp* (static) and *creek, lake, ocean* (dynamic). **Where
each token sits is measured; the names of the regions are chosen.**

## Green substrate, amber story — both true at once

- **GREEN (verified):** real attention, exact diffusion (`Aᵗ`, mass conserved),
  exact stationary distribution (a true fixed point `π·A = π`), exact spectral
  embedding. Verified in Node.
- **AMBER (honest limits):** in head 0 the diffusion properties separate function
  words from content words sharply — function words (the, over, near) rush through
  (flow **0.96**), content words (fox, dog, river) pool (depth ~0.8). This **passes
  a shuffle test** (scramble the matrix and the separation collapses to ~0, so it
  is real structure, not an artifact of the metric). But two honest limits, stated
  on the page: it is **head-specific** (head 1 is much weaker), and this is **one
  sentence**. A real, shuffle-validated correlation in this head — **not** a
  universal law. The six water bodies are an imposed vocabulary over exact
  measurements.

Independently reproduced in Node: rows are stochastic, `π` is a true fixed point,
function-word flow = 0.96, and the depth↔content separation is real (0.70) and
collapses under shuffle (0.08), weaker in head 1 — exactly as claimed.

## Companion pieces

How attention looks as a different geometric object each time — the UD0
**Artificial Intelligence** interpretability cluster:
[THE ATTENTION HOURGLASS](https://davidwise01.github.io/attention-hourglass/) (flow
to a prediction) · [THE ATTENTION MESH](https://davidwise01.github.io/attention-mesh/)
(topology) · [THE BLACKBOARD LINEAGE](https://davidwise01.github.io/blackboard-lineage/)
(the shared workspace) · [TTU1 · Transformer Tech](https://davidwise01.github.io/ttu1/).

---
David Lee Wise / ROOT0 / TriPod LLC · CC-BY-ND-4.0
