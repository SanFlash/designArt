# DESIGNART — Personal Fashion Studio

A responsive fashion customization studio built with Next.js. The current release includes garment-specific editorial illustrations, fabric shading and drape details, customization controls, and a browser-local design library.

## Features
- Garment catalog for gowns, dresses, sarees, lehengas, suits, shirts and contemporary looks.
- Garment-specific silhouette paths with fabric highlights, folds, seam details, draping and optional embroidery.
- Color, fabric, neckline, sleeve, length, fit, pattern and embroidery controls.
- Portrait upload and manual face crop / placement controls.
- Editorial concept renderer with garment drape, shading and seam details.
- Save, reopen, delete and download designs.
- IndexedDB browser-local persistence.
- Responsive desktop and mobile interface.

## Run locally
```bash
npm install
npm run dev
```
Open http://localhost:3000.

## Important try-on limitation
The fitting-room output is an editorial concept composite, not a photorealistic virtual try-on. The current app does not perform human parsing, pose estimation, body segmentation, cloth warping, occlusion handling, or physics-based fabric simulation. The face crop is manually adjusted and does not perform AI face segmentation. Do not use the preview to judge garment fit or sizing.

A true photorealistic try-on requires an integrated virtual try-on inference service (or a self-hosted model) with consent-based image processing, person/garment segmentation, pose estimation, garment warping and realistic compositing. No AI provider credentials are included in this repository; configure them server-side before enabling such a service. Never expose provider keys in browser code.

## Storage and privacy
Designs and image previews are stored in IndexedDB in the current browser. They are device- and browser-specific; clearing site data removes them. The app does not upload photographs to a remote AI provider in this release.

## Deployment
Deploy the repository root as a Next.js project on Vercel. Browser-local storage remains on each visitor's device.

Repository: https://github.com/SanFlash/designArt
