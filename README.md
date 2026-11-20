# neurochem

Drop and combine neuroactive compounds onto an anatomical human brain to see where they act, how they spread, and what changes from hour zero to years.

```bash
python3 -m http.server 8089
```

Open `http://localhost:8089` and tap any compound pill. Zero build step, zero backend, runs in your browser with Three.js and Web Audio.

## What it renders

- Segmented anatomical brain with photographic cortical gyri, deep sulci, cerebellum, thalamus, midbrain, pons, plus sculpted bilateral hippocampus, amygdala, and striatum
- Two-pass depth-prepass frosted glass cortex so activated deep structures glow cleanly inside without alpha-sorting artifacts
- Custom GLSL volumetric wavefront that spreads across the folded prefrontal cortex on impact, paired with live action-potential arcs and synaptic cleft bursts
- Five-stage pharmacokinetic timeline (`0h Ingestion`, `1h Early`, `Peak Tmax`, `t1/2 Clearance`, `Years Chronic`) with auto-play harmonic chimes

## Combining stacks

Tap `+ Combine` (or Shift-click any pill) to layer up to 4 compounds at once, or try a preset like Caffeine + L-Theanine or the Focus Trio (Caffeine + L-Theanine + Creatine). Overlapping brain structures blend colors in real time and surface synergy notes or clinical cautions (for example SSRI + SNRI serotonin risk or Lithium + Psilocybin seizure risk).

## Deep links and WebMCP

```js
// Control the brain directly from an agent or browser console
window.neurochem.selectCompounds(['caffeine', 'theanine', 'creatine'], 2)
window.neurochem.focusBrainRegion('cerebellum')
window.neurochem.checkStackInteraction(['ssri', 'snri'])
```

URL state works out of the box too: `?compound=caffeine,theanine&phase=2`. Tools are also registered on `navigator.modelContext` alongside `llms.txt`, `llms-full.txt`, and `agent-card.json`.

## Compounds included

- SSRIs (Escitalopram)
- SNRIs (Venlafaxine)
- Caffeine
- L-Theanine
- Creatine Monohydrate
- Stimulants (Methylphenidate)
- Psilocybin (Psilocin)
- Magnesium L-Threonate
- Ketamine / Esketamine
- Lithium

## License

MIT © [Hemanth.HM](https://h3manth.com)
