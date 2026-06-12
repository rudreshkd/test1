# Maia's Birthday Cake 🎂

A one-page interactive birthday surprise:

1. **Blow out the candles** — uses the microphone to detect blowing (flames flicker, lean away, and go out one by one with smoke).
2. **Cut the cake** — the view switches to a higher angle, the candles are removed, and a knife appears. Drag it along the dotted guides to cut one slice; the slice slides out of the cake.
3. **Finale** — a big "Happy Birthday Maia!" with confetti raining down and balloons rising.

## Running it

The microphone only works on `localhost` or HTTPS (browsers block it on `file://`), so serve it:

```sh
cd bdaycake
python3 -m http.server 8000
```

Then open <http://localhost:8000> and allow microphone access when prompted.

**No mic?** If mic access is blocked or unavailable, the app automatically falls back to tapping each flame to blow it out.
