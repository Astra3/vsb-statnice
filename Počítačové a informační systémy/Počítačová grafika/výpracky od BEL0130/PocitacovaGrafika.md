# 🎨 Počítačová grafika (ZPG, URO)

Tento dokument obsahuje vypracovanie okruhov k predmetu **Počítačová grafika** podľa oficiálnych štátnicových požiadaviek. Využíva GitHub Markdown.

---

## 🧠 1. Metody a nástroje pro realizaci grafických uživatelských rozhraní

## Témata:
- Kognitivní schopnosti člověka  
- Mentální modely  
- Základní pravidla designu  
- Barevné prostory  
- Volba barev a prezentace textu

### 📝 Vypracovanie:

# 🔹 1.1 Kognitivní schopnosti člověka
> Jak lidské vnímání, paměť, pozornost a zrakové rozpoznávání ovlivňují návrh rozhraní.

**Komunikace človeka s programem**
---
1. vstupni informace
2. vyhodnoceni informace
3. stanovení reakce
4. provedení reakce

**reakčný čas**
---

- čas potrebný k vyhodnocení reakce 
- čas potrebný k stanovení reakce
- čas k vykonáni pohybu

Dobre navrhnuté použivateľské rozhranie skracuje čas reakcie a provedení reakce


**fittuv zákon popisuje čas zasažení cíle na obrazovce**
---

<img src="./images/fittuv_zakon.jpg" alt="fittuv zakon">

T - čas k zasažení \
a, b - konštanty \
d - vzdialenosť od cieľa \
s - veľkosť cieľa 

- dôležitá časť fitovho zákona (d/s) kde d je dĺžka a s je veľkosť cieľa. skrátenie času zasiahnutia cieľa priamo súvisí z rýchlosťou provedení reakce. to znamená **čím väčšie a bližšie pri sebe sú elementy ktoré slúžia na ovládanie rozhrania tým lepšie je uživateľské rozhranie**

**čas výberu položiek z menu**
---
<img src="./images/vyber_poloziek_z_menu.jpg" alt="vyber z menu">

T- čas k výberu \
k, c - konštaty \
b - počet položiek 

- výber z menu priamo súvisí z množstvom položiek v menu. čím ma menu menej položiek tým lepšie menu (antipríklad VS menu)



**typy pameti**
---
<img src="./images/tri_typy_pameti.jpg" alt="tri typy pamate">


**krátkodobá pamäť**
---  

rýchle strata zvyčajne si človek pamätá 7 +- 2 položky
> nie je vhodne krátkodobú pamäť preťažovať


**dlhodobá pamäť**
---  
> Uživateľské rozhranie by malo využívať čo najviac dlhodobú pamäť nadobudnutú z ostatných aplikácií napríklad pohyb v menu pomocou šípiek, odoslanie formulára pomocou enteru, pohyb v 3D pomocou WASD a podobne, a čo najmenej meniť ovládanie alebo celkové rozloženie systému.


**Gesalt theory**
---  
<img src="./images/clovek_a_UI8.jpg" alt="gesalt" width="800">
<img src="./images/clovek_a_UI9.jpg" alt="gesalt objekt a pozadie" width="800">
<img src="./images/clovek_a_UI11.jpg" alt="idealizovany tvar" width="800">
<img src="./images/clovek_a_UI12.jpg" alt="blizkost a vytvaranie skupin" width="800">
<img src="./images/clovek_a_UI13.jpg" alt="kontinuita" width="800">
<img src="./images/clovek_a_UI14.jpg" alt="symetria" width="800">
<img src="./images/clovek_a_UI15.jpg" alt="vnimanie na zaklade skusenosti" width="800">

> Gestaltová teorie popisuje, ako človek prirodzene vníma usporiadanie vizuálnych prvkov ako celky namiesto jednotlivostí.  
> V dizajne používateľského rozhrania sa uplatňuje napríklad v princípoch:

- **Objekt a pozadie** – schopnosť oddeliť prvok od pozadia,
- **Idealizovaný tvar** – dopĺňanie neúplných obrazcov do známych tvarov,
- **Blízkosť a vytváranie skupín** – zhlukovanie súvisiacich prvkov,
- **Kontinuita** – vnímanie plynulých línií a usporiadania,
- **Symetria** – rozpoznanie vyvážených, harmonických tvarov,
- **Vnímanie na základe skúsenosti** – rýchla orientácia v známom prostredí.



**8 zlatých pravidiel dobrého UI**
---



---

# 🔹 1.2 Mentální modely
>človek hľadá vo všetkom systém a postúpnosť aby si uľahčil premýšlanie.

