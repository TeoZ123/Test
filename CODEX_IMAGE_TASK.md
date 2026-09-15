# Task: Generate 14 images for the GleamJet demo landing page

## 1. Project context

This directory is a static, self-hosted demo website used internally at Shoplazza to demonstrate a "URL import" feature (it copies an external landing page into a merchant store). The site must contain **zero third-party assets** and **no real brands, media outlets or people**, so every image has to be freshly generated.

- `index.html` — an English "advertorial" article in the style of a home & living news site. Fictional publication: *The Home Living Journal*. Fictional brand: *Northwick Home*. Fictional product: **GleamJet Cordless Spin Scrubber** (a cordless electric cleaning brush for bathrooms and kitchens). Fictional author: *Margaret Lindqvist*, Home & Living Editor.
- `order.html` — a simple single-column checkout page for the same product.
- `img/` — 14 JPG files. **All 14 currently exist as flat gradient placeholders.** Your job is to replace each one with a generated photo, **keeping the exact same file name and pixel size**. No HTML changes are needed.
- `dist/` — build output. Ignore it; it is regenerated at publish time.

Page palette (for harmony, not for text overlays): accent teal `#0f766e`, sale orange `#c2410c`, near-black `#1a1a1a`, soft grey `#f6f7f8`.

## 2. Hard rules for every image

1. Photorealistic. Natural light. Clean, modern, middle-class home interiors. Editorial / e-commerce photography quality.
2. **No text, no captions, no watermarks, no logos, no brand marks** anywhere in the image (including on the product, packaging, clothing, or background).
3. **No real or recognisable people.** All faces must be generic, fictional adults. Avoid any resemblance to celebrities or public figures.
4. Output as JPG, sRGB, quality 85 to 90, exactly the pixel dimensions listed below (crop or outpaint as needed, do not letterbox).
5. The product must look **identical across all product images**. Use the product spec in section 3 verbatim in every product prompt.

## 3. Product spec (paste into every prompt that shows the product)

> A cordless handheld electric spin scrubber: matte white cylindrical body about 30 cm long, a soft teal rubber grip band around the middle, a single round teal power button, a slim teal accent ring where the brush head attaches. A telescoping brushed-aluminium extension pole that clicks onto the bottom of the handle. Four interchangeable snap-on heads in white plastic with teal bristles or pads: (1) a flat round scrubbing pad about 10 cm across, (2) a pointed corner brush, (3) a dome-shaped brush, (4) a soft grey microfibre polishing pad. Minimal Scandinavian-style design, no printed text or logo on any part.

## 4. Image list

Priority A = visible above the fold or repeated across pages; generate these first.

