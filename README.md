# D'PARKZ — official website

One page, one file: `index.html` holds all the content, styling and behaviour.
Everything else is media, fonts and the animation libraries, all served from this site (no third-party CDNs):

```
index.html
assets/img/     photos as WebP, each with a -sm phone size (storefront.jpg is the link preview)
assets/walk/v2/  the 150 walk-in frames: hd/ 1920px, md/ 1280px, sm/ 720px (phones load every second one).
                 Change the folder name (v3, ...) whenever the frames change, because assets are cached for a year.
assets/vendor/  GSAP 3.12.5, ScrollTrigger, Lenis 1.1.13 (self-hosted, no CDN)
assets/fonts/   Playfair Display and Manrope (self-hosted)
vercel.json     long-term caching for everything in assets/
```

## Sections

1. Walk-in: the frames follow the scroll; the page continues only after the last frame
2. Our story, signature dishes, what we serve
3. The plates: pinned sideways scroll, then the full list with photo previews
4. The atmosphere
5. Gallery
6. Visit: rating, storefront, address, phone, Call and Get directions
7. Closing statement and footer

## Hosting

Upload the folder to any static host (Netlify, Vercel, GitHub Pages, cPanel). To preview locally:

```
python -m http.server 8080
```

## Still to supply

- Blue Blossom Milkshake photo (currently an illustration)
- Logo file (the typed "D'PARKZ" wordmark is used for now)
- Replace AI-generated visuals with real photography before launch if they are not the actual restaurant