<img src="./images/mentalni_model_okna.jpg" alt="vnimanie na zaklade skusenosti">

**mentálne modely formujú realitu do skupín pre jednoduchšie porozumenie systému**

> Když se model podaří nalézt, pak nastupuje:
- pocit jistoty a ovládnutí produktu,
- pocit víry, že lze odhadnout chování v nových situacích, 
- pocit víry, že produkt v nových situacích uspěje. 
> Když ne, pak pocity opačné
- nejistoty, frustrace, skepse
- nejistota, zda pro nové úkoly bude produkt vhodný.

pre dobré uživateľské rozhranie je výhodné mať jednoducho a rýchlo vytvoritelný mentálny model aplikácie. Dá sa využiť už existujúce skúsenosti uživateĺa s mentálnymi modelmi (rozvrhovať rozhranie podľa už existujúceho rozhrania)

tvorba dobrého mentálneho modelu
- Udělejte inventuru veškeré komunikace vašeho programu 
s uživatelem. Rozdělte komunikaci na části, které budou tvořit 
jednotlivá menu, dialogová okna, případně stránky. Obsah oken 
rozdělte na části (max. přibližně 7) obsahující prvky GUI. Menu 
a podmenu organizujte tak aby délka zpravidla nebyla větší než 
max. cca 12 položek.
-  Pro každé okno, skupinu prvků GUI, menu, podmenu nalezněte 
maximálně výstižné názvy (To je naprosto zásadní, a to i tehdy, 
když v GUI některé z nich nakonec nebudou vidět).
- Nakreslete si schéma řazení menu, oken, stránek na papír 
(mentální model GUI). Podobně nakreslete i zamýšlené mentální 
modely jednotlivých oken. 

---

# 🔹 1.3 Základní pravidla designu
---
**1. Konzistence:**
---
- Podobné posloupnosti akcí v podobných situacích
- Konzistentní terminologie (např. na různých místech menu, menu a nápověda, …)
- Podobný vzhled oken, stránek, konzistentní 
používání barev, fontů, grafiky (ikon), … 

**2. Informativni zpětná vazba**
---
- Na každou akci uživatele reagovat zpětnou vazbou 
signalizující, že se něco děje nebo stalo.
- Být tak konkrétní, jak je na základě od uživatele 
získaných informací možné. 

**3. Prevence chyb a řešení chybových situací**
---
- Nedovolte uživateli udělat chybu. Např.: Zakažte 
položky v menu (tlačítka, …), které by v daném 
okamžiku neměly být provedeny. Nedovolte psát 
písmena, když mají vstoupit čísla. Ihned provést 
možné kontroly správnosti (rozsahy atd.).
- Když už chyba vznikne, poskytněte uživateli 
nápovědu, jak ji odstranit.

**4. UNDO možnosť**
---
-  Bez komentáře – prostě vždy a pokud možno na 
všechno. Realizujte také „redo“.

**5. Zkušený uživatel požaduje plnou kontrolu nad produktem**
---
- Jednoduše: Zkušený uživatel chce mít produkt 
zcela „přečtený“. Jestliže se mu nepodaří 
dosáhnout tohoto stavu, produkt se mu nelíbí.

**6. Připravte produkt také pro zkušené uživatele**
---
- Důmyslná GUI vyhovují zpravidla spíše uživateli 
nezkušenému.
- Zkušeného uživatele komplikované GUI při 
provádění běžných akcí obvykle zdržuje (např. 
opakované otvírání víceúrovňových menu pro vy 
volání příkazu).
- Zkušený uživatel přivítá: možnost zápisu příkazu 
(krátká jména příkazů) na příkazový řádek, 
klávesové zkratky, makra, …

**7. Organizujte akce do uzavřených celků**
---
- Komplikované akce s větším počtem kroků 
rozdělte na menší celky mající jasný začátek a 
konec. Po vykonání každého celku zpětná vazba, 
jak to dopadlo. Také velké formuláře rozdělte na 
menší (uživatele o tom ale předem informujte).

**8. Nepřetěžujte krátkodobou paměť a vizuální systém uživatele**
---
- Přiměřený počet položek v menu, tlačítek ve 
skupinách, přehledná a jasná struktura obrazovky 
(okna, stránky).
- Nedopusťte chaos na obrazovce. I 
komplikovanější struktura se ale může stát 
přijatelnou, jestliže je okno, stránka, obrazovka 
vnímáno jako pěkné.


---

# 🔹 1.4 Barevné prostory  
> Využitie farebných priestorov, ich význam v navrhovaní GUI a zásady práce s farbami.

