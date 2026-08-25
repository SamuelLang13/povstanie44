# Povstanie 44 🇸🇰

**Interaktívna mapa a časová os Slovenského národného povstania (29. august – 30. október 1944).**

🔗 Živá stránka: https://povstanie44.sk _(po nasadení)_

## Čo stránka obsahuje

- **Interaktívna mapa** postavená na OpenStreetMap (Leaflet) — front sa deň po dni mení podľa časovej osi
- **Tri prepínateľné vrstvy územia**: povstalecké územie (biele), sovietsky postup pri Karpatsko-duklianskej operácii (modré), nemecká okupácia (červená)
- **Vojenské emblémy jednotiek** priamo na mape — slovenský dvojkríž, partizánska hviezda, nemecký železný kríž (vlastná kresba, žiadne cudzie logá ani zakázané symboly)
- **Časová os** s krokovaním po dňoch/týždňoch, nastaviteľnou rýchlosťou a plynulými prechodmi
- **Klikateľné značky** — velitelia, taktické skupiny, partizáni, nemecké jednotky, vedenie Slovenského štátu, Východoslovenská armáda, dôležité mestá, letiská, vypálené obce, miesta popráv, ďalšie osobnosti SNP
- **Plnohodnotný informačný web** s podstránkami: Pozadie a príčiny, Velenie a štát, Osobnosti SNP, Taktické skupiny, Partizáni a Nemci, Mestá a letiská, Represálie, Bilancia a dôsledky, Pamäť dnes, Kompletná chronológia, Slovníček pojmov, Zdroje
- **Zdieľateľné odkazy** na konkrétne záložky aj jednotlivé osoby/miesta (`#reprisals/klak`, `#command/tiso`...)
- Historické fotografie s overenou public domain / CC licenciou (Wikimedia Commons)

## Technológie

Jeden samostatný `index.html` súbor — žiadny build proces, žiadne závislosti na inštaláciu.

- [Leaflet.js](https://leafletjs.com/) (cez CDN) — mapová knižnica
- Mapové dlaždice: [CARTO Dark Matter](https://carto.com/basemaps) (postavené na dátach OpenStreetMap)
- Fonty: Spectral, Source Sans 3, JetBrains Mono (Google Fonts)
- Čistý HTML/CSS/JavaScript, žiadny framework

## Lokálne spustenie

Stačí otvoriť `index.html` v ľubovoľnom modernom prehliadači. Pre plnú funkčnosť (najmä mapové dlaždice) je potrebné pripojenie na internet.

```bash
git clone https://github.com/VASE-MENO/povstanie44.git
cd povstanie44
open index.html   # macOS
# alebo len dvojklik na súbor
```

## Nasadenie na GitHub Pages s vlastnou doménou

1. V nastaveniach repozitára **Settings → Pages** zvoľ zdroj `Deploy from a branch`, vetvu `main`, priečinok `/ (root)`.
2. Súbor `CNAME` v tomto repozitári už obsahuje `povstanie44.sk` — GitHub Pages ho automaticky použije.
3. U svojho registrátora domény (napr. WebSupport, Wedos) nastav DNS záznam typu `CNAME` smerujúci `povstanie44.sk` na `VASE-MENO.github.io` (alebo `A` záznamy na GitHub Pages IP adresy, ak chceš apex doménu — pozri [oficiálny návod GitHub](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site)).
4. Počkaj na overenie DNS (môže trvať niekoľko hodín) a zapni v nastaveniach **Enforce HTTPS**.

## Presnosť a zdroje

Ide o vzdelávací projekt, nie o akademickú publikáciu. Hranice frontu, vrstva nemeckej okupácie aj poloha niektorých bodov sú zámerne zjednodušené a orientačné — presné zdroje sú uvedené v záložke **Zdroje** priamo na stránke a pri každej jednotlivej karte. Pri chybe alebo spresnení, prosím, otvor [issue](../../issues) alebo pošli pull request.

Hlavné použité zdroje: Múzeum SNP, Ústav pamäti národa, Vojenský historický ústav, Wikipédia, Ministerstvo obrany SR, Denník N / HistoryLab.sk a ďalšie — plný zoznam v záložke Zdroje na stránke.

## Licencia

- **Kód** (HTML/CSS/JS v tomto repozitári): [MIT licencia](LICENSE) — voľne použiteľné, upraviteľné, šíriteľné.
- **Historický textový obsah**: spracované na základe verejne dostupných zdrojov citovaných v aplikácii; pri ďalšom šírení odporúčame uviesť pôvodné zdroje.
- **Fotografie**: každá má vlastnú licenciu uvedenú priamo pri nej (verejná doména alebo Creative Commons, Wikimedia Commons) — rešpektujte konkrétnu licenciu daného súboru.
- **Mapové dáta**: © prispievatelia OpenStreetMap, dlaždice cez CARTO.

## Prispievanie

Historické korekcie, doplnenie ďalších osobností/udalostí či technické vylepšenia sú vítané cez pull request alebo issue.
