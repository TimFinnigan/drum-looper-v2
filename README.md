# Dream Looper

A browser-based loop sequencer tuned for slow, hazy, minimalist dream pop. Everything is synthesized live with the Web Audio API.

## Sound

- Soft, boxy drum machine voices: Kick, Snare, Hat, Rim
- Melodic tracks that follow the current chord: Bass, Pad (detuned saws, slow attack), Keys (organ with a little vibrato), Bell
- Slow chord loops (maj7, m7, add9) that advance each pass through the pattern
- **Mood**: Dream (major) or Haze (minor)
- **Key**: any of the 12 keys
- **Haze**: long, dark reverb
- **Tone**: warm lowpass, from dusky to open
- A dotted-eighth tape delay on everything
- Defaults to 78 BPM (range 50 to 140) with a sparse half-time starter pattern

## Controls

- **Click or drag on steps** to paint notes
- **Play** (or Space) to start and stop
- **Random** (or R) generates a new sparse pattern, keeping the same key and mood
- **Clear** resets all steps
- **Export** (or E) renders one pass per chord, plus a reverb tail, to a WAV file
- **Up / Down arrows** change BPM by 5
- **Steps** switches between 8, 16 and 32 steps

## Local Development

Open `index.html` in a modern browser. No build step and no dependencies.

## License

MIT
