## assets/icon.png
- Date: 2026-10-30
- Tool and model: Codex CLI 0.164.0 / built-in image generation (model id not reported by the tool)
- Seed: not supported
- Reference images: none
- Prompt:

```text
Use your image generation capability to create ONE image. Do not modify any other files.

NEON NIGHT REPO ICON · Pick-Your-AI/pick-your-ai-market

Create one square 1024 × 1024 px image of a single repository glyph.
Use a simple geometric silhouette with a luminous outline and one accent spark.
Keep the background empty and the glyph inside the central 688 × 688 px square.
Size class SQUARE: a squarish glyph about 600 to 660 px on each side.

GLYPH: market radar scope. A round radar scope with concentric rings and a sweeping beam, with three small competitor blips of different sizes scattered across the rings, reading as market research and competitive positioning
SPARK PLACEMENT: one bright spark on the largest blip at the upper right of the scope
PALETTE: outline #0F766E, glow #14B8A6; one spark in #FBBF24.
The spark is the only filled shape and the only element in #FBBF24; keep the
glyph outline in #0F766E so the spark remains distinct at small sizes.

No text, letters, numbers, words, logos, brand marks, human figures or third-party IP.

Produce four candidates. Use the tool's default seed.
The lock pass renders assets/icon.png as a flat glyph in the family's light-surface
inks, without a tile or glow. Do not render the repository name in the image.

Negative list: no background tile, no frame, no gradient backdrop, no text, no letters, no numbers, no watermark, no photo realism, no extra icons, no blue.
Palette hex values: every stroke exactly flat #0F766E (RGB 15,118,110), glow #14B8A6, single spark flat #FBBF24. Plain pure white background, glyph inside the central 688 x 688 px square with generous empty margin. Aspect ratio 1:1, 1024x1024.

REVISION: the previous attempt had hand-drawn wobble and texture that bloated the file. Draw clean vector-style geometry: perfectly smooth circles, uniform stroke width, solid flat fills, hard edges, no paper grain, no noise, no brush texture, no shading. Keep the shapes few and bold: outer ring, two inner rings, centre dot, one sweep line, three blips, one spark.
```

- Candidates: 1 per attempt, 2 attempts; selected: attempt 2 (reason: attempt 1 hand-drawn wobble, failed icon-budget on auto ground; attempt 2 cleaner geometry, passed with --ground transparent)
- Post-processing: showcase.py 1.0.0 content icon normalize --ground transparent; output sha256 056f61ac0a8a82ab11fbf16769f86c30b825d117c2b726d6ed198f49bb394501; size 248 KB
