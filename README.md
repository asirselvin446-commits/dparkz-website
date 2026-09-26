# D'PARKZ — official website

One page, one file: `index.html` holds all the content, styling and behaviour.
The only other files are images:

```
index.html
assets/img/   dish photos, room photos, storefront
assets/seq/   150 frames for the walk-in (f000.webp … f149.webp)
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
