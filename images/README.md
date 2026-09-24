# Property photos

Real photos are in place, sourced from the "Torrance photos" folder on Justin's Desktop
(originally HEIC, converted to JPG and resized to 2000px wide for web use).

| File | Used for |
|---|---|
| `hero-exterior.jpg` | Hero background |
| `front-exterior.jpg` | Gallery — Front Exterior |
| `living-room.jpg` | Gallery — Living Room |
| `kitchen.jpg` | Gallery — Kitchen |
| `primary-bedroom.jpg` | Gallery — Primary Bedroom |
| `primary-bathroom.jpg` | Gallery — Primary Bathroom |
| `second-bedroom.jpg` | Gallery — Second Bedroom |
| `second-bathroom.jpg` | Gallery — Second Bathroom |
| `backyard.jpg` | Gallery — Backyard |

## Swapping a photo

Each gallery tile in `index.html` is a `<button class="gallery-item">` with an `<img>`
and a `data-src` attribute (used by the lightbox) both pointing at the same file:

```html
<button class="gallery-item" data-caption="Kitchen" data-src="images/kitchen.jpg">
  <img src="images/kitchen.jpg" alt="Remodeled kitchen" loading="lazy">
  <span class="gallery-caption">Kitchen</span>
</button>
```

To swap a photo, just replace the file at that path (keep the same filename) or update
both the `src` and `data-src` to point at a new filename. The hero background is set on
the `<img class="hero-photo">` in the `.hero-media` block near the top of `index.html`.

## Note

Justin's original photo folder had several extra good shots not used here (an alternate
front exterior angle, extra kitchen/living-room angles, a second backyard angle, a close-up
of the new AC unit and electrical panel). Ask if you want any of those swapped in instead,
or added as additional gallery tiles.
