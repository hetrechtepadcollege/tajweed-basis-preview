# De Tuin van Dzikr — App instructies

## Doel
Een visuele dzikr-app waarbij de tuin groeit naarmate de gebruiker dzikr doet. Doelgroep: kinderen (6-12), tieners en volwassenen/ouders.

## Dzikr-types
- **SubhanAllah** (سُبْحَانَ اللّٰهِ) — roept bloemen op
- **Alhamdulillah** (اَلْحَمْدُ لِلّٰهِ) — roept bomen op
- **Allahu Akbar** (اَللّٰهُ اَكْبَرُ) — roept ster-bloesems op

## Persistentie
- Tuin-staat wordt opgeslagen in `localStorage` (sleutel: `dzikrGardenState`)
- Reset-knop verwijdert de staat na bevestiging

## GoatCounter events
- `tuin-van-dzikr/app-gestart` — bij laden
- `tuin-van-dzikr/tap/{type}` — bij elke dzikr-tap
- `tuin-van-dzikr/mijlpaal/{type}-{aantal}` — bij 33, 99, 333 taps
- `tuin-van-dzikr/tuin-gereset` — bij reset

## Technische notities
- Alle JavaScript staat inline in `index.html` (geen `script.js`)
- Plant-animaties zijn pure CSS (geen canvas, geen externe libraries)
- Arabische tekst: `AlQalamQuranMajeed` font, `<p dir="rtl" lang="ar">`
