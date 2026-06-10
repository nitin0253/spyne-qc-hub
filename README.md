# Spyne QC Dashboard Hub

Central launcher for all QC pendency dashboards. Each product dashboard runs independently in its own Vercel deployment — this hub just provides a single URL with tab switching.

## Products
| Tab | URL | Status |
|-----|-----|--------|
| 🖼️ Images | https://vin-tracker-delivery.vercel.app/ | Live |
| 🎬 Videos | https://video-tracker-delivery.vercel.app/ | Live |
| 🔄 360° | — | In Progress |

## Setup
1. Create a new GitHub repo (e.g. `spyne-qc-hub`)
2. Add `index.html` and `vercel.json` from this folder
3. Connect to Vercel → deploys automatically
4. When 360° is ready, update the `data-src` on the 360 iframe in `index.html`

## Adding 360°
When the 360 dashboard is deployed, update `index.html`:
1. Change the `<div class="frame" id="frame-360">` to an `<iframe>`
2. Set `src` to the 360 Vercel URL
3. Remove the `tab-badge` SOON label from the 360 tab button
