# Custom Emoji — Family Extension v01

Status: `generation-ready`
Use case: `logo-brand`
Reference assets: `assets/custom-emoji/masters/`

## Master prompt

Create one static Telegram Custom Emoji master on a transparent background. The new symbol must belong exactly to the attached CU club emoji family. Match its visual grammar: clean flat vector-like line icon, very dark navy shapes, consistent medium-thick white outer stroke and internal white linework, restrained signal-orange accents close to `#FC8A05`, clear outdoor-tech character and a strong silhouette that remains readable at 100×100 px.

Center the object on a square canvas and preserve the same scale and transparent padding as the references. Use sparse purposeful details only. No photorealism, plush or glossy 3D render, heavy gradients, drop shadow, background, text, letters, numbers, pseudo-logo, commercial mark or watermark.

Subject: `[ONE PRECISE MEANING]`.

Depict: `[ONE CONCRETE OBJECT OR COMPACT SCENE]`.

Use signal orange only for `[FUNCTIONAL DETAIL / ROUTE / STATE]`.

## Reference selection

Attach two or three existing masters with comparable geometry and meaning. Always include at least one simple line icon. Do not generate a new symbol without visual references from this directory.

## Production

1. Generate the high-resolution transparent master.
2. Compare it on one contact sheet with the full current pack.
3. Reject candidates with different stroke weight, excessive volume, weak small-size silhouette or inconsistent padding.
4. Export a transparent PNG exactly 100×100 px into `assets/custom-emoji/telegram-100x100/`.
5. Add the filename, meaning and one base Unicode emoji to `assets/custom-emoji/README.md`.

## Acceptance checklist

- one unambiguous meaning;
- one dominant silhouette;
- navy, white and signal orange only;
- line weight and padding match the pack;
- no text or AI-gibberish;
- transparent background;
- legible at 100×100 px in both Telegram themes;
- master and Telegram export are both committed.
