# 🎸 Bass & Guitar Tab Trainer

A practice player for plain-text bass and guitar tabs. Paste or upload a tab, set the tempo, and play along with a metronome while a line moves through each bar.

> Single `index.html` · no build step · no dependencies

---

## Quick start

1. Open `index.html` in a browser.
2. Open **Add your tab**, then paste a tab or upload a `.txt` file.
3. Set the **BPM** (or tap along with the recording) and press **Play**.
4. Drag across the bars you want to practice to loop them.

---

## Features

### Practice
- **Metronome** with adjustable BPM, beats per bar, accented downbeat, count-in and tap tempo
- **Moving playhead** that follows the bar in time, with optional auto-scroll to keep it in view
- **Speed control** (40–120%) for slow practice
- **Speed trainer** that adds 5% each loop pass, up to 100%

### Looping
- Drag across bars (or shift-click) to loop them
- Loop **1 / 2 / 4 / 8** bars from the current bar
- Set the start and end with **Start here** / **End here**
- Shift the loop a bar at a time with **‹ ›**
- Loop a whole section with **Loop this section**

### Playback
- **Bass tones**: fingerstyle, pick, synth, clean
- **Guitar tones**: clean, overdrive, nylon
- **Bass and guitar tabs**: 4–5 string tabs play as bass and 6+ strings as guitar, or set the instrument yourself
- **Alternate tunings** like drop D and E♭ are read from the string names
- **Chords**: stacked notes play together (guitar chords are strummed) and are named above the tab, like `Em` or `C/G`. A line of chord names above a tab is lined up with its bars.
- **Long lines**: a tab line much longer than a normal bar plays as several bars
- **Note snapping** to 8ths, 16ths or triplets
- **Sync offset** for audio delay (useful with Bluetooth headphones)

### Finding tabs
- Type a song name to open search results on **Songsterr**, **Ultimate Guitar** or the web, then paste the tab in
- Switch between the **Bass** and **Guitar** part. If a tab has both, only the selected part is shown and played.

Your tab and settings are saved in the browser.

---

## Playing techniques

Joined notes change the pitch of the ringing note instead of plucking again.

| Technique | Written as |
|---|---|
| Hammer-on / pull-off | `h` `p` |
| Slide | `/` `\` `s` |
| Bend | `b`, or `7b9` to bend up to a target |
| Release | `r` or `(7)` |
| Vibrato | `~` |
| Muted note | `x` |

**Bend sizes:** `1/2`, `½` or `full` in the tab is followed. Unmarked bends go to the next note in the song's key (detected from the tab), or you can force half or full steps in **Settings**.

---

## Tab format

Standard ASCII tab, one line per string, with `|` as bar lines:

```
G|----------------|
D|------------2---|
A|--------2-------|
E|0---0-----------|
```

- Lines like `[Verse]` above a group of tab lines become section labels.
- Tunings come from the string names (`Eb|`, `D|`). If a name looks like a typo (strings too close or too far apart), the standard interval is used instead.
- Upload accepts plain-text files (`.txt`, `.tab`). Guitar Pro and PDF files aren't supported; copy the tab out as text first.
- Text tabs don't record note lengths, so timing comes from note spacing. Each bar's notes are fitted to the beat grid, which handles the usual padding dashes.

---

## Keyboard

| Key / action | Does |
|---|---|
| `Space` | Play / stop |
| `L` | Loop on / off |
| `[` / `]` | Set the loop start / end at the current bar |
| Click a bar (or focus it and press `Enter`) | Start from that bar |
| Drag across bars (or shift-click) | Loop those bars |

---

## Hosting on GitHub Pages

1. Go to **Settings → Pages** in the repo.
2. Set the source to the `main` branch and `/ (root)`, and save.
3. The player will be at `https://<your-username>.github.io/<repo-name>/`.

---

## Tabs

The repo only ships original example riffs. Get song tabs from a licensed source such as [Songsterr](https://www.songsterr.com) or [Ultimate Guitar](https://www.ultimate-guitar.com).
