# Bass & Guitar Tab Trainer

A practice player for plain-text bass and guitar tabs. Paste or upload a tab, set the tempo, and play along with a metronome while a line moves through each bar.

It's a single `index.html` with no build step and no dependencies.

## Features

- **Metronome** with adjustable BPM, beats per bar, accented downbeat, count-in and tap tempo
- **Moving playhead** that follows the bar in time, with optional auto-scroll to keep it in view
- **Speed control** (40–120%) for slow practice, and **looping** over a range of bars
- **Tab playback** with bass tones (fingerstyle, pick, synth, clean) and guitar tones (clean, overdrive, nylon)
- **Bass and guitar tabs**: 4–5 string tabs play as bass and 6+ strings as guitar, or set the instrument yourself. Alternate tunings like drop D and E♭ are read from the string names.
- **Playing techniques**: hammer-ons and pull-offs (`h` `p`), slides (`/` `\` `s`), bends (`b`, or `7b9` to bend up to a target), releases (`r` or `(7)`), vibrato (`~`) and muted notes (`x`). Joined notes change the pitch of the ringing note instead of plucking again.
- **Chords**: stacked notes play together (guitar chords are strummed) and are named above the tab, like `Em` or `C/G`. A line of chord names above a tab is lined up with its bars.
- **Long lines**: a tab line much longer than a normal bar plays as several bars
- **Looping**: drag across bars (or shift-click) to loop them, loop 1/2/4/8 bars from the current bar, set the start and end with **Start here** / **End here**, shift the loop a bar at a time, or loop a whole section with **Loop this section**. Optional speed trainer adds 5% each pass up to 100%.
- **Bend sizes**: `1/2`, `½` or `full` in the tab is followed. Unmarked bends go to the next note in the song's key (detected from the tab), or you can force half or full steps.
- **Tab search**: type a song name to open search results on Songsterr, Ultimate Guitar or the web, then paste the tab in
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
- Tunings come from the string names (`Eb|`, `D|`). If a name looks like a typo (strings too close or too far apart), the standard interval is used instead.
- Upload accepts plain-text files (`.txt`, `.tab`). Guitar Pro and PDF files aren't supported; copy the tab out as text first.
- Text tabs don't record note lengths, so timing comes from note spacing. Each bar's notes are fitted to the beat grid, which handles the usual padding dashes.

## Keyboard

- **Space**: play / stop
- **L**: loop on / off
- **[** and **]**: set the loop start / end at the current bar
- **Click a bar** (or focus it and press Enter): start from that bar
- **Drag across bars** (or shift-click): loop those bars

## Tabs

The repo only ships original example riffs. Get song tabs from a licensed source such as [Songsterr](https://www.songsterr.com) or [Ultimate Guitar](https://www.ultimate-guitar.com).
