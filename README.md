# neurochem

Drop and combine neuroactive compounds on an anatomical human brain to inspect target regions, synaptic reactions, and pharmacokinetics from `0h` to `years`.

[h3manth.com/fun/neurochem](https://h3manth.com/fun/neurochem/)

```bash
python3 -m http.server 8089
```

No build step, no backend. Runs in the browser with Three.js, GLSL, and Web Audio.

```js
window.neurochem.selectCompounds(['caffeine', 'theanine', 'creatine'], 2)
window.neurochem.focusBrainRegion('cerebellum')
window.neurochem.checkStackInteraction(['ssri', 'snri'])
```

Also exposes WebMCP (`navigator.modelContext`), URL state (`?compound=caffeine,theanine&phase=2`), `llms.txt`, and `agent-card.json`.

## License

MIT © [Hemanth.HM](https://h3manth.com)
