# Spa Chemistry

A single-page water chemistry helper for a 290-gallon bromine hot tub, built to run on a phone.

Enter the four pad readings off an AquaDoc test strip by tapping the matching colour, and the app returns a staged dose plan: mineral base first (alkalinity, calcium), then pH, then sanitizer, with a retest timer between stages.

## Screens

- **Test** — colour-match the four pads (calcium hardness, bromine, total alkalinity, pH). A water panel shows each reading against its target with a LOW / OK / HIGH call. Targets are editable and persist on the device.
- **Plan** — the staged dose list. Each step shows the chemical, the reason, the before → after value, and the amount. Tap to check off. A retest timer sits at the bottom.
- **Chemicals** — the seven products on hand, with dose rates and handling notes.

## Targets

| Reading | Target |
| --- | --- |
| Bromine | 6–10 ppm |
| pH | 7.2–7.8 |
| Total alkalinity | 80–120 ppm |
| Calcium hardness | 250–500 ppm |

Editable in-app; overrides are stored in the browser and survive a reload.

## Running it

`index.html` is fully self-contained — open it in any browser, no build step and no server.

Published via GitHub Pages. On iOS, open the Pages URL in Safari and use Share → Add to Home Screen for a full-screen launcher.

## Dose rates

Rates marked **estimate** in the Chemicals screen are general spa ratios; the rest come off the product labels. Alkalinity and calcium doses are derived from standard chemistry (sodium bicarbonate at roughly 1½ tbsp per 10 ppm at 290 gal; calcium chloride at 2 tbsp per 10 ppm at 500 gal). The sanitizer estimates are still to be confirmed against the bottles.

Doses are guidance, not a substitute for reading the label. Add one chemical at a time, circulate, and retest.
