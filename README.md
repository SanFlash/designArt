# DESIGNART — Personal Fashion Studio

A responsive fashion studio with photographic garment references, design controls, portrait uploads and a browser-local project library.

## Current features
- Photographic outfit references for evening gowns, column dresses, sarees, lehengas, tailored suits, linen outfits and contemporary dresses.
- Search and category filters.
- Design brief controls for color, fabric, neckline, sleeves, length, fit, pattern and embroidery.
- Portrait upload and adjustable manual crop.
- Side-by-side personal style board using the user's portrait and the selected outfit photograph.
- Save, reopen and delete projects using IndexedDB.
- Responsive desktop and mobile layout.

## Run locally
```bash
npm install
npm run dev
```
Open http://localhost:3000.

## Important: current realism boundary
This release removes the cartoon garment drawings and uses photographic fashion references instead. The color/fabric/neckline controls currently save a design brief; they do not physically recolor or reconstruct the clothing in the reference photograph. The generated board places the user's portrait beside the selected outfit reference. It does **not** put the outfit onto the user's body.

A real virtual try-on requires a model/service that performs person segmentation, pose estimation, garment parsing, clothing warping, occlusion handling and photorealistic synthesis. No such inference model or credentials are configured in this repository. Do not present the current style board as an accurate fitting or sizing result.

## Image sources and rights
The catalog uses externally hosted example fashion photographs from the following publishers/retailers for demonstration: ELLE/ Hearst, PeterPhoto, Etsy sellers, Studio East6, Legere, and Olivia Sophie. These images remain the property of their respective rights holders and may be subject to copyright, hotlink restrictions or commercial licensing. Replace them with owned, licensed, or user-uploaded product photography before commercial launch. Image delivery also depends on the source hosts remaining available.

## Privacy and storage
Portraits and saved projects are stored in IndexedDB in the visitor's browser. The app does not upload user photos to an AI provider in this release. Browser data is device-specific and can be removed by clearing site data.

## Deployment
Deploy the repository root as a Next.js project on Vercel.

Repository: https://github.com/SanFlash/designArt
