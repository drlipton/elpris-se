# elpris-se

Svensk statisk informationssida om att Sverige har **fyra elområden** (SE1–SE4), inte ett enda elpris. Sidan förklarar skillnaden mellan områdena och visar spotpriser (öre/kWh, exklusive skatt, nät, påslag och moms).

Det här är inte elhandel, inte investeringsråd och inte godkänt av Energimarknadsinspektionen (Ei) eller PTS.

**Första live-knappen** går till [Elpriskollen](https://elpriskollen.se/). Affiliate-platser för Elskling och Vattenfall är avsiktligt tomma tills riktiga URL:er klistras in.

## GitHub Pages

Live-URL: https://drlipton.github.io/elpris-se/

Källan är grenen `main`, sökväg `/`. Filen `.nojekyll` gör att GitHub Pages inte kör Jekyll.

## Filer

| Fil | Roll |
| --- | --- |
| `index.html` | Startsida på svenska |
| `styles.css` | Layout och typografi |
| `404.html` | Svensk felsida |
| `robots.txt` | Tillåt indexering |
| `.nojekyll` | Stäng av Jekyll |

## Så klistrar du in affiliate-URL:er senare

Platshållarna ligger i `index.html`. De är **inte live**: `href="#"`, inaktiva och märkta *Ej live · framtida reklam*. Hitta kommentarerna och byt bara ut länken när du har en riktig URL.

1. `<!-- AFFILIATE_ELSKLING -->` — byt `href="#"` mot den riktiga Elskling-länken, ta bort `aria-disabled`, `tabindex="-1"` och klassen `btn-off`, lägg till `btn-live` (eller en egen reklamklass), och ta bort texten *Ej live · framtida reklam*.
2. `<!-- AFFILIATE_VATTENFALL -->` — samma steg för Vattenfall.

Klistra inte in påhittade länkar eller provisionsbelopp. Markera reklam tydligt. Elpriskollen ska fortsätta vara första live-knapp.

## Drift

Inget betalt hostingkonto. Bara GitHub Pages från den här publika repot.
