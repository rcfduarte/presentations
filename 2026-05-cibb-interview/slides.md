---
theme: cnc-v2
title: Glutamatergic Signaling in Health and Aging
info: |
  CiBB-PostDoc IT057-26-5 interview backup walk-through deck. 25 May 2026.
fonts:
  provider: none
canvasWidth: 1920
aspectRatio: 16/9
transition: fade
download: false
highlighter: shiki
shiki:
  theme: rose-pine-dawn
layout: title
subtitle: Computational Models Linking Receptor Function to Cellular Plasticity Across Neural and Endocrine Tissue
speaker: Renato C. F. Duarte · CNC-UC / CiBB · University of Coimbra · 25 May 2026
---

<template #subtitle>

Computational Models Linking Receptor Function to Cellular Plasticity Across Neural and Endocrine Tissue

**Collaborating groups**:  Synapse Architecture (Joana Ferreira, MIA-Portugal)  ·  Mitochondrial Biology in Aging and Disease (Quan Zhang, CNC-UC / Oxford)

</template>

<template #contact>

  <ContactItem icon="email" href="mailto:renato.duarte@cnc.uc.pt">renato.duarte@cnc.uc.pt</ContactItem>
  <ContactItem icon="website" href="https://comp-neuro.org">comp-neuro.org</ContactItem>

</template>

<template #logos>

  <img :src="'/logos/cnc.svg'" alt="CNC" style="height:56px" />
  <img :src="'/logos/cibb.svg'" alt="CiBB" style="height:56px" />
  <img :src="'/logos/uc.png'" alt="UC" style="height:56px" />
  <img :src="'/logos/fct.png'" alt="FCT" style="height:56px" />

</template>

---
layout: multi-fig
slots: 2
kicker: The premise
title: Same machinery, two tissues
---

<template #narration>

Pancreatic islets and cortical microcircuits use **similar glutamate-mediated machinery** and a **similar glutamate–somatostatin feedback brake** — at radically different timescales.

</template>

<div class="fig-slot">
  <img :src="'/figures/slide2-parallel-architecture.svg'" alt="Parallel architecture: cortical vs islet" />
  <div class="caption">Parallel architecture: cortical microcircuit and pancreatic islet share the Glu→SST→feedback motif.</div>
</div>

<div class="fig-slot">
  <img :src="'/figures/slide2-kinetics-traces.svg'" alt="Kinetics: ~10 ms cortical vs ~30 s islet" />
  <div class="caption">Same motif, ~1000× timescale gap — ~10 ms in cortex, ~30 s in islet.</div>
</div>

---
layout: multi-fig
slots: 4
kicker: Section 1 — Achievements
title: Glutamate plasticity & biophysics
---

<template #narration>

15 years building biophysical models of glutamate-driven plasticity — from receptors to functional circuits.

</template>

<div class="fig-slot">
  <img :src="'/figures/slide3-quaresima2022-tripod-panel.png'" alt="Quaresima 2022 Tripod" />
  <div class="caption">Quaresima 2022 (<i>J Physiol</i>) — Tripod neuron, structural reduction of the dendritic tree.</div>
</div>

<div class="fig-slot">
  <img :src="'/figures/slide3-quaresima2025-updown-panel.png'" alt="Quaresima 2025 Up/Down" />
  <div class="caption">Quaresima 2025 — Nonlinear dendritic integration supports Up/Down dynamics.</div>
</div>

<div class="fig-slot">
  <img :src="'/figures/slide3-korcsak2024-panel.png'" alt="Korcsak 2024" />
  <div class="caption">Korcsak-Gorzo 2024 (Neuromethods, invited) — Phenomenological synaptic dynamics.</div>
</div>

<div class="fig-slot">
  <img :src="'/figures/slide3-duarte-morrison2019-panel.png'" alt="Duarte Morrison 2019" />
  <div class="caption">Duarte & Morrison 2019 (<i>PLoS Comput Biol</i>) — Circuit plasticity framework.</div>
</div>

---
layout: multi-fig
slots: 4
kicker: Section 1 — Current line (HetSyn)
title: Heterosynaptic plasticity & chemoarchitecture
---

<template #narration>

FCT PEX **HetSyn**: glutamate-driven adaptive E/I control via dendritic heterosynaptic plasticity, set within a chemoarchitectural axis framework.

</template>

<div class="fig-slot">
  <img :src="'/figures/slide4-bcm-landscape.png'" alt="BCM landscape" />
  <div class="caption">SP3 — BCM-like plasticity landscape (heterosynaptic E/I).</div>
</div>

<div class="fig-slot">
  <img :src="'/figures/slide4-spillover.png'" alt="Spillover" />
  <div class="caption">SP3 — Glutamate spillover & dendritic compartments.</div>
</div>

<div class="fig-slot">
  <img :src="'/figures/slide4-cns2026-hetsyn.svg'" alt="CNS 2026 hetsyn" />
  <div class="caption">CNS-2026 abstract — heterosynaptic adaptive E/I control.</div>
</div>

<div class="fig-slot">
  <img :src="'/figures/slide4-chemoarchitecture-axis.svg'" alt="Chemoarchitecture axis" />
  <div class="caption">Chemoarchitecture: neurotransmitter axes shape cortical computation.</div>
</div>

---
layout: two-column
kicker: Section 2 — Project rationale
title: Why islets — and why now
---

<template #text>

