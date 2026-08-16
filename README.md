# Mr.SD Men's Salon & Spa — Website

A premium, single-page React + Vite website for Mr.SD Men's Salon & Spa (Kodungaiyur, Chennai).

## Tech stack

- React 18
- Vite 5
- Tailwind CSS 3
- lucide-react (icons)

## Project structure

```
.
├── index.html
├── package.json
├── postcss.config.js
├── tailwind.config.js
├── vite.config.js
├── public/
│   └── favicon.svg
└── src/
    ├── App.jsx        # entire site (all sections + logic)
    ├── main.jsx        # React entry point
    └── index.css       # Tailwind directives
```

## Run locally

```bash
npm install
npm run dev
```

Then open the URL Vite prints (usually http://localhost:5173).

## Build for production

```bash
npm run build
```

Output goes to the `dist/` folder. Preview it locally with:

```bash
npm run preview
```

## Deploy to Vercel

1. Push this project to a GitHub repository.
2. Go to [vercel.com](https://vercel.com), click "New Project", and import the repo.
3. Vercel auto-detects Vite. Confirm these settings (should be filled in automatically):
   - **Framework Preset:** Vite
   - **Build Command:** `npm run build`
   - **Output Directory:** `dist`
4. Click **Deploy**.

No environment variables are required — the booking form is a frontend-only demo (it does not submit anywhere), and WhatsApp/Call/Directions links use static values already in the code.

## Notes

- All images (hero, gallery, about) are embedded directly in `src/App.jsx` as base64 data — no external image hosting is required.
- Two of the images in the gallery/about sections came from stock/downloaded sources rather than the salon's own photos — see project chat history for details if you plan to replace them with real photography.