**Základy farebného vnímania**
---
- Farba vzniká ako výsledok interakcie svetla rôznych vlnových dĺžok s čapíkmi v sietnici oka.
- Ľudské oko má 3 typy čapíkov: pre červenú, zelenú a modrú. Najcitlivejšie je na **žltú farbu** (kombinácia červenej a zelenej).
- Približne **8 % populácie má poruchu farebného videnia**, čo je nutné pri návrhu GUI zohľadniť.

<img src="./images/Human_Color_Sensitivity.jpg" alt="rozdielne zastúpenie čapíkov a tyčiniek" width="400">

**Modely farebných priestorov**
---
- **RGB** (Red, Green, Blue) – používa sa pre displeje. Každý pixel má hodnoty R, G a B.
- **HSV** (Hue – odtieň, Saturation – sýtosť, Value – jas) – intuitívnejší pre výber farby.
- **CMY(K)** – subtraktívny model používaný pri tlači (cyan, magenta, yellow, black).

---
<img src="./images/HSV.jpg" alt="farebný kužeľ HSV s kruhom" width="200"> 

HSV kuzel

---
<img src="./images/HSV2.jpg" alt="HSV rozlozenie" width="200">

HSV

---
<img src="./images/CMY.jpg" alt="CMY(K) rozlozenie" width="400">

RGB/CMY(K)

---

**Reprezentácia farieb**
---
- V GUI systémoch sa často používa zápis pomocou RGB zložiek.
- **"Web-safe" farby** – historicky obmedzená paleta 216 farieb kompatibilných s 256-farebnými monitormi (dnes málo významné).

**Farebný kontrast**
---
- Kľúčový pre čitateľnosť – W3C odporúča:
  - Jasový rozdiel (brightness): väčší než 125.
  - Rozdiel zložiek (color difference): väčší než 500.

```plaintext
Brightness = (299×R + 587×G + 114×B)/1000
Color Difference = ∑ max - min pre každú zložku R, G, B
```

**Pravidlá pri výbere farieb v GUI**
---
- **Používaj málo farieb** – menej je často viac.
- **Vyhýbaj sa agresívnym kombináciám** – napr. červená a modrá vedľa seba sú únavné pre zrak.
- **Zvýš kontrast pre zrakovo postihnutých** – pomáha využiť zvyšky farebného vnímania.

<img src="./images/handicaped.jpg" alt="simulácia zhoršeného farebného vnímania" width="300">

**Typy farebných schém**
---
- **Monochromatická** – rôzne jasy a sýtosti jednej farby. Harmonické a nenásilné.
- **Analógová** – farby blízko seba na farebnom kruhu. Fungujú v prírode aj dizajne.
- **Komplementárna** – farby oproti sebe na farebnom kruhu. Veľmi kontrastné, opatrne s použitím pri texte.

<img src="./images/RCW.jpg" alt="farebný kruh s teplými a studenými farbami" width="500">

**Teplé a studené farby**
---
- **Teplé** (červená, oranžová, žltá) – pôsobia aktívne, energicky.
- **Studené** (modrá, zelená) – pôsobia upokojujúco a pasívne.


**Farebné schémy v praxi**
---
- Príroda aj umenie ponúkajú inšpirácie – napr. Monet, Van Gogh, Vermeer.
- **Príklady z výtvarného umenia** ukazujú, ako kombinovať kontrast, sýtosť a teplotu farieb.

<img src="./images/similar_color.jpg" alt="blízke farby v praxi" width="600">

blizke farby sa nachádzajú v malom kruhu na z velkeho HSW

---
<img src="./images/Complementary.jpg" alt="komplementárne farby" width="600">

komplementárne sa nachádzajú dva kruhove vyrezy oproti sebe na HSW (2 monochromaticke farby tvoriace komplementarne farby)


<img src="./images/Monet.jpg" alt="Monet – rozvetvená komplementárna schéma" width="600">

volba farieb podla moneta 3 kruhove vyrezy tvoriace "radioaktivny piktogram" (3 monochromaticke tvoriace komplementarne farby)


**Zásady pre návrh UI z hľadiska farieb**
---
- Zachovaj konzistenciu v použitých farbách naprieč aplikáciou.
- Biela alebo veľmi svetlá farba je najvhodnejšia pre pozadie s textom.
- Sýte farby používaj na zvýraznenie, ale šetrne.
- Uvažuj aj kultúrne a emocionálne asociácie farieb.





---

# 🔹 1.5 Volba barev a prezentace textu
> Kontrast, čitelnost, barvoslepost, výběr barev pro různé režimy (dark/light mode).

---

**Prezentácia textu – dôležité zásady**
---