| # | File name | Size (px) | Priority | Where it appears | Prompt |
|-|-|-|-|-|-|
| 1 | `img/hero.jpg` | 1200 × 700 | A | Full-width hero image directly under the headline and byline | Editorial photo. A woman's hand holding [PRODUCT SPEC] with the pointed corner brush attached, scrubbing along the grout line of a white subway-tile bathroom wall. Fine water droplets and a little foam on the tile. Bright soft daylight from a window on the left. Shallow depth of field, tile in sharp focus, background softly blurred. Horizontal composition, product slightly right of centre. |
| 2 | `img/product.jpg` | 1200 × 800 | A | Section "What It Actually Is" | Product photography, top-down 30-degree angle. [PRODUCT SPEC] laid out neatly on a light grey-veined marble countertop: the handle in the centre, the extension pole beside it, and the four brush heads in a row in front. A white USB-C charging cable coiled loosely at one side. Bright, even natural light, soft shadows, minimal styling, lots of clean negative space. |
| 3 | `img/before-after.jpg` | 1200 × 700 | A | Section "The 30-Day Test", split before/after | Photorealistic before-and-after comparison of the same tiled shower floor with small white square tiles, shot from directly above. Left half: grout lines grey and stained, soap scum haze, slightly dull. Right half: identical tiles with bright white clean grout, glossy and spotless. A thin vertical soft divider exactly in the middle. No text, no labels, no arrows. Natural bathroom lighting. |
| 4 | `img/product-thumb.jpg` | 600 × 600 | A | Sticky sidebar CTA card (displayed ~260 px wide) and the checkout page thumbnail (96 px) | Clean e-commerce product shot. [PRODUCT SPEC] handle standing upright with the flat round scrubbing pad attached, the other three heads arranged small at its base. Plain very light grey seamless background, centred, soft natural shadow underneath. Square composition, product fills about 75% of the frame. |
| 5 | `img/author.jpg` | 300 × 300 | A | Author avatar in the byline (40 px circle) | Professional editorial headshot of a fictional woman in her late forties, shoulder-length light brown hair, warm genuine smile, wearing a plain dark green blouse, neutral warm grey background, soft window light. Head and shoulders, centred, square crop. |
| 6 | `img/avatar-1.jpg` | 300 × 300 | B | Customer review card: "Denise Okafor-Hale, Austin, TX" | Casual portrait of a fictional Black woman in her fifties, short natural hair, friendly relaxed expression, bright living room softly blurred behind her. Head and shoulders, square crop. |
| 7 | `img/avatar-2.jpg` | 300 × 300 | B | Customer review card: "Tom Brannigan, Leeds, UK" | Casual portrait of a fictional white man in his forties with a short beard and a grey crew-neck sweater, outdoors on an overcast day, brick houses blurred behind him. Head and shoulders, square crop. |
| 8 | `img/avatar-3.jpg` | 300 × 300 | B | Customer review card: "Priya Venkataraman, Toronto, ON" | Casual portrait of a fictional South Asian woman in her thirties, long dark hair, smiling, modern apartment kitchen blurred behind her. Head and shoulders, square crop. |
| 9 | `img/avatar-4.jpg` | 300 × 300 | B | Reader comment: "Karen Whitlock" | Casual selfie-style portrait of a fictional white woman in her sixties with short grey hair and glasses, warm smile, kitchen background. Head and shoulders, square crop. |
| 10 | `img/avatar-5.jpg` | 300 × 300 | B | Reader comment: "Marcus Delaney" | Casual portrait of a fictional Black man in his thirties, clean-shaven, plain navy t-shirt, neutral indoor background. Head and shoulders, square crop. |
| 11 | `img/avatar-6.jpg` | 300 × 300 | B | Reader comment by the author, "Margaret Lindqvist" | **The same fictional woman as `author.jpg`** (late forties, shoulder-length light brown hair), but a more casual setting: home office, slight three-quarter angle, relaxed smile. Head and shoulders, square crop. |
| 12 | `img/avatar-7.jpg` | 300 × 300 | B | Reader comment: "Sophie Marchetti" | Casual portrait of a fictional Italian woman in her forties with dark wavy hair, warm evening light, neutral background. Head and shoulders, square crop. |
| 13 | `img/avatar-8.jpg` | 300 × 300 | B | Reader comment: "Dev Raghunathan" | Casual portrait of a fictional Indian man in his late twenties wearing thin-rimmed glasses, light blue shirt, neutral background. Head and shoulders, square crop. |
| 14 | `img/avatar-9.jpg` | 300 × 300 | B | Reader comment: "Linda Feuerstein" | Casual portrait of a fictional white woman in her fifties with blonde hair, garden with greenery blurred behind her. Head and shoulders, square crop. |

Replace `[PRODUCT SPEC]` with the full paragraph from section 3.

Negative prompt suggestion for all images: `text, letters, words, logo, watermark, caption, signature, brand name, deformed hands, extra fingers, cartoon, illustration, 3d render look, oversaturated, blurry`.

## 5. Delivery and verification

1. Write each file to `img/<name>.jpg`, overwriting the placeholder. Do not rename, do not add new files, do not change the HTML.
2. Verify sizes, for example:
   ```bash
   python3 -c "from PIL import Image;import glob;[print(f, Image.open(f).size) for f in sorted(glob.glob('img/*.jpg'))]"
   ```
   Expected: hero 1200×700, product 1200×800, before-after 1200×700, product-thumb 600×600, all others 300×300.
3. Optional visual check: `python3 -m http.server 8765` in this directory, then open `http://localhost:8765/` and `http://localhost:8765/order.html`.
4. Do **not** publish. Publishing to the hosted URL is done separately with `lark-cli apps +html-publish --app-id app_17e3gpfsqd0 --path ./dist` after `dist/` is rebuilt; leave that step to the project owner.

## 6. Consistency checklist before you finish

- [ ] The scrubber looks the same (white body, teal grip, teal button, teal accent ring, aluminium pole, four heads) in `hero.jpg`, `product.jpg`, `product-thumb.jpg`.
- [ ] `author.jpg` and `avatar-6.jpg` are clearly the same fictional woman.
- [ ] No text, logo or watermark appears in any image.
- [ ] No image contains a real, recognisable person or a real brand.
- [ ] All 14 files exist at the exact required pixel sizes and open without error.
