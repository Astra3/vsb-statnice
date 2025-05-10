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

#### 🔹 Barevné prostory



---

#### 🔹 Volba barev a prezentace textu
> Kontrast, čitelnost, barvoslepost, výběr barev pro různé režimy (dark/light mode).


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

