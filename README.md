# ZipChair AI (Static)

This repo is a static Vercel deploy containing:

- `/` — ZipChair shopping assistant (fully client-side; loads `public/data/products.json`)
- `/pitch/` — pitch deck (static HTML)
- `/intel/` — competitor intel dashboard (static; loads JSON from `/intel/data/*`)

## Local dev

```bash
cd projects/zipchair-deploy
npm run dev
```

Then open:

- http://localhost:3000/
- http://localhost:3000/pitch/
- http://localhost:3000/intel/

## Notes

- The assistant requires a web server for `fetch()` to load `products.json` (browsers typically block `file://` fetches).
