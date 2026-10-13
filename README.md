# Cvičebnice

Interaktívne cvičebnice na precvičovanie školských predmetov. Každý príklad sa generuje nový, odpoveď sa automaticky skontroluje a ku každému príkladu je k dispozícii postup riešenia. Popri cvičení si môžeš otvoriť aj teóriu z prednášok.

Je to statická stránka: žiadny server, žiadna inštalácia, všetko beží v prehliadači.

## Cvičebnice

| Predmet | Priečinok | Obsah |
|---|---|---|
| **ADM** | [`amd/`](amd/) | Matice, sústavy lineárnych rovníc, Gaussova eliminácia, inverzná matica, determinanty |
| **PPI** | [`ppi/`](ppi/) | Booleove funkcie, normálne formy (MDNF, MKNF), Karnaughove mapy, logické obvody, automaty, preklápacie obvody |
| **MA** | [`ma/`](ma/) | Funkcie, polynómy, elementárne funkcie, limity a spojitosť, derivácie, Taylorov polynóm, l'Hospital, priebeh funkcie |

## Čo cvičebnice ponúkajú

- **Nekonečne veľa príkladov.** Zadania sa generujú náhodne, takže sa nikdy nezopakujú.
- **Kontrola odpovede.** Čísla, zlomky (`2/7`), výrazy (`sqrt(3)/2`, `pi/6`), zoznamy, výber z možností aj voľne zapísané výrazy (pri deriváciách sa porovná funkcia, nie tvar zápisu).
- **Postup riešenia** ku každému príkladu, pri niektorých aj s grafom.
- **Karta „Teória + cvičenie“.** Teória z prednášok vedľa príkladov, aby si ju mohol hneď vyskúšať.
- **Štatistika.** Úspešnosť na prvý pokus za každú tému, aktuálna a najlepšia séria. Ukladá sa v prehliadači (`localStorage`), tlačidlom „Vynulovať štatistiku“ ju vymažeš.
- **Svetlý aj tmavý režim**, použiteľné na mobile.

## Štruktúra repozitára

```
.
├── index.html        # úvodná stránka s odkazmi na jednotlivé cvičebnice
├── amd/index.html    # Cvičebnica ADM
├── ppi/index.html    # Cvičebnica PPI
├── ma/index.html     # Cvičebnica MA
└── README.md
```

Každá cvičebnica je jeden samostatný súbor `index.html` (HTML, CSS a JavaScript dokopy). Jediná externá závislosť sú písma z Google Fonts, bez nich sa použijú systémové.

## Nasadenie na GitHub Pages

1. V repozitári otvor **Settings → Pages**.
2. V časti **Build and deployment** vyber **Deploy from a branch**, vetvu `main` a priečinok `/ (root)`.
3. Po minúte-dvoch bude stránka dostupná na `https://<používateľ>.github.io/<repozitár>/`.

Cvičebnice sa potom otvárajú na `…/amd/`, `…/ppi/` a `…/ma/`. Lokálne stačí otvoriť `index.html` v prehliadači.

## Pridanie ďalšej cvičebnice

1. Vytvor nový priečinok (napr. `xyz/`) a daj do neho `index.html`.
2. Pridaj do neho odkaz späť: `<a class="backlink" href="../">← Cvičebnice</a>`.
3. V koreňovom `index.html` pridaj ďalšiu kartu (`<a class="card" href="xyz/">…</a>`).

## Poznámka

Príklady a postupy sú generované programom a overované automatickými testami, no môžu v nich ostať chyby. Ak niečo nesedí, ber to ako podnet pozrieť si prednášku alebo skontrolovať výsledok inak.
