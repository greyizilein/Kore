# KORE Website — Video Setup

## Videos: Two Options

### Option A — Online (works immediately, no downloads needed)
The site uses **YouTube iframes** as background videos. Simply open the HTML files in a browser 
with an internet connection — videos play automatically.

---

### Option B — Self-hosted (works offline, faster, no YouTube branding)
Download these 4 free videos from Pexels and place them in the `videos/` folder:

| Filename to save as | Download from Pexels |
|---|---|
| `videos/hero.mp4` | https://www.pexels.com/video/a-female-model-walking-in-a-black-dress-9510022/ |
| `videos/reel1.mp4` | https://www.pexels.com/video/fashion-model-walking-in-the-runway-9512048/ |
| `videos/reel2.mp4` | https://www.pexels.com/video/a-woman-walking-down-the-runway-9512045/ |
| `videos/reel3.mp4` | https://www.pexels.com/video/models-walking-down-the-runway-while-carrying-woven-baskets-on-their-head-9511845/ |
| `videos/band.mp4`  | https://www.pexels.com/video/fashion-model-19862866/ |

**How to download from Pexels:**
1. Go to the URL above
2. Click the "Free Download" button
3. Choose HD quality
4. Rename the file as shown in the table and place it in the `videos/` folder

All videos are by **cottonbro studio** and **Bubble Media** — free for commercial use under the Pexels license.

---

### Replacing YouTube Video IDs
If you want to use different YouTube videos as backgrounds, open `index.html` or `system.html`
and find lines like:

```
src="https://www.youtube.com/embed/ysz5S6PUM-U?autoplay=1&mute=1&loop=1..."
```

Replace `ysz5S6PUM-U` (appears twice per iframe) with the YouTube video ID you want.
The video ID is the part after `v=` in a YouTube URL, e.g.:
`https://www.youtube.com/watch?v=`**`ysz5S6PUM-U`**

---

## Pages
- `index.html` — Homepage with hero video + video reel
- `collection.html` — Full product collection
- `product.html` — Single product view
- `system.html` — The System (brand philosophy)

## Design System
- Dark mode: `#08080A` background, `#F2EFE8` text, `#C4A46B` brass accent
- Light mode: `#F5F0E8` background, `#100E0A` text, `#9C7840` brass accent
- Fonts: Bodoni Moda (display) + Syne (body) — loaded from Google Fonts
- Theme preference saved in `localStorage` under key `kore-theme`
