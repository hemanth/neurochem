# neurochem

Drop and combine neuroactive compounds onto an anatomical human brain to see where they act, live synaptic reactions, and how effects shift from hour zero to years.

Live at [h3manth.com/fun/neurochem](https://h3manth.com/fun/neurochem/).

```bash
python3 -m http.server 8089
```

Zero build step, zero backend. Three.js, custom GLSL, and Web Audio.

## How it works

- 8 real anatomical structures: folded prefrontal cortex, cerebellum, thalamus, midbrain, pons, hippocampus, amygdala, and striatum
- 5 timeline stages: `0h`, `1h`, `Peak (Tmax)`, `t1/2`, and `Years` with auto-play harmonic chimes
- Multi-compound stacking (`+ Combine` or Shift-click): blends overlapping regions and flags synergies or clinical cautions (SSRI + SNRI, Lithium + Psilocybin, Caffeine + L-Theanine, Focus Trio)
- Live action-potential arcs and synaptic cleft bursts scaled to each phase

## Agent API and deep links

```js
window.neurochem.selectCompounds(['caffeine', 'theanine', 'creatine'], 2)
window.neurochem.focusBrainRegion('cerebellum')
window.neurochem.checkStackInteraction(['ssri', 'snri'])
```

Also exposed via WebMCP (`navigator.modelContext`), URL params (`?compound=caffeine,theanine&phase=2`), `llms.txt`, and `agent-card.json`.

## Compounds

SSRIs, SNRIs, Caffeine, L-Theanine, Creatine, Stimulants, Psilocybin, Mg Threonate, Ketamine, Lithium.

## License

MIT © [Hemanth.HM](https://h3manth.com)
