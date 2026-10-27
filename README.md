# Gapahuken

En minimalistisk presentasjon om MVP: hvorfor det er bedre å bygge en gapahuk enn et slott når noen står ute i regnet.

Skrevet i Markdown, med [Marp](https://marp.app).

## Se presentasjonen

Krever Node 18 eller nyere.

```sh
npm install
npm run dev
```

Åpne <http://localhost:8080/slides.md>. Siden oppdateres når du lagrer `slides.md` eller `theme.css`.

Vil du presentere i eget vindu?

```sh
npm run present
```

Talernotatene ligger som skjulte kommentarer i `slides.md`. Åpne presentatørvisningen med ikonet nederst i presentasjonen.

## Bygg

```sh
npm run build   # lager slides.html
npm run pdf     # lager gapahuken.pdf (bruker Chrome)
```

`slides.html` er en selvstendig side, men henter bilder og fonter fra `images/` og `fonts/`. Flytt hele mappen hvis du skal vise den fra en annen maskin.

## Rediger

- `slides.md` — all tekst. `---` skiller lysbildene.
- `theme.css` — typografi, farger og bildebehandling.
- `images/` — bilder beskåret til 16:9.
- `fonts/` — lokale woff2-fonter, så presentasjonen virker offline.

Bytte av bilde gjøres med en Marp-direktiv:

```md
![bg](images/mitt-bilde.jpg)
```

Varianter: `![bg right](...)`, og klassene `photo`, `photo center`, `photo right`, `photo light`, `cover`, `statement`, `list`, `steps` og `credits`.

## Bilder

Alle bildene er hentet fra Wikimedia Commons og brukt under sine respektive lisenser.

| Bruk    | Bilde                                                                                                                                         | Fotograf        | Lisens       |
| ------- | --------------------------------------------------------------------------------------------------------------------------------------------- | --------------- | ------------ |
| Forside | [Misty Mountains](<https://commons.wikimedia.org/wiki/File:Misty_Mountains_(Unsplash_zR40wedS1aQ).jpg>)                                       | James Bloedel   | CC0          |
| Regn    | [Rain on a puddle in Tuntorp 1](https://commons.wikimedia.org/wiki/File:Rain_on_a_puddle_in_Tuntorp_1.jpg)                                    | W.carter        | CC BY-SA 4.0 |
| Person  | [Beyond the fog](<https://commons.wikimedia.org/wiki/File:Beyond_the_fog_(Unsplash).jpg>)                                                     | Jorge Fernández | CC0          |
| Slott   | [Palace Neuschwanstein](<https://commons.wikimedia.org/wiki/File:Palace_Neuschwanstein_(Unsplash).jpg>)                                       | Mathias Konrath | CC0          |
| Gapahuk | [Biscuit Brook Lean-To](https://commons.wikimedia.org/wiki/File:Biscuit_Brook_Lean-To,_Frost_Valley,_NY.jpg)                                  | Daniel Case     | CC BY-SA 4.0 |
| Test    | [Aftermath of an ice rain in the forest](https://commons.wikimedia.org/wiki/File:Aftermath_of_an_ice_rain_in_the_forest,_Vienna,_Austria.jpg) | Simon           | CC BY 2.0    |
| Vegg    | [Biscuit Brook Lean-To 2](https://commons.wikimedia.org/wiki/File:Biscuit_Brook_Lean-To,_Frost_Valley,_NY_2.jpg)                              | Daniel Case     | CC BY-SA 4.0 |
| Tåke    | [Burg Hohenzollern](https://commons.wikimedia.org/wiki/File:Burg_Hohenzollern-101611.jpg)                                                     | Rainer Halama   | CC BY-SA 4.0 |
| Bål     | [Bonfire and Sun](<https://commons.wikimedia.org/wiki/File:Bonfire_and_Sun_(54056503423).jpg>)                                                | Egor Plenkin    | CC BY 2.0    |

Bildene er beskåret til 16:9, men ellers ikke endret.

## Fonter og verktøy

- [Cormorant Garamond](https://fonts.google.com/specimen/Cormorant+Garamond) — SIL Open Font License
- [EB Garamond](https://fonts.google.com/specimen/EB+Garamond) — SIL Open Font License
- [Marp](https://marp.app) — MIT

Presentasjonen har ingen innholdsmessig avhengighet til internett. Alt ligger lokalt.