- Texty musia byť vizuálne usporiadané tak, aby uľahčovali čítanie a zapamätanie obsahu.
- Dôležité informácie zvýrazni nadpisom, vizuálnou hierarchiou alebo obrázkom.
- Vzhľad stránky priamo ovplyvňuje, či bude čitateľ ochotný pokračovať v čítaní.

<img src="./images/Text_Organization.jpg" alt="Zlé a dobré usporiadanie textu" width="400">

zlé/dobré

---

**Organizácia textu a čitateľnosť**
---

- Vizuálna štruktúra pomáha čitateľovi vytvoriť si **mentálny model** stránky.
- Odporúča sa rozbíjať text do kratších odstavcov, používať odrážky, deliace prvky a nadpisy.
- Dlhé riadky znižujú čitateľnosť – ideálne je **60–70 znakov na riadok**.

<img src="./images/Text_Organization2.jpg" alt="Vnímanie dlhých riadkov" width="400">

zlé/dobré

---

**Sadzba textu a zarovnanie**
---

- **Obojstranné zarovnanie** (justifikácia) vytvára tzv. „rieky“ – vizuálne prázdne pásy, ktoré zhoršujú čitateľnosť, najmä pre dyslektikov.
- **Zarovnanie naľavo** je preferované – lepšie sa sleduje, menší vizuálny stres.
- Príliš dlhé alebo zložité vety znižujú zrozumiteľnosť. Krátke, jasné vety sú vhodnejšie.

<img src="./images/Text_Organization3.jpg" alt="obojstranne zarovnanie" width="300">
<img src="./images/Text_Organization4.jpg" alt="zarovnanie na lavo a skratenie riadkov" width="300">

zlé/dobré



---

**Výber fontov a štýlu písma**
---

- Používaj max. 2 fonty a 3 veľkosti písma.
- Kurzíva a tučné písmo len výnimočne – sú horšie čitateľné.
- NEpoužívaj celé slová veľkými písmenami (napr. NADPISY).
- Nezabudni na antialiasing pre malé písmo – znižuje „zúbky“.
- **Bezpatkové fonty (sans-serif)** sú na obrazovke čitateľnejšie ako klasické knižné (serif).

<img src="./images/Fonts.jpg" alt="Výber fontu a jeho čitateľnosť" width="600">

---

**Pozadie a kontrast**
---

- Vhodné pozadie je kľúčové – najlepšia je **biela alebo veľmi svetlá farba**.
- Kontrast písma voči pozadiu musí byť dostatočný.
- W3C odporúča:
  - **Brightness difference > 125**
  - **Color difference > 500**

```plaintext
Brightness = (299×R + 587×G + 114×B)/1000
Color Difference = ∑ max - min pre R, G, B
```

<img src="./images/Font_bg.jpg" alt="Pozadie a čitateľnosť textu" width="800">

---

**Dostupnosť pre zrakovo postihnutých**
---

- Približne **8 % populácie má poruchy farebného videnia**.
- Riešenie: **zvýšiť farebný kontrast** a zamedziť použitiu červeno-zelených kombinácií.
- Dôležité je testovať aj tzv. **dark mode** aj **light mode** – každý režim má iné požiadavky na kontrast.

<img src="./images/Handicaped2.jpg" alt="Simulácia porúch farebného videnia" width="500">

---

**Zhrnutie pre návrh textovej prezentácie v GUI**
---

- Vždy myslieť na **konzistentnú štruktúru a hierarchiu**.
- Zohľadniť fyziológiu zraku a schopnosť čítania z obrazovky.
- Vyhýbaj sa čisto dizajnérskym rozhodnutiam – priorita je **čitateľnosť**.
- Dbaj na rozdiely medzi výstupom na papier a obrazovku – DPI, fonty, štýly.




---


## 🖼️ 2. Standardní zobrazovací řetězec

### Témata:
- Realizace jednotlivých kroků řetězce  
- Modelovací a zobrazovací transformace  
- Phongův osvětlovací model  
- Řešení viditelnosti  
- Identifikace těles  
- Stručná charakteristika OpenGL a jazyka GLSL

### 📝 Vypracovanie:



---

## 📐 3. Geometrické modelování

### Témata:
- Afinní a projektivní prostory  
- Popis těles a možnosti jejich reprezentace  
- Základní křivky (Fergusonova kubika, Bézierova křivka)  
- Vlastnosti a použití týchto kriviek

### 📝 Vypracovanie:


---

## ❓ Příkladová otázka

> **Popište možnosti reprezentace těles a způsob jejich vykreslení pomocí standardního zobrazovacího řetězce v kontextu grafického rozhraní OpenGL.**

---

