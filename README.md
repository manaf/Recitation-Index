# Recitation-Index

Master manifest for the recitations served to the Mushaf mobile app.

The app fetches `reciters.json` on first launch (via jsDelivr) and uses
it to populate the reciter picker. Each entry carries the URL pattern
for fetching that reciter's segment JSONs from the `Recitations` repo.

Audio MP3s themselves are NOT in `Recitations` — the JSONs contain
`audio_url` fields pointing to public CDNs (`audio-cdn.tarteel.ai`,
`download.quranicaudio.com`).

## URL

```
https://cdn.jsdelivr.net/gh/manaf/Recitation-Index@main/reciters.json
https://raw.githubusercontent.com/manaf/Recitation-Index/main/reciters.json
```

## Source

Recitation data mirrored from [QUL](https://qul.tarteel.ai). See
`scripts/recitation/` in the mushaf app repo for the import scripts.
