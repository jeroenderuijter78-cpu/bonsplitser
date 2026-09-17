# Klopt!

**Klopt!** is een mobiele web-app van JerApps.nl om rekeningen en gezamenlijke kosten eerlijk te verdelen.

## Mogelijkheden

- **Live bijhouden** wie wat neemt tijdens het eten of drinken.
- **Bon scannen** met de camera of een bestaande foto.
- Bonregels na de scan altijd **controleren en corrigeren**.
- Automatische rekencontrole: bonregels + fooi tegenover het betaalde totaal.
- Een bon achteraf handmatig invoeren en verdelen.
- Gedeelde hapjes gelijk verdelen, aantallen gebruiken of vrije bedragen invoeren.
- Fooi gelijk of naar rato verdelen.
- **Uitje verrekenen**: meerdere voorschotten en kosten verwerken en automatisch zien wie aan wie betaalt.
- Eindafrekeningen delen, kopiëren, downloaden als tekst of afdrukken / opslaan als PDF.

## Bon scannen

De scanfunctie gebruikt Tesseract.js in de browser. De foto wordt op het apparaat verwerkt; er is geen eigen server of API-sleutel nodig. Bij de eerste scan is internet nodig om de OCR-bibliotheek en taalbestanden te laden.

OCR kan fouten maken. Daarom toont Klopt! na iedere scan eerst een controlescherm. De app vergelijkt bovendien de som van de gevonden regels en de fooi met het totaal op de bon.

## Publicatie

De app staat op GitHub Pages. De repository heet om historische redenen nog `bonsplitser`; de publieksnaam van de app is **Klopt!**.

Gemaakt door **JerApps.nl**.
