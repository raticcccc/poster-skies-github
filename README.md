# Poster Skies — WebAR

A mobile-first, image-target WebAR demo built with A-Frame and MindAR.

## Run locally
Camera access requires HTTPS or localhost.

```bash
python3 -m http.server 8000
```

Open http://localhost:8000, allow camera access, tap **ENTER EXPERIENCE**, and scan the matching poster.

## Deploy with GitHub Pages
1. Create a new GitHub repository.
2. Upload **all files and folders in this ZIP** to the repository root. `index.html` must be at the root.
3. Commit the files to the `main` branch.
4. Open **Settings → Pages**.
5. Under **Build and deployment**, choose **Deploy from a branch**.
6. Select branch `main` and folder `/ (root)`, then Save.
7. Wait for the Pages deployment and open the published HTTPS URL on your phone.

Keep the `assets/` and `lib/` folders alongside `index.html`; do not rename them.

## Included assets
- `assets/poster.mind` — MindAR image target
- `assets/poster.jpg` — poster reference
- `assets/models/` — supplied GLB character models
- `lib/` — A-Frame and MindAR browser libraries

The target file was generated for a particular poster image. Scan that same poster for tracking to work.

## Notes
This is a static client-side project; no backend or build step is required. Test on a real phone over HTTPS. Model scale and placement may need tuning for your particular model exports and device.
