# GTA 6 Giveaway · $GIVEAWAY

Landningssida för $GIVEAWAY. Varje 0,3 SOL man håller = 1 ticket, inget tak. Kopia #1 betalas av dev och dras på releasedagen (19 nov). Efter det köper fees en ny kopia för varje $79.99, och sedan blir det en ny dragning.

Allt ligger i en fil: `index.html`. Bilden som visas när länken delas på X heter `og.jpg`.

## Fyll i CONFIG (överst i scriptet i index.html)

| Fält | Vad |
|---|---|
| `name`, `ticker` | Namn och ticker (ticker utan $). Byts automatiskt överallt på sidan. |
| `ca` | Mint-adressen efter launch. Tom = "Posted here and on X at launch". |
| `x` | Länk till X-kontot, t.ex. `https://x.com/handle` |
| `dexscreener` | Valfritt |
| `site` | Domänen, syns på ticket-korten |
| `solPerTicket` | 0.3 |
| `copyPrice` | 79.99 (USD, Standard Edition) |
| `firstDraw` | Tid för dragning #1. Nu `2026-11-19T20:00:00+01:00` (20:00 svensk tid). Nedräkningen räknar hit. |
| `totalTickets` | Antal tickets vid senaste snapshot. Fyll i för att visa odds i ticket-räknaren. 0 = dolt. |
| `vault.usd` | Hur mycket som ligger i vaulten just nu (USD). Fyller mätaren. |
| `vault.copiesBought` | Hur många kopior fees har köpt |
| `vault.updated` | T.ex. `"20 Nov, 14:00"` |
| `draws` | Resultattavlan. Status: `scheduled`, `waiting`, `live` eller `won`. Sätt `winner` till vinnarens plånboksadress när den är dragen. |

## Deploy

GitHub → Vercel som de andra sajterna: nytt repo med `index.html`, `og.jpg` och den här README:n, importera i Vercel, välj Framework "Other", inget build-steg.

## Kolla efter deploy

- Intron: trumman tonar in och kulorna droppar ner en och en, sedan blåser de runt.
- Scrolla genom "How a draw works": kulorna åker in → snapshot-linjen sveper → trumman blandar → guldkulan åker ut genom toppen.
- Typsnitten (Anybody, Figtree, Spline Sans Mono) laddas från Google Fonts.
- "Make my ticket card" ger en bild att posta på X.
- X-förhandsvisningen visar og.jpg.
