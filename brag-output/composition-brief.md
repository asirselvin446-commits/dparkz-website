# Hyperframes Composition Brief: D'PARKZ

## Objective
Create a short, polished launch-style brag video for D'PARKZ — a restaurant in Thakkamalpuram, Tamil Nadu.

## Output
- Composition directory: `brag-output/composition/`
- Rendered video: `brag-output/brag.mp4`
- Format: landscape — 1920x1080
- Duration: 20 seconds

## Source Material
- Project root: `c:\Users\asus\Downloads\Demo-Web`
- Primary files read: `index.html` (all content, CSS, JS in one file), `README.md`
- Product name: D'PARKZ
- Tagline / strongest claim: "Good food. Good company. Good memories."
- Key UI or visual moment to recreate: The warm dark palette (#1B120B night), Playfair Display serif wordmark, food photography (Dynamite Chicken, Mutton Biryani), the dining room atmosphere photo, the 4.6 rating from 5,078 reviews, and the polaroid-style gallery prints
- Copy that must appear verbatim:
  - "D'PARKZ"
  - "Restaurant · Thakkamalpuram"
  - "Where flavour meets ambience."
  - "4.6" and "from 5,078 reviews"
  - "Good food." / "Good company." / "Good memories."

## Creative Direction
- Tone preset: polished
- Creative direction: warm premium restaurant film — candlelight confidence
- Interpretation: Fewer scenes, longer holds. Restraint in motion. The serif typography and warm palette do the heavy lifting. Every transition is a slow crossfade. The food and atmosphere photography are the centrepiece, not motion tricks.
- Angle: The website *is* the walk-in. The brag video distils that experience into 20 seconds — the warm dark palette, the serif elegance, the food, the atmosphere, and the tagline. It's a restaurant that made its website feel like arriving.
- Hook: Dark screen. The D'PARKZ wordmark in Playfair Display fades in warm. "Restaurant · Thakkamalpuram" appears as a small label.
- Outro / punchline: "Good food. Good company. Good memories." in three lines, then the D'PARKZ wordmark in teal. Hold and breathe.
- Avoid:
  - Generic SaaS language ("streamline your workflow", "all-in-one platform")
  - Abstract filler visuals or gradients not from the project palette
  - Fast cuts, aggressive motion, or anything that undermines the polished warmth
  - Recreating the walk-in scroll animation literally — reference the atmosphere it creates, not the technique

## Visual Identity
- Background: #1B120B (the site's --night)
- Text: #F3E5C7 (the site's --paper-lt)
- Accent 1: #B96B3E (the site's --orange)
- Accent 2: #2F6F6B (the site's --teal)
- Secondary surface: #E8D5B0 (the site's --paper)
- Brown: #5B432E (the site's --brown)
- Display font: Playfair Display (serif, weights 400/400i/600/600i/700/700i — self-hosted in the project)
- Body font: Manrope (sans, weights 400-800 — self-hosted in the project)
- Visual references from the project:
  - The polaroid-style `.print` gallery cards (cream background, slight rotation, serif caption)
  - The grain texture overlay (fractal noise SVG pattern, 6% opacity)
  - The warm dark/paper color alternation between sections
  - The star rating display with terra (#974A28) fill

## Storyboard
Use the storyboard in `brag-output/brag-plan.md` as the creative contract.

Scene summary:
1. The Arrival — 4s — D'PARKZ wordmark + "Restaurant · Thakkamalpuram" label fade in on dark background
2. The Room — 4s — Full-bleed dining room photo with "Where flavour meets ambience." overlay
3. The Plates — 5s — Two polaroid-style dish cards (Dynamite Chicken, Mutton Biryani) arrive one by one
4. The Rating — 3.5s — Large "4.6" with stars and "from 5,078 reviews"
5. Good Memories — 3.5s — Three-line tagline + D'PARKZ wordmark in teal

## Audio
- Audio role: warm cinematic bed
- Audio arc: gentle fade-in at the opening, steady and warm through the middle scenes, gentle fade-out under the closing tagline
- Music: happy-beats-business-moves-vol-12-by-ende-dot-app.mp3
- Music treatment: volume 0.32, fade in from 0s, gentle fade-out starting ~18s. Let the music breathe under the visuals without competing.
- Music cue guidance: bundled preset at `C:\Users\asus\.gemini\config\skills\brag\assets\music\cues\happy-beats-business-moves-vol-12-by-ende-dot-app.music-cues.json`; tempo ~110 BPM. Optional timing hints: strong cue near 8.74s for first dish card (Scene 3), strong cue near 13.11s for rating reveal (Scene 4), strong cue near 17.47s for the tagline (Scene 5). Use ≤2 strong cue locks.
- Audio-reactive treatment: subtle; use music RMS/bass to make the background warmth and grain overlay breathe gently. No waveform/equalizer visuals.
- Audio-coupled moments:
  - Scene 3 / dish card landings — soft drop or wood knock, one per card
  - Scene 4 / rating reveal — single gentle bell when "4.6" appears
- SFX selection guidance: prefer warm, organic sounds (impactWood_light, interface/drop) over metallic or aggressive impacts. Maximum 3 SFX total. Consult sfx-analysis.md for low high-frequency-risk options.
- SFX analysis guidance: `C:\Users\asus\.gemini\config\skills\brag\assets\sfx\sfx-analysis.md`
- Exact SFX choice: Hyperframes should choose filenames, timestamps, density, and volume based on the implemented animation.
- Audio files: copy the chosen music and any Hyperframes-selected SFX into `brag-output/composition/assets/`

## Hyperframes Instructions
Load the composition-building Hyperframes domain skills — `hyperframes-core` (composition contract + `data-*` timing), `hyperframes-animation` (motion), `hyperframes-creative` (design spec, beats, audio-reactive), `hyperframes-keyframes` (seek-safe keyframes), and `hyperframes-cli` (lint/check/render). /brag is its own workflow: do not enter the `hyperframes` entry-point intent interview and do not route into its generic promo / launch-video workflow. Prefer native Hyperframes conventions over anything in `/brag`.

Requirements:
- Show at least one real UI, copy, or visual element from the source project.
- Keep all text readable in the final render.
- Keep the video within 15-25 seconds.
- Include the planned music/SFX layer unless audio was explicitly disabled or documented as intentionally silent.
- Treat `/brag` audio notes as guidance, not a fixed cue sheet. Choose SFX after the visual animation exists.
- Treat music cue metadata as optional timing hints. Hyperframes decides exact animation timing and should ignore cues that hurt readability, scene pacing, or the product story.
- Major reveals may move toward nearby strong cues within about 0.15s. Smaller entrances may align to nearby beat points within about 0.10s. Use only 1-2 strong cue locks in a 20s video.
- Use SFX to support motion: warm wood/drop sounds for dish card arrivals, a single bell for the rating reveal. Professional restraint — no more than 3 SFX total.
- Honor planned music treatment: gentle fade-in, steady bed, gentle fade-out under the closing tagline.
- When music is present, consider Hyperframes audio-reactive workflow: extract audio data and use RMS/bass for subtle, brand-specific motion. Good targets are the grain overlay opacity and the background warmth/vignette. Avoid waveform/equalizer visuals.
- Use local assets for audio and any required runtime/media dependencies.
- Run `hyperframes check` before render — it is brag's single gate.

## Image Assets
The following images from the project should be copied into the composition for use:
- `assets/img/photo-room.webp` — the dining room (Scene 2 background)
- `assets/img/dish-dynamite-chicken.webp` — Dynamite Chicken dish photo (Scene 3)
- `assets/img/dish-mutton-biryani.webp` — Mutton Biryani dish photo (Scene 3)
