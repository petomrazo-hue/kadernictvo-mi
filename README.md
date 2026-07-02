# Madame hair & beauty — web (kadernictvomichalovce.sk)

Statická prezentačná stránka pre kaderníctvo **Madame hair & beauty**
(Námestie Slobody 15, Michalovce). Čisté HTML/CSS/JS — **bez build kroku**,
bez frameworku, bez závislostí.

Autor návrhu: **Peter Mráz** — https://mrazosoft.sk

---

## Štruktúra

```
index.html        Domov (hero, služby, „Ako to prebieha“, galéria teaser, recenzie, kontakt)
sluzby.html       Služby (kompletný cenník/úkony)
galeria.html      Galéria (24 fotiek, filter Vlasy/Mihalnice/Líčenie, lightbox)
salon.html        O salóne
kontakt.html      Kontakt + FAQ + mapa
css/style.css     Celý dizajn systém (CSS custom properties, responzívne)
js/main.js        Interakcie (reveal, lightbox, galéria filter, mapa facade, menu)
images/           WebP fotky + galéria
images/CREDITS.md Pôvod a licencie všetkých fotiek  ← DÔLEŽITÉ, prečítať
fonts/            Self-hosted woff2 (Great Vibes, Cormorant Garamond, Jost)
robots.txt, sitemap.xml, favicon.svg, apple-touch-icon.png
.nojekyll         (pre GitHub Pages)
.github/workflows/pages.yml   Príklad deployu cez GitHub Actions (voliteľné)
sablona/madame-sablona.html   Bonus: celá stránka v jednom súbore (inline CSS/JS, base64 fotky)
```

## Spustenie lokálne

Stačí otvoriť `index.html` v prehliadači, alebo spustiť ľubovoľný statický server:

```bash
python3 -m http.server 8000     # potom http://localhost:8000
```

## Nasadenie

Ľubovoľný statický hosting (Apache/Nginx/GitHub Pages/Netlify…). Nič sa nebuilduje —
nahrajú sa súbory tak ako sú. `.nojekyll` je pre GitHub Pages; `pages.yml` je hotový
Actions workflow, ak by ste chceli deploy cez GitHub.

## Dôležité poznámky

- **Fonty sú self-hosted** (woff2 v `fonts/`) — žiadny Google Fonts CDN. Dôvod: GDPR
  (CDN prenáša IP návštevníka do USA). Preto stránka nepotrebuje cookie lištu kvôli fontom.
- **Fotky galérie** pochádzajú z FB profilu salónu — viď `images/CREDITS.md`. Časť fotiek
  obsahuje identifikovateľné tváre klientok → pred ostrým spustením odporúčam získať súhlas
  na použitie na webe, alebo ich vymeniť. Fotky služieb sú z Pexels (Pexels License).
- **SEO**: každá stránka má vlastný `title`/`description`/`canonical`, Open Graph, JSON-LD
  `HairSalon` (adresa, telefón, otváracie hodiny, hodnotenie), `robots.txt` a `sitemap.xml`
  (nastavené na doménu `kadernictvomichalovce.sk` — pri inej doméne upraviť).
- **Merania**: v `<head>` je Google Tag Manager (`GTM-NZXLTB38`) s **Consent Mode v2,
  default denied**. Kontajner/ID si nahraďte vlastným.
- **Doplniť pred spustením**: IČO a kontaktný e-mail prevádzkovateľa v pätičke.
