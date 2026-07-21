# Camera LiDAR Calibration in the Eye of LiDAR — Project Page

Static project page for the paper *"Camera LiDAR Calibration in the Eye of LiDAR"*
(anonymous submission).

The page shows the title, abstract, and the three algorithm components with figures/videos:
(1) recovering the LiDAR optical center ("eye"), (2) the plane-attract / silhouette-repel
objective in the virtual LiDAR-eye camera, and (3) the final calibrated overlays and range render.

## Local preview

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```

## Structure

- `index.html` — page markup (hero, teaser, abstract, method steps, self-consistency).
- `styles.css` — styling.
- `assets/` — web-optimized media:
  - `final_overlay.png` — calibrated overlay + range panorama teaser.
  - `eye_recovery.mp4` — LiDAR optical-center recovery animation.
  - `process_objective.mp4` — board-silhouette objective converging in the LiDAR-eye view.
  - `final_overlays.mp4` — time-synced overlays on the RGB video.

## Deploy to GitHub Pages

1. Create a new public repo (e.g. `camera-lidar-calib-page`).
2. Push this folder's contents to the repo root.
3. Settings -> Pages -> source = `main` branch, root (`/`).
4. Served at `https://<user>.github.io/camera-lidar-calib-page/`.

`.nojekyll` is included so GitHub Pages serves all files as-is.
