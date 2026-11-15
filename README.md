# Pad Looper

A single-page browser looper for a 25-key MIDI controller with 8 pads and 8 knobs (built around the Akai MPK mini).
Open `index.html` in Chrome or Edge, click to start, and allow MIDI (and the microphone if you want to record your voice).

## Controls

- **Record:** press the lowest key, then a pad. Play, then hit the pad again to stop. The mic is recorded together with the keys.
- **Play:** hit a pad that has a recording.
- **Loop:** press the highest key, then a pad. Hit the pad again to stop.
- **Volume:** each knob sets the volume of the pad in the same position.
- **Sounds:** pick an instrument from the row under the title (piano, synths, drums, and some silly and sci-fi ones).
- **Record to file:** the header button records everything you hear plus the mic and downloads it as a WAV.

The lowest and highest key follow octave shifts. Key, pad channel and knob assignments can be changed in the ⚙ menu.
Without a controller: keys A–J play notes, 1–8 are pads, R and L are the record and loop keys.

## Running from a local server (optional)

```bash
python -m http.server 8770 --bind 127.0.0.1
```

Then open http://localhost:8770.
