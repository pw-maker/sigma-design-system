# SIGMA design system

The visual language of SIGMA Corporation of America's websites (www.sigmaphoto.com, the shop, and blog.sigmaphoto.com, the
SIGMA Blog), taken from the live pages for designing SIGMA pages in Agency.

The Sigma Sans and Sigma Serif web fonts in `fonts/` are SIGMA's own, © SIGMA, all rights reserved, and are here for this
prototype only. Keep this repository private.

## Contents

- `fonts/`: the eight web fonts the sites load, as woff2
- `colors_and_type.css`: `@font-face` rules for them (relative to this folder), colour, type and spacing tokens, and semantic
  styles
- `assets/`: the SIGMA wordmark (`sigma-wordmark.svg`, 103×24, black), the Σ roundel used in footers (`sigma-roundel.svg`,
  80×80, black ring with a serif capital sigma), and the north-east arrow that follows external links (`icon-link.svg`, 6×6)
- `reference/`: four real pages from the sites, frozen as static HTML with their images at their live URLs. Treat them as the
  ground truth for components and layout:
  - `trevor-key-hero.html`: the homepage banner, a full-bleed photo with centred white display type (2322×1227 viewport)
  - `sigma-blog-freedom-to-move.html`: a blog article on a phone (440 wide), with photos, EXIF captions, a CTA banner, an
    "About" block, product and related-post cards, and the blog footer
  - `sigma-blog-trevor-key.html`: a photo-book feature on the blog (440 wide)
  - `sigma-shop-trevor-key.html`: the shop's product page (1371 wide): promo bar, header, gallery, buy column, footer

## Visual foundations

- **Type does the work.** Three families: **Sigma Serif head** (the Headline cut, one weight) for H1s and display titles, always
  uppercase; **Sigma Serif** (the Text cut, regular, bold and italic) for all body copy, prices, buttons and secondary
  headings; **Sigma Sans** at 13px, uppercase and slightly tracked (0.2px on the blog, 0.08–0.26px in the shop) for nav,
  categories, captions, labels and footers. Body is 16/20. Blog H1 36/39.6; homepage hero 88/96; CTA headings 36/45 in the Text cut.
- **Colour is almost absent.** Ink `#333333` on off-white paper `#FEFEFD`; muted ink at 70% for secondary labels; pure white
  for article columns and the shop footer. The only accents: a 2px pink `#FF859B` rule under inline links in blog copy, and
  pure red `#FF0101` for a returns warning. Logos are pure black.
- **Photography carries the colour.** Images are full width of their column, never rounded, never bordered, never shadowed,
  shown at their native aspect ratio unless they're a banner or card thumbnail (then `object-fit: cover`). Banners put white
  text straight on the photo, sometimes over a 50% grey dim (`#404040` or `#495664`); no gradients, no text shadow.
- **Square and flat.** No radius anywhere except pill CTAs (radius 9999px, `#F2F2F2` fill, `#202020` bold serif label). The
  shop's primary button is a flat `#333333` bar, 40px tall, white uppercase Sans label. No shadows, no blur, no borders except
  hairline `#707070` rules on form controls.
- **Generous, regular whitespace.** 16px page gutters; 80px between blog blocks; 96px between sections; 160px above footers;
  16/24/32px inside components.
- **Static headers.** Text-only nav (MENU / SEARCH on the blog; PRODUCTS, MADE IN AIZU, INSPIRATION, SUPPORT, NEWS on the shop)
  with the wordmark centred, no icons, no divider, not sticky.
- **Footers** start with the centred Σ roundel, then uppercase Sans link groups (INFORMATION, CUSTOMER SERVICE, POLICIES,
  FOLLOW SIGMA PHOTO, FOLLOW CINE), muted headings, and "© 2025 All Rights Reserved".

## Iconography

Almost none. Nav and actions are words, not icons. The only icons are the north-east arrow after external links
(`assets/icon-link.svg`), the radio ring and +/− of the shop's quantity stepper (simple 1px `#333` strokes), and the two
logos. No emoji, no icon font in designs.
