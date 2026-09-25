# Pulse Lab

A music-reactive visualizer that runs in your browser. Built with plain HTML, CSS, Canvas and the Web Audio API. No build step, account, API keys, or runtime dependencies.

## Features

- Orbit, spectrum and waveform views
- A synthesized demo beat
- Local audio files (MP3, WAV and other formats supported by your browser)
- Microphone visualization without speaker feedback
- Sensitivity and playback volume controls
- Remembered settings, responsive layout, and light/dark themes

Audio is processed on your device. This app does not upload or record audio. The volume control affects music and demo playback; it does not change microphone capture volume.

## Run locally

Open `index.html` directly for demo and file playback, or serve this folder:

```sh
python -m http.server 8000 --bind 127.0.0.1
```

Then open <http://localhost:8000>. Microphone access needs a supported browser, permission, and a secure context such as localhost or HTTPS. Click **Stop** to release the microphone.

## GitHub Pages

This project can be hosted directly from the root of the `main` branch. There is no build command. The site must use HTTPS for microphone access.

## Files

- `index.html`: page and accessible controls
- `styles.css`: responsive styles and themes
- `app.js`: audio sources, settings, and visual rendering

The project started as an interactive chat visualization and has been exported and adapted to run independently. It has no dependency on the chat application.
