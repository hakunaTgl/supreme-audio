# SUPREME Audio Studio

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![JavaScript](https://img.shields.io/badge/JavaScript-ES6%2B-F7DF1E?logo=javascript)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![TensorFlow.js](https://img.shields.io/badge/TensorFlow.js-4.11-FF6F00?logo=tensorflow)](https://www.tensorflow.org/js)
[![Web Audio API](https://img.shields.io/badge/Web%20Audio-API-blueviolet)](#)
[![Live Demo](https://img.shields.io/badge/Live-Demo-brightgreen)](https://hakunatgl.github.io/supreme-audio/)

> SUPREME Audio Studio - A browser-based neural audio stem separator and production suite. Powered by TensorFlow.js, Web Audio API, Tone.js, and WaveSurfer. Maximum capability, zero server costs.

---

## Table of Contents

- [Features](#features)
- [Tech Stack](#tech-stack)
- [Quick Start](#quick-start)
- [Usage Guide](#usage-guide)
- [Project Structure](#project-structure)
- [Supported Formats](#supported-formats)
- [Roadmap](#roadmap)
- [Contributing](#contributing)
- [License](#license)

---

## Features

| Feature | Description |
|---|---|
| **Neural Stem Separation** | AI-powered isolation of Vocals, Drums, Bass, and Other stems using TensorFlow.js |
| **Multiple ML Models** | Supports Demucs and Spleeter neural network architectures |
| **Real-Time Synthesizer** | Full synthesis engine powered by Tone.js |
| **FX Processor** | Advanced digital effects chain with real-time DSP processing |
| **Spectral Analysis** | Visual harmonic and spectral audio analysis tools |
| **Waveform Visualization** | Interactive waveform display powered by WaveSurfer.js |
| **Neural AI Assistant** | Floating draggable panel with natural language + voice command support |
| **Drag & Drop Upload** | Supports MP3, WAV, FLAC, OGG, M4A files up to 500MB |
| **Per-Stem Controls** | Individual gain sliders, solo, and export for each separated stem |
| **Processing Modes** | High Quality, Balanced, and Fast neural processing options |
| **100% Client-Side** | Runs entirely in the browser - no server, no uploads, full privacy |

---

## Tech Stack

| Technology | Version | Purpose |
|---|---|---|
| **TensorFlow.js** | 4.11.0 | Neural network inference for stem separation |
| **TF Speech Commands** | 0.4.0 | Voice command recognition |
| **WaveSurfer.js** | 6.3.0 | Audio waveform visualization |
| **Tone.js** | 14.8.49 | Synthesis engine & scheduling |
| **Web Audio API** | Native | Low-level audio processing |
| **Vanilla JS (ES6+)** | - | Core application logic |

---

## Quick Start

No installation required! Open in any modern browser:

### Option 1: Live Demo
Visit the live demo: **[hakunatgl.github.io/supreme-audio](https://hakunatgl.github.io/supreme-audio/)**

### Option 2: Local Development

```bash
# 1. Clone the repository
git clone https://github.com/hakunaTgl/supreme-audio.git
cd supreme-audio

# 2. Serve locally (any static server works)
npx serve .
# OR
python -m http.server 8080
# OR
npx live-server

# 3. Open in browser
# Navigate to http://localhost:8080
```

> Note: Must be served via HTTP(S), not opened as a `file://` URL, due to Web Audio API restrictions.

---

## Usage Guide

### Stem Separation
1. Click "Neural Separator" in the sidebar
2. Drag and drop your audio file (or click to browse)
3. Select processing mode: **High Quality** | **Balanced** | **Fast**
4. Click **Process** to run neural separation
5. Use per-stem controls to solo, adjust gain, or export individual stems

### AI Assistant
- Click the floating AI panel to expand it
- Type or speak commands like:
  - `"split vocals"`
  - `"analyze audio"`
  - `"show stems"`
  - `"apply reverb"`

### Synthesizer
1. Navigate to **Synthesizer** in the sidebar
2. Use the keyboard or MIDI input to play notes
3. Adjust oscillator type, envelope (ADSR), and effects

### FX Processor
- Chain multiple effects: Reverb, Delay, Compressor, EQ, Distortion
- All processing happens in real-time via Web Audio API nodes

---

## Project Structure

```
supreme-audio/
|-- index.html          # Main application (single-file SPA)
|-- public/             # Production demo UI assets
`-- README.md
```

> The core application lives in `index.html` as a self-contained single-page app with all styles and scripts inline for maximum portability.

---

## Supported Formats

| Format | Extension | Notes |
|---|---|---|
| MP3 | `.mp3` | Most common, widely supported |
| WAV | `.wav` | Lossless, recommended for best results |
| FLAC | `.flac` | Lossless compressed |
| OGG | `.ogg` | Open format |
| M4A | `.m4a` | Apple format |

**Max file size:** 500MB

---

## Roadmap

- [x] Neural stem separation (Vocals, Drums, Bass, Other)
- [x] Real-time synthesizer
- [x] FX processor chain
- [x] Waveform visualization
- [x] AI Assistant panel with voice commands
- [x] Drag-and-drop file upload
- [x] Per-stem export
- [ ] MIDI input support
- [ ] BPM detection and time-stretching
- [ ] Beat quantization tools
- [ ] Multi-track mixer with automation
- [ ] Export to DAW project format
- [ ] Offline PWA support

---

## Contributing

Contributions are welcome!

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/your-feature`
3. Commit your changes: `git commit -m 'feat: add your feature'`
4. Push and open a Pull Request

---

## License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

---

<p align="center">Built with passion by <a href="https://github.com/hakunaTgl">hakunaTgl (Tylor Fenwick)</a> - <a href="https://hakunatgl.github.io">Portfolio</a></p>
