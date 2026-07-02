# Immo Store — voorstel (Pixelshift)

Vertrouwelijke voorstelpagina voor **Immo Store** (Sam Van Hecke), gemaakt door **Pixelshift**.
Statische site — geen build-stap nodig.

## Structuur
```
index.html            → de voorstelpagina (root van de site)
vendor/               → lokaal gehoste assets, geen externe CDN's nodig
  three.module.min.js   three.js (MIT-licentie)
  hanken-grotesk-*.woff2 Hanken Grotesk font (SIL OFL-licentie)
  *.LICENSE(.md)        de bijhorende licenties
```

## Hosten op Vercel
Deze repo is een pure statische site. Bij het importeren in Vercel:
- **Framework Preset:** Other
- **Build Command:** *(leeg laten)*
- **Output Directory:** *(leeg laten — de root wordt geserveerd)*

Vercel serveert `index.html` automatisch op de root-URL. Geen `vercel.json` nodig.

## Lokaal bekijken
```bash
python3 -m http.server 8000
# → http://localhost:8000/
```

De pagina draagt `noindex,nofollow`: ze verschijnt niet in Google en is enkel via de directe link bedoeld.
