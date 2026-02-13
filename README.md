# Talarklokke

> **A single-file countdown timer for seminars and conferences.** Click a preset button to start counting down. Designed for projecting on a screen so speakers can see their remaining time. No dependencies, no build step — just open `index.html` in a browser.

---

## Kva er dette?

Talarklokke er eit enkelt nedteljingsverktøy laga for seminar og konferansar der fleire talarar har ulik taletid. I staden for å halda styr på klokka og rekna ut når kvar talar skal vera ferdig, trykker du berre på ein knapp — til dømes **10 min** — og nedteljinga startar med ein gong.

Alt ligg i éi einaste HTML-fil. Ingen avhengnadar, ingen byggesteg, ingen server. Opne fila i ein nettlesar, og du er klar.

## Funksjonar

- **Stor retro sjusegment-visning** med DSEG7 Classic-skrifttypen
- **Eittklikksnedteljing** — trykk på ein knapp, og tida startar å renna
- **Tilpassbare knappar** — standardverdiar er 2, 5, 10, 15 og 20 minutt, men du kan leggja til, fjerna og endra via redigeringsmodusen
- **-1 / +1 min** — juster tida medan nedteljinga går (nyttig når ting tek litt lenger eller kortare tid enn planlagt)
- **Fargekodar** — kvit tekst medan tida går, raud under 30 sekund, blinkande raud når tida er ute
- **Gul pause** — teksten vert gul og blinkar sakte når du set på pause
- **«TIDA ER UTE»** — melding og overtidsteljar (+00:00) når tida går ut
- **Lydsignal** — tretonig bjelleklang via Web Audio API (ingen eksterne lydfiler)
- **Fullskjerm** — perfekt for projisering
- **Fungerer utan nett** — etter at skrifttypen er lasta inn fyrste gong, treng du ikkje internett
- **Lagrar innstillingar** — tilpassa knappar vert lagra i localStorage

## Bruk

1. Opne `index.html` i ein nettlesar
2. Trykk på ein av tidsknappane for å starta nedteljinga
3. Bruk **FULLSKJERM** for å visa på ein projektor

## Tastatursnarvegar

| Tast | Handling |
|------|----------|
| `Mellomrom` | Pause / fortset |
| `Escape` | Nullstill |
| `F` | Fullskjerm |
| `S` | Lyd av/på |
| `Pil opp` | +1 minutt |
| `Pil ned` | -1 minutt |

## Tilpassing

Trykk **REDIGER** for å opna redigeringspanelet. Der kan du:

- Endra varigheita på eksisterande knappar
- Fjerna knappar du ikkje treng
- Leggja til nye knappar

Trykk **Lagre** når du er ferdig. Innstillingane vert lagra i nettlesaren og er der neste gong du opnar sida.

## Teknisk

- Éi HTML-fil med innebygd CSS og JavaScript
- [DSEG7 Classic](https://github.com/keshikan/DSEG)-skrifttypen (lasta via CDN)
- Tidtaking basert på `performance.now()` for nøyaktig nedteljing sjølv om nettlesarfana er i bakgrunnen
- Lydsignal laga med Web Audio API (sinustonar, ingen eksterne filer)
- Førehandsval lagra i `localStorage`

## Lisens

MIT
