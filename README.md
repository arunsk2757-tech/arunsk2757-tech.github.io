# Arun S Kumar: portfolio

A one-page story portfolio: a white architectural pavilion builds itself as you scroll, while the page explains how I work with AI. After that come client work, the AI Lab and the Oasis film, and at the end the pavilion's lights come on beside the contact details.

Everything here was built with AI. The page was designed and coded with Claude, and the pavilion was modelled and rendered in Blender through Claude.

## Put it online with GitHub Pages (free)

1. Sign in at github.com and click **New repository**. Name it `portfolio`, set it to **Public**, and click **Create repository**.
2. On the new repository page, click **uploading an existing file**.
3. Open the `site` folder on your computer, select **everything inside it**, and drag it into the browser. Wait for the upload to finish, then click **Commit changes**.
4. Go to **Settings → Pages**. Under **Branch**, choose `main` and `/ (root)`, then click **Save**.
5. After a minute or two, the site is live at `https://<your-github-name>.github.io/portfolio/`.

For a company-specific greeting, add `?for=` to the link. For example, `https://<your-github-name>.github.io/portfolio/?for=4spots` opens with "Hi 4spots team".

## Files

| File | What it is |
|---|---|
| `index.html` | The whole page: layout, styles and script |
| `media/frames/` | 150 Blender renders of the pavilion, played by scrolling |
| `media/work/` | Client project screenshots |
| `media/nexus/` | Real NexusAI and ADAS screens |
| `media/oasis.mp4` | The Oasis of Intelligence film (VEED watermark cropped out) |
| `media/Arun_S_Kumar_CV.pdf` | CV offered for download |

## Adding the ADAS driving video

Save it as `media/adas.mp4` (a short clip of 10–20 seconds works best) and run `python3 build.py` again. The interface screenshot is then replaced by the video.

## Rebuilding

`python3 build.py` creates:
- `dist/site/`: the folder to upload to GitHub Pages
- `dist/Arun_S_Kumar_Portfolio.html`: a single file to attach to emails
- `dist/Arun_S_Kumar_Portfolio_4spots.html`: the same file, with the 4spots greeting
