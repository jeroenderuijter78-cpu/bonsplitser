# Bonsplitser

Een mobiele web-app om een restaurantrekening eerlijk over een groep te verdelen.

## Mogelijkheden

- **Live bijhouden** wie wat neemt tijdens het uitje.
- **Bon scannen** met de camera of een bestaande foto.
- Bonregels na de scan altijd **controleren en corrigeren**.
- Automatische rekencontrole: bonregels + fooi tegenover het betaalde totaal.
- Bon achteraf handmatig invoeren.
- Gedeelde hapjes gelijk verdelen, aantallen verdelen of vrije bedragen gebruiken.
- Fooi gelijk of naar rato verdelen.
- Eindafrekening per persoon delen, kopiëren, downloaden als tekst of afdrukken / opslaan als PDF.

## Bon scannen

De scanfunctie gebruikt Tesseract.js in de browser. De foto wordt op het apparaat verwerkt; er is geen eigen server of API-sleutel nodig. Bij de eerste scan is internet nodig om de OCR-bibliotheek en taalbestanden te laden.

OCR kan fouten maken. Daarom toont Bonsplitser na iedere scan eerst een controlescherm. De app vergelijkt bovendien de som van de gevonden regels en de fooi met het totaal op de bon.

## Gebruik via GitHub Pages

1. Maak op GitHub een nieuwe repository, bijvoorbeeld `bonsplitser`.
2. Upload **de volledige inhoud van deze map**, inclusief de map `assets`.
3. Ga in GitHub naar **Settings → Pages**.
4. Kies bij **Build and deployment** voor **Deploy from a branch**.
5. Kies branch **main** en map **/(root)**.
6. Klik op **Save**.
7. Na publicatie is de app bereikbaar via de GitHub Pages-link die GitHub toont.

## Bestanden

- `index.html` — de volledige app.
- `assets/bonsplitser-logo.png` — het Bonsplitser-logo.
- `assets/favicon.png` — pictogram voor het browsertabblad.

De gewone functies werken volledig lokaal in de browser. Alleen de OCR-code en taalbestanden voor de bon-scanner worden bij gebruik van de scanner vanaf een CDN geladen.
