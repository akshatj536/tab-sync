# Bass & Guitar Tab Trainer

A practice player for plain-text bass and guitar tabs. Paste or upload a tab, set the tempo, and play along with a metronome while a line moves through each bar.

It's a single `index.html` with no build step and no dependencies.

## Features

- **Metronome** with adjustable BPM, beats per bar, accented downbeat, count-in and tap tempo
- **Moving playhead** that follows the bar in time and scrolls the page
- **Speed control** (40–120%) for slow practice, and **looping** over a range of bars
- **Tab playback** with bass tones (fingerstyle, pick, synth, clean) and guitar tones (clean, overdrive, nylon)
- **Bass and guitar tabs**: 4–5 string tabs play as bass and 6+ strings as guitar, or set the instrument yourself. Alternate tunings like drop D and E♭ are read from the string names.
- **Note snapping** to 8ths, 16ths or triplets, and a sync offset for audio delay (useful with Bluetooth headphones)
- Your tab and settings are saved in the browser

## Run it

Open `index.html` in a browser. Nothing to install.

To host it on GitHub Pages: push the repo, then go to **Settings → Pages**, set the source to the `main` branch and `/ (root)`, and save. The player will be at `https://<your-username>.github.io/<repo-name>/`.

## Tab format

Standard ASCII tab, one line per string, with `|` as bar lines:

```
G|----------------|
D|------------2---|
A|--------2-------|
E|0---0-----------|
```

- Lines like `[Verse]` above a group of tab lines become section labels.
- Upload accepts plain-text files (`.txt`, `.tab`). Guitar Pro and PDF files aren't supported; copy the tab out as text first.
- Text tabs don't record note lengths, so timing comes from note spacing. Each bar's notes are fitted to the beat grid, which handles the usual padding dashes.

## Keyboard

- **Space**: play / stop
- **Click a bar** (or focus it and press Enter): start from that bar

## Tabs

The repo only ships original example riffs. Get song tabs from a licensed source such as [Songsterr](https://www.songsterr.com) or [Ultimate Guitar](https://www.ultimate-guitar.com).
