# DESIGNART V1

A local-first fashion customization and face-composite try-on demonstration built with Next.js.

## Features
- Curated garment catalog: dresses, ethnicwear, menswear and contemporary styles.
- Live color, fabric, neckline, sleeve, length, fit, pattern and embroidery controls.
- Personal photo upload with adjustable face crop.
- Transparent face cutout and canvas-based compositing onto a stylized fashion template.
- Save designs and previews in browser-local storage; reopen and delete saved designs.
- Download PNG try-on concept.
- Responsive desktop and mobile UI.

## Run locally
```bash
npm install
npm run dev
```
Open http://localhost:3000.

## Storage and privacy
V1 stores project records and image data in this browser's localStorage. Nothing is uploaded to an AI provider. Data is browser- and device-specific; clearing site data removes saved projects. Download important previews.

## Try-on limitation
This is a face-compositing demonstration using a stylized model/template, not automatic face recognition, real body-based fitting, physical cloth simulation, or a fit guarantee. Face cropping is manually adjustable.

## Deployment
The frontend can be deployed to Vercel. Browser-local persistence remains on each visitor's device. For cross-device accounts and centralized image storage, add a hosted database and object storage in a later release.

Repository: https://github.com/SanFlash/designArt
