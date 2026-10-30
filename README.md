# launchpins-data

Public data for the Launch Pins app.

`trajectories.json` lists launch directions once they're announced, keyed by
Launch Library 2 launch ID. The app uses them for the space jellyfish forecast
and visibility globe; launches not listed fall back to the app's estimate.

```json
{
  "updated": "2026-10-29T12:00:00Z",
  "launches": {
    "<launch id>": { "heading": 125, "name": "Starlink Group 6-99", "source": "Spaceflight Now" }
  }
}
```

- `heading`: compass degrees the rocket flies after liftoff (from Cape Canaveral, NE is about 45 to 56, SE about 124 to 137).
- `name`: for people reading the file.
- `source`: where the direction was announced; shown in the app.

Remove launches once they've flown to keep the file small.