- **Minimal proxy** — small endocrine clusters with 3 cell types vs. cortex's billions of cells and dozens to hundreds of types. Same Glu machinery, simpler substrate.
- **Conserved feedback motif** — α→δ Glu→somatostatin→α brake, isomorphic to the cortical pyramidal→SST→pyramidal brake.
- **Electrophysiologically informative** — islet activity carries information; one tissue for computation, the other for glucose homeostasis.
- **Computationally tractable** — small enough for end-to-end biophysical modelling on GPU; cortex still requires reduction.

</template>

<template #figure>

  <img :src="'/figures/slide5-population-schematic.svg'" alt="Population schematic: islet vs cortical microcircuit" style="width:100%;" />

</template>

---
layout: single-figure
kicker: Section 2 — The plan
title: Four research questions, basic → translational
---

<img :src="'/figures/slide6-objectives-grid.svg'" alt="Four objectives" style="width:100%; height:100%; object-fit:contain;" />

---
layout: single-figure
kicker: Section 2 — Translational deliverable
title: From models to drug targets
---

<img :src="'/figures/slide7-drug-screening-pipeline.svg'" alt="Drug-screening pipeline" style="width:100%; height:100%; object-fit:contain;" />

<template #caption>

Output is **target prioritisation**, not bench discovery. The model is the filter; the experiment is the deliverable.

</template>

---
layout: single-figure
kicker: Section 3 — Future direction
title: A translational branch I have been missing
---

<img :src="'/figures/slide8-bidirectional-flow.svg'" alt="Bidirectional flow" style="width:100%; height:100%; object-fit:contain;" />

<template #caption>

Opens the clinical/translational axis the line was missing — and feeds insights **back** to cortical Glu/GABA via a more accessible substrate.

</template>

---
layout: acknowledgements
title: Team & support
---

<template #collaborators>

- **Joana Ferreira** (Synapse Architecture, MIA-Portugal)
- **Quan Zhang** (Mitochondrial Biology, CNC-UC / U. Oxford)
- **Alessio Quaresima** (U. Trento) — Tripod neuron + Up/Down work
- **Beatriz Aleixo** (PhD, CNC-UC) — SP3 heterosynaptic plasticity

</template>

<template #funding>

- **FCT PEX HetSyn** — current PI grant
- **CiBB / CNC-UC** — host institution
- **This position** — CiBB4Health+ IT057-26-5

</template>

<template #logos>

  <img :src="'/logos/cnc.svg'" alt="CNC" style="height:48px" />
  <img :src="'/logos/cibb.svg'" alt="CiBB" style="height:48px" />
  <img :src="'/logos/uc.png'" alt="UC" style="height:48px" />
  <img :src="'/logos/fct.png'" alt="FCT" style="height:48px" />

</template>

---
hide: true
layout: equation
kicker: Backup B1
title: Multi-timescale biophysical framework
---

Fast processes (ion channels, $\mu$s) → slow processes (gene expression, days), with averaged signals passed between scales.

$$
\frac{dV}{dt} = \frac{1}{C_m}\left( I_{\text{ext}} - g_{\text{Na}}(V - E_{\text{Na}}) - g_{\text{K}}(V - E_{\text{K}}) - I_{\text{syn}}(t) \right)
$$

$$
\frac{d[\text{CREB}_p]}{dt} = k_+ [\text{Ca}^{2+}]^n - k_- [\text{CREB}_p]
$$

<template #notes>

JAX-GPU accelerated. Parameter sweeps over $10^4$ conditions feasible. Slow processes updated less frequently; averaged signals passed across scales.

</template>

---
hide: true
layout: two-column
kicker: Backup B2
title: Gene-expression → electrophysiology bridge
---

<template #text>

**Camuñas-Soler 2020** (*Cell Metab* 31:272) — 1,369 islet cells with **paired** measurements:

- Single-cell RNA-seq (genome-wide expression)
- Patch-clamp electrophysiology (currents, exocytosis, action potentials)

</template>

<template #figure>

The bridge enables **direct integration of Zhang's transcriptomic experiments into the biophysical models**:

CREB activation → gene-expression changes → predicted ion-channel & receptor changes → simulated functional response → comparison to ex-vivo experiments.

Closes the loop between molecular biology and cellular function.

</template>

---
hide: true
layout: bullets
kicker: Backup B3
title: Specific drug examples
---

- **GluN2B-selective NMDA antagonists** — in Phase 3 trials for neurological indications; computationally test for **islet-protective effects** in hypoglycaemia.
- **GLP-1R agonists** (semaglutide, etc.) — approved for diabetes; computationally test for potential **neuroprotective effects** in models of repeated seizures / aging.
- **Somatostatin receptor (SSTR) subtype modulators** — potential cross-tissue intervention point.
- **CREB-pathway inhibitors** — restrict pathological positive-feedback loop; test in both tissue models.

---
hide: true
layout: concept
kicker: Backup B4
title: CREB module — converging from divergent inputs
---

**Neural side**: NMDA → Ca²⁺ → CaMK/PKA → CREB → CRTC1 → neural-gene expression

**Islet side**: AMPA + GLP-1R → Ca²⁺ → CaMK/PKA → CREB → CRTC2 → islet-gene expression

Same transcription factor, **different tissue-specific partner proteins** (CRTC1 vs CRTC2), different downstream gene sets — but the same upstream gate.

Pathological positive feedback when activation is repeated (seizures, recurrent hypoglycaemia): CREB-driven gene expression amplifies receptor-driven Ca²⁺ signalling.
