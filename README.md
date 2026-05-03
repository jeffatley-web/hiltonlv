# Hilton Grand Vacations Club Paradise — Case Study Deployment

Files for shipping the Hilton HGVC Paradise case study via the GitHub Pages + Webflow embed split pattern, mirroring the Turtle Bay setup.

## Files

| File | Purpose | Size |
|---|---|---|
| `index.html` | Standalone HTML, served by GitHub Pages at the public preview URL | 38,888 chars |
| `hilton-hgvc-paradise.css` | Stylesheet — referenced by both the standalone and the Webflow embed | 34,085 chars |
| `webflow-embed.html` | Drop-in code for the Webflow Embed block on aquarevwater.us | 39,077 chars |

## Repo

`https://github.com/jeffatley-web/hiltonlv` — dedicated repo for this case study.

## Public URLs

- Standalone preview: `https://jeffatley-web.github.io/hiltonlv/`
- CSS direct: `https://jeffatley-web.github.io/hiltonlv/hilton-hgvc-paradise.css`

## Deployment

1. Files committed to repo root
2. GitHub Pages enabled: Settings → Pages → Deploy from branch → main → / (root)
3. Webflow page (e.g. `aquarevwater.us/hilton-paradise`) → drop a single Embed block, paste contents of `webflow-embed.html`, publish

## Update workflow

When the master case-study HTML at `Aquarev Water /Case Study/Hilton Desert Paradise/Hilton HGVC Paradise - Visual Report.html` is edited, regenerate these 3 files and `git push`. Webflow auto-picks up CSS changes; body changes require re-pasting the embed.
