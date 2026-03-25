# 🎵 Harmonium

A responsive, fully playable harmonium built with vanilla HTML, CSS, and JavaScript — no libraries, no dependencies.

Live demo: *(add your GitHub Pages link here)*

---

## Features

- **Real synthesized sound** — Web Audio API with sawtooth oscillators, detuned for that warm reed tone. Sound sustains while key is held, just like a real harmonium bellows.
- **Mobile-first vertical layout** — on phones the keyboard flips vertical and locks to full screen with zero scrolling
- **Glissando / slide** — drag your finger across keys on touch screens to play a sweep
- **Desktop keyboard mapping** — play without touching the screen

| Keys | Notes |
|------|-------|
| `A S D F G H J` | White keys (C3 – B3) |
| `W E T Y U` | Black keys (C#3 – A#3) |
| `K L ; ' \` | White keys (C4 – G4) |
| `O P ]` | Black keys (C#4 – F#4) |

- **Two octaves** — C3 to G4
- **Multi-touch** — play chords on mobile
- Zero external files, zero dependencies

---

## How it sounds

The harmonium tone is built from three sawtooth oscillators per note:
- Main oscillator at the base frequency
- Second oscillator detuned by 0.3% for a natural chorus/beating effect
- A faint octave harmonic at 2× frequency
- Low-pass filter to round off the harsh edges

This mimics how a real harmonium reed vibrates — a continuous tone that sustains as long as you hold the key.

---

## Play the song

This project was built to play **Kaayarr jo the woh shaayarr banee**. Here's the keyboard cheat sheet:

| Note | Key |
|------|-----|
| C | A |
| C# | W |
| D# | E |
| F | F |
| G | G |
| G# | Y |
| A# | U |

```
Kaayarr jo the woh shaayarr banee
E  F E  A A  A A  W  A U  U

Arzz kiyaa hai humne bhii
A  E  E  A Y  Y  Y  U

Aisee tu lage ki gulaabb hai
A A A A A  W  A U  E  W  A U
```

---

## Run locally

Just open `index.html` in any browser — no server needed.

```bash
git clone https://github.com/YOUR_USERNAME/harmonium.git
cd harmonium
# open index.html in your browser
```

---

## Built with

- HTML5
- CSS3 (Flexbox, CSS Grid, `clamp()`, `100dvh`)
- Web Audio API
- Zero dependencies

---

## License

MIT — use it, remix it, play it.
