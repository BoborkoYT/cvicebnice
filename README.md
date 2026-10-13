# Cvičebnice

Interaktívne cvičebnice na skúšky: **ADM**, **PPI** a **MA**. Otvoríš, vyberieš tému a počítaš. Každý príklad je nový, odpoveď sa hneď skontroluje a vždy si môžeš pozrieť postup.

Statická stránka, bez servera a bez inštalácie, všetko beží v prehliadači.

## Čo sa tu ponúka

### ADM (`amd/`)
Matice, sústavy lineárnych rovníc, Gaussova eliminácia, inverzná matica a determinanty.

### PPI (`ppi/`)
Booleove funkcie, MDNF a MKNF, Karnaughove mapy, logické obvody, automaty a preklápacie obvody.

### MA (`ma/`)
Funkcie, polynómy a racionálne funkcie, elementárne funkcie, limity a spojitosť, derivácie, dotyčnice a diferenciál, Taylorov polynóm, l'Hospital a priebeh funkcie.

### Spoločné vlastnosti
- Príklady sa generujú náhodne, nikdy sa nezopakujú.
- Kontrola odpovede: čísla, zlomky (`2/7`), výrazy (`sqrt(3)/2`, `pi/6`), zoznamy, výber z možností. Pri deriváciách sa porovnáva funkcia, nie tvar zápisu.
- Postup riešenia ku každému príkladu, pri mnohých aj s obrázkom (graf, stavový diagram, priamky sústavy).
- **Teória + cvičenie:** teória z prednášok vedľa príkladov. Po chybe je pri správe odkaz na teóriu k danej téme.
- **Skúška:** vyber témy, počet príkladov a časový limit. Odpovede sa nekontrolujú hneď, na konci je výsledok, rozbor po témach a postupy.
- **Slabé miesta:** stránka si pamätá typy príkladov, ktoré ti nešli, a môže ich ponúkať častejšie.
- **Ťahák:** zhrnutie všetkých tém na jednej strane, ktorú sa dá vytlačiť.
- **Kartičky:** pojmy a pravidlá, otočíš a označíš, či si to vedel.
- **Pracovný list na tlač:** príklady s prázdnymi riadkami a riešeniami na ďalšej strane.
- **Štatistika:** úspešnosť za tému, séria správnych odpovedí v rade. Dá sa exportovať do súboru a importovať na inom zariadení.
- Svetlý aj tmavý režim, funguje na mobile.

### Obrázky a interaktívne pomôcky
- **MA:** grafy základných funkcií, limity, dotyčnice a Taylorove polynómy, a posuvníky: parametre sínusovky, dotyčnica a jej bod, funkcia a jej derivácia, stupeň Taylorovho polynómu, kubická funkcia s extrémami a ε–δ pri limite.
- **PPI:** stavové diagramy automatov Moore a Mealy, prehrávač po krokoch so zvýraznením stavu a časové diagramy preklápacích obvodov D, T a JK.
- **ADM:** sústava dvoch rovníc ako dve priamky s priesečníkom.

## Ako to vzniklo

Lenivo. Žiadne ručné programovanie ani vypisovanie príkladov.

1. Do Claude som nahral PDF z prednášok.
2. Napísal som jednu vetu typu „urob mi z toho interaktívnu stránku, kde si to budem môcť precvičiť“.
3. Claude z prednášok vytiahol témy, napísal generátory príkladov s riešeniami, teóriu aj celé rozhranie.
4. Chyby som len zahlásil (screenshot, „toto nesedí“) a Claude ich opravil. Karnaughove mapy sa napríklad prerobili podľa referenčného súboru, ktorý som mu poslal.
5. Výsledok sa otestoval automaticky: tisíce vygenerovaných príkladov, kontrola odpovedí a pri limitách a deriváciách aj číselné overenie.

Ostatné (hosting, úvodná stránka, tlačidlá späť, tento README) išlo tou istou cestou, vždy jednou vetou.

## Upozornenie

Príklady, postupy aj teória sú generované a overované testami, no môžu v nich ostať chyby. Pri pochybnostiach ber prednášku ako smerodajnú.
