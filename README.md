# romanpavlorek.eu

Osobní web Romana Pavlorka — **hry · hudba · příběhy**. Jeden člověk z ČR: staví indie hry a aplikace (pod značkou 3R Studio), nahrává hudbu, píše.

Statický web (vanilla HTML/CSS/JS, bez frameworku). Hostován na Hetzner VPS přes Caddy, auto-deploy z této `main` větve.

## Stránky

| Soubor | Obsah |
|---|---|
| `index.html` | Rozcestník — hudba, studio, příběhy, zápisky, kontakt |
| `roman-music.html` | Roman jako autor — album **Spektrum barev**, vlastní texty a hlas |
| `pavler.html` | **Pavler** — AI-produkovaná virální hudba (hyperpop, phonk), TikTok/Spotify funnel |
| `blog-personal.html` | Zápisky / blog — rozcestník článků |
| `blog-post-personal.html` | Šablona jednotlivého článku |

## Design

- Světlé téma, fialovo-žluto-teal akcenty, fonty DM Sans / Instrument Serif
- Animované gradientní pozadí, fullscreen sekce, plynulý scroll
- Dvojjazyčnost CZ/EN (přepínač v hlavičce)

## Dvě identity (záměrné dělení)

- **Roman Pavlorek** (tento web) — osobní brand: autorská hudba (Spektrum barev), kniha **Paleta**, fyzikální/filozofické úvahy, blog, Pavler
- **3R Studio** ([3rstudio.eu](https://3rstudio.eu)) — produktová značka: hry, aplikace, 3Cue

## Stav (k 2026-06-11)

**Hotovo:** deploy, HTTPS, auto-deploy, Cloudflare, struktura všech stránek, dvojjazyčnost.

**Zbývá / k ověření:**
- [ ] **Google Analytics má placeholder `G-XXXXXXXXXX`** — měření zatím neběží, doplnit reálné measurement ID
- [ ] První blog zápisky (sekce „Zápisky" je prázdná)
- [ ] **Sjednotit termíny s realitou**: stránka slibuje „Spektrum barev — album srpen 2026", ale produkce zatím nemá hotové mastery a čeká na IČO; zvážit „2026" bez měsíce
- [ ] Paleta — odkazy „Číst ukázku / Koupit" jsou zatím placeholdery („brzy")
- [ ] Skrýt/odložit hudební sekce do doby, než bude obsah živý (dle původního plánu)

## Deploy

Push do `main` → automatický deploy na VPS (Caddy servíruje statické soubory). Žádný build krok.
