# Drum Looper

A browser-based loop sequencer with swappable style kits. Everything is synthesized live with the Web Audio API.

Pick a kit with the **Kit** dropdown. Each kit has its own sounds, tracks, theme, tempo range, starter pattern and randomizer, and keeps its own pattern while you switch between them.

## Kits

### Classic (default)

The original drum looper: Kick, Snare, Hi-Hat, Open Hat, 808, Clap and two Toms on a neon dark grid. 60 to 200 BPM, starts empty, and Random picks a four-on-the-floor, syncopated or half-time groove.

### Dream

Slow, hazy, minimalist dream pop.

- Soft, boxy drum machine voices: Kick, Snare, Hat, Rim
- Melodic tracks that follow the current chord: Bass, Pad, Keys, Bell
- Slow chord loops (maj7, m7, add9) that advance each pass through the pattern
- **Mood**: Dream (major) or Haze (minor), and any of the 12 **Key**s
- **Chords**: Drift, Float and Sway (4 chords), Long (8 chords with a borrowed minor iv), or Wander, which random-walks through chords that sit well together so it never repeats. The pad voicing and keys arpeggio also rotate every time a progression comes around
- **Haze**: long, dark reverb. **Tone**: warm lowpass, from dusky to open
- A dotted-eighth tape delay on everything
- 50 to 140 BPM, defaulting to 78, with a sparse half-time starter pattern

## Controls

- **Click or drag on steps** to paint notes
- **Play** (or Space) to start and stop
- **Random** (or R) generates a new pattern in the active kit's style
- **Clear** resets the active kit's steps
- **Export** (or E) renders the loop to WAV (Dream renders one pass per chord, plus a reverb tail)
- **Up / Down arrows** change BPM by 5
- **Steps** switches between 8, 16 and 32 steps

## Adding a kit

A kit is one entry in the `KITS` object in `index.html`: an id, title, `tracks` (name and color), `play` (one voice function per row), a BPM range, `starter` and `randomize` functions, and a `body.kit-<id>` block of CSS variables for its theme. Kits that set `fx: true` route through the shared reverb and delay bus.

## Local Development

Open `index.html` in a modern browser. No build step and no dependencies.

## License

MIT
