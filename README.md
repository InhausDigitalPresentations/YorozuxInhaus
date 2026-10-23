# YOROZU — Time is Rare

A cinematic web pitch built by INHAUS for Yorozu, Abu Dhabi. It's a static site with no build step, so it's ready for GitHub Pages.

## Publish on GitHub Pages
1. Create a new repository and upload everything in this folder: `index.html`, `.nojekyll`, `README.md` and the whole `assets/` folder.
2. Go to **Settings → Pages → Build and deployment**, choose **Deploy from a branch**, then **main / root**, and save.
3. After a minute or two the deck is live at `https://<user>.github.io/<repo>/`.

Notes:
- A GitHub Pages site is public to anyone who has the link. The page tells search engines not to index it (`noindex`), but avoid giving the repo an obvious name.
- The total size is about 43 MB (eight 1080p clips and nine ambient loops) and every file is well under GitHub's limits.

## Presenting
- On the first screen, click **Begin with sound**. Browsers only allow audio after a click.
- Move forward with → / Space / click / scroll, and back with ←. Press **F** for full screen and **M** for sound on/off.
- **Index:** click **Index** (top right) or press **I** to open the chapter menu, then click any slide to jump to it. Clicking the chapter name at the bottom left opens it at the current chapter. **Esc** closes it.
- Some slides reveal lines one at a time. Keep pressing → and the slide changes once all its lines are shown.
- Use `#12` at the end of the URL to jump to slide 12. Slides 34 and 35 carry the retainer (AED 26,000 per month) and the performance-marketing scope.
- The clock in the top right counts the time spent. The closing slide uses it: "You spent N minutes with Yorozu today."

## Editing
- **Links on the closing slide:** in `index.html`, find `const LINKS` near the bottom and fill in the Instagram, LinkedIn and website URLs. Links left empty are hidden.
- **Copy:** each slide is a `<section class="slide">` in `index.html`, in presentation order.
- **Sound:** each slide has `data-bed` (`sea`, `market`, `brewery` or `none`) and `data-level` (0–1) for its ambient level. The beds crossfade between slides.
- **Images and video:** these are in `assets/img` and `assets/video`, taken from Yorozu's own Japan photo books, marketing plan and Draft 01 films. Single images and loops sit in the `tall` rectangle (9:16, or `p45` for 4:5); `rev` on the `.split` puts it on the left.

## Before presenting, check
- **Second lines and craft facts.** The TIME IS RARE second lines are generic on purpose ("years", "a season", "thousands of times"). Confirm each one with Chef Akira before you put a specific number on it.
- **Footage still to be filmed.** Dashed frames mark material that doesn't exist yet: the year-one/two/three tiles in the archive. Slide 17's Mina-at-dawn tile is an illustrative visualisation (Seedream 5.0 Pro + Kling 4.0, from Mina Zayed reference photos), captioned as such; replace it with real footage when it is shot. Slide 21 now carries Chef Akira's own portrait and a photograph of a fisherman at the nets.
- **Ambient sound.** It comes from the Draft 01 films. Listen to it, and if those films carry licensed music, cut that out or replace the beds.
- **Imagery.** Every image and clip is documentary material from the Japan journey, now served from the high-resolution masters and the 1080p films. The only generated material: the Mina-at-dawn visualisation (slide 17), the regraded water and darker counter on slide 10, and nine ambient loops (slides 01/36, 07, 08, 10, 11, 12 ×3, 17). See `../ENHANCEMENT/VISUAL_ENHANCEMENT_REPORT.md`.
