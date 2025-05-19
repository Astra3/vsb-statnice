# Otázky u státnic
Tento dokument obsahuje primárně otázky (u některých i stručné odpovědi), na které se komise ptá u státnic. Děkuji mimuss za sepsání otázek. Dokument potřebuje v některých částech úpravy formátování, nebojte se poslat PR.

# Počítačové a informační systémy

## Programování

### UPR/FPR/C#/JAVA
1. **Paradigmata programování** *(Sawa)*
   * Imperatívne, objektové, funkcionálne, deklaratívne.
   * Rozdiely: stav vs. bezstavovosť, vedľajšie efekty.
   * Príklady jazykov pre jednotlivé paradigmy.

2. **Dynamicky/staticky typované jazyky, generické typy** *(Sawa)*
   * Príklady jazykov (Python vs. Java).
   * Výhody/nevýhody.
   * Generické typy – ako fungujú v C++, Jave.
   * Rozdiel medzi jednoduchými (int, float) a štruktúrovanými typmi (struct, class).

<details>
  <summary>Stručná odpověď</summary>
  V staticky typovaných jazykoch (napr. C, Java) je typ premenných známy už v čase prekladu. Programátor musí výslovne uviesť typ, a prekladač ho skontroluje. To umožňuje skorú detekciu chýb a optimalizáciu kódu.

  Naopak, dynamicky typované jazyky (napr. Python, JavaScript) určujú typ premenných až za behu programu. Typ sa môže zmeniť, čo zvyšuje flexibilitu, ale aj riziko chýb.

  **Výhody statickej typovosti:**
  - Lepšia optimalizácia.
  - Menšie riziko runtime chýb.
  - Podpora nástrojov ako IntelliSense.

  **Výhody dynamickej typovosti:**
  - Rýchlejší vývoj.
  - Flexibilita v práci s dátami.

  Moderné jazyky ako TypeScript alebo Python s type hintingom sa snažia kombinovať výhody oboch prístupov.
</details>

3. **Funkce v C, vlastnosti a rekurze** *(Dohnálek)*
   * Deklarácia, definícia, premenne, návratové hodnoty.
   * Rekurzia – príklady, zásobník volaní.
   * Statické vs. dynamické premenne vo funkciách.
   * Inline, externé, globálne funkcie.

4. **Funkcionální programování, vícenásobné funkce, rozdíly oproti imperativnímu** *(Vasinek)*
   * Hlavné črty FP: bezstavové funkcie, bez vedľajších efektov, funkcie ako objekty.
   * Pure functions, vyššie-rádové funkcie, lambda výrazy.
   * Lazy evaluation.
   * Porovnanie s imperatívnym programovaním (napr. for-cykly vs. map/reduce).
   * Príklady v jazykoch ako Haskell, OCaml, F#.
   * Closure, currying, referenčná transparentnosť.

5. **Datové Struktury (Radecký)**
   * Základné štruktúry: pole, zoznamy, zásobník, fronta, strom, graf.
   * Rozdiely medzi lineárnymi a nelineárnymi štruktúrami.
   * Implementácia – dynamická vs. statická pamäť.
   * Výhody/nevýhody jednotlivých štruktúr.
   * Zložitosť operácií (vkladanie, mazanie, vyhľadávanie).
   * Hashovanie a hash tabuľky.

6. **Rekurze, typy, účel, příklady použití (Kudělka)**
   * Čo je rekurzia – forma riešenia problémov volaním funkcie samej seba.
   * Typy rekurzie: priama, nepriama, nekonečná, koncová (tail-recursion).
   * Príklady: faktoriál, Fibonacci, hľadanie cesty v grafe, triedenia.
   * Výhody/nevýhody oproti iteratívnemu riešeniu.
   * Pamäťové nároky – zásobník volaní.
   * Optimalizácia rekurzie.

7. **Datové typy a správa paměti (Janoušek)**
   * Primitívne a zložené dátové typy.
   * Statická vs. dynamická alokácia.
   * Správa pamäti v C++ (new/delete), garbage collection (v iných jazykoch).
   * Heap vs. stack pamäť.
   * Problémy: memory leaks, dangling pointers.
   * Alignement a padding v pamäti.

8. **Mapování UML na kód (Janoušek)**
   * Prevod triednych diagramov UML do objektovo orientovaného kódu.
   * Asociácie, generalizácia, kompozícia vs. agregácia – ako sa implementujú.
   * Použitie nástrojov (napr. Enterprise Architect, StarUML).
   * Zásady čistého návrhu a SOLID princípy.
   * Príklad triedneho diagramu + jeho prepis do kódu.

### OOP
1. **Principy OOP s důrazem na C++ (časná vazba, pozdní vazba...)** *(Kudělka)*
   * 4 základné princípy OOP: dedičnosť, zapúzdrenie, polymorfizmus, abstrakcia.
   * Statická (časná) väzba vs. dynamická (pozdejší) väzba.
   * Virtuálne funkcie, vtable.
   * Príklady na polymorfizmus (preťažovanie, pretieňovanie).
   * Konštruktory, destruktory, správa zdrojov (RAII).

2. **OOP - dědičnost, zapouzdření, interface, abstraktní třída...** *(Fusek)*
   * Definícia a použitie zapúzdrenia (modifikátory prístupu).
   * Dedičnosť (jednoduchá, viacnásobná, virtuálna v C++).
   * Rozdiel medzi rozhraním a abstraktnou triedou.
   * Príklady implementácie rozhrania (napr. v Jave vs. C++).
   * Výhody použitia abstrakcie a znovupoužiteľnosti kódu.

## Softwarové inženýrství

### SWI
1. **Životní cyklus softwaru** *(Štolfa)*
   * Modely: vodopád, iteratívny, agilný, spiral.
   * Fázy: analýza, návrh, implementácia, testovanie, údržba.
   * Výhody/nevýhody jednotlivých modelov.
   * Rola zákazníka v procese.

<details>
  <summary>Stručná odpověď</summary>
  Životný cyklus softvéru zahŕňa všetky fázy vývoja od požiadaviek až po údržbu. Klasický model je vodopádový, ale existujú aj iteratívne a agilné prístupy.

  Fázy životného cyklu:

  - **Zber a analýza požiadaviek** &mdash; komunikácia s klientom, dokumentácia požiadaviek (napr. pomocou UML).
  - **Návrh** &mdash; návrh architektúry, tried, databázy – UML diagramy ako triedne, sekvenčné.
  - **Implementácia** &mdash; samotné programovanie podľa návrhu.
  - **Testovanie** &mdash; jednotkové, integračné, systémové, akceptačné testy.
  - **Nasadenie** &mdash; uvedenie systému do prevádzky.
  - **Údržba** &mdash; oprava chýb, aktualizácie, reakcie na zmenu požiadaviek.

  Agilné metodiky (napr. Scrum) zdôrazňujú iterácie, spätnú väzbu a priebežné testovanie. Cieľom životného cyklu je minimalizovať riziká a maximalizovať kvalitu softvéru.
</details>

2. **UML, class diagram** *(Štolfa a Fusek)*
   * UML – účel, typy diagramov.
   * Class diagram – atribúty, metódy, vzťahy: asociácia, dedičnosť, kompozícia.
   * Príklad návrhu systému (napr. knižnica, e-shop).

3. **Dynamický pohľad, sekvenčné/aktivity diagramy** *(Štolfa a Kudělka)*
   * **Sekvenčný diagram** &mdash; interakcie objektov v čase.
   * **Activity diagram** &mdash; priebeh činností, podmienky, vetvenie.
   * **Dynamický pohľad** &mdash; ako sa systém chová, nie ako vyzerá.
   * Príklady s konkrétnou úlohou (napr. „pridanie produktu do košíka“).
7. Co je případ užití (use case) a jak vypadá diagram?
8. Jaký je rozdíl mezi aktérem, use casem, user story?
9. Jaké jsou vztahy mezi use casy? (include vs. extend)
10. Co je třídní diagram, stavový diagram, sekvenční diagram?

### VIS

1. **Návrhové vzory** *(Radecký, Štolfa, Gajdoš, Kudělka)*
   * **Observer, Composite** – vzory: účel, UML diagram, reálne použitie.
   * Singleton, Factory, Strategy, MVC, Adapter...
   * Ako vybrať vhodný návrhový vzor.
   * Diagram + implementácia.
   * Otázky na **praktické využitie** v projektoch.

<details>
<summary>Stručná odpověď</summary>
  Observer (pozorovateľ) je návrhový vzor typu behaviorálny. Rieši situáciu, keď objekt (subject) potrebuje informovať viacero ďalších objektov (observerov) o zmene svojho stavu. Implementace probíhá tak, že subject má seznam observerů, kterým posílá notifikace (typicky přes metodu `notify()`) a všichni observers implementují metodu `update()`.

  **Použitie:**
  - GUI komponenty (napr. event listener).
  - MVC architektúra – Model upozorňuje View, že sa zmenil.

  **Výhody:**
  - Oddelenie logiky od zobrazenia.
  - Dynamické pridávanie/odoberanie observerov.

  **Nevýhody:**
  - Možné problémy s výkonom pri veľkom počte pozorovateľov.
</details>

6. **IS, životní cyklus informačního systému (Dohnálek)**
   * Fázy vývoja IS: plánovanie, analýza, návrh, vývoj, nasadenie, údržba.
   * Rozdiel medzi softvérom a IS.
   * Nástroje a procesy v rámci vývoja IS (CASE tools, databázy, UML).
  
7. Co je dědičnost, agregace, kompozice, asociace v UML?
8. Co je zapouzdření?
9. Co je návrhový vzor Singleton, Strategy, Observer, Factory, Composite?
10. Rozdíl mezi MVC a třívrstvou architekturou.
11. Jak se mapuje UML na kód?
12. Jak vypadá správně strukturovaná prezentační vrstva?
13. Co je model v MVC?
14. Co je aplikace a datová vrstva?


## Databázové systémy

1. **SQL Join – vnitřní a vnější** *(Bača)*\
   Vysvetlenie INNER JOIN (záznamy z oboch tabuliek, kde existuje zhoda) a OUTER JOIN (LEFT, RIGHT, FULL – doplnenie údajov aj keď nie je zhoda).
   * **Príklad:** `SELECT \* FROM A LEFT JOIN B ON A.id = B.id`
   * **Použitie:** Kombinácia údajov z viacerých tabuliek.

2. **Zotavení** *(Bača)*\
   **Obsah:** Obnovenie databázy do konzistentného stavu po páde – využitie transakčných logov, checkpointov a protokolovania.
   * **Súvislosť:** Súčasť správy transakcií a ACID vlastností.

3. **Funkční závislosti v RDB – význam a definice** *(Bača)*\
   A → B znamená, že hodnota A jednoznačne určuje hodnotu B.
   * **Použitie:** Normalizácia, detekcia redundancií, návrh schém.
   * **Príklad:** Rodné číslo → Meno, Priezvisko.

4. **SQL Select** *(Krátký)*\
   **Obsah:** Základný príkaz na výber údajov – `SELECT [sloupec] FROM [tabuľka] WHERE ...`\
   **Možnosti:** `DISTINCT`, `ORDER BY`, `GROUP BY`, `LIMIT`

5. **Rozdíl mezi výskytem fantomů a neopakovatelným čtením** *(Krátký)*
   * **Neopakované čítanie:** Pri opakovanom SELECT-e sa hodnota zmení.
   * **Fantomové záznamy:** Pri opakovanom čítaní pribudnú/zmiznú celé riadky kvôli INSERT/DELETE.
   * **Riešenie:** Vhodná úroveň izolácie (REPEATABLE READ, SERIALIZABLE).

6. **Indexy v DB** *(Krátký)*\
   **Obsah:** Štruktúry (napr. B-stromy) na zrýchlenie vyhľadávania v tabuľkách.
   * **Výhoda:** Rýchlejšie SELECT, nevýhoda: spomalenie INSERT/UPDATE.

7. **Transakce** *(Krátký)*\
   **Obsah:** Sekvencia SQL príkazov, ktorá sa vykoná ako celok (buď úplne, alebo vôbec).
   * **Súvislosť:** Zabezpečuje konzistenciu v DB.

8. **ACID**
   * **Atomicita** – buď všetko, alebo nič.
   * **Konzistencia** – systém prejde z jedného konzistentného stavu do iného.
   * **Izolácia** – transakcie sa navzájom neovplyvňujú.
   * **Trvácnosť (Durability)** – po potvrdení ostanú dáta uložené.

9. **Funkční závislosti, normální formy** *(Chovanec)*
   * Funkčné závislosti ako základ pre normalizáciu.
   * Normálne formy: 1NF (atomické dáta), 2NF (odstránenie parciálnych závislostí), 3NF (odstránenie tranzitívnych závislostí).
   * **Cieľ:** Redukcia redundancie.

10. **Procedurální SQL** *(Chovanec)*\
    Rozšírenie SQL o programovacie prvky – deklarovanie premenných, cykly, podmienky.
    * **Použitie:** Funkcie, procedúry, zložité spracovania dát.

11. **Dekompozice, konceptuální a relační datový model** *(Chovanec)*
    * Konceptuálny model: ER diagram.
    * Relačný model: tabulky, kľúče, vzťahy.
    * Dekompozícia: rozdelenie tabuliek pri normalizácii.

12. **Transakce, ACID, serializovatelnost (Fasuga)**
    * Zopakovanie ACID vlastností.
    * **Serializovateľnosť:** výstup transakcií je rovnaký ako keby bežali sekvenčne.

13. **Procedury, funkce, triggery** *(Fasugič)*
    * **Procedúry:** vykonávajú akcie, nemusia vracať hodnotu.
    * **Funkcie:** vracajú hodnotu, volateľné v SELECT-e.
    * **Triggery:** automatické reakcie na zmenu v tabuľke (INSERT/UPDATE/DELETE).

14. **Relační model, normální formy, funkční závislosti** *(Fasuga)*\
    Zhrnutie základov návrhu databáz – entita, relácia, kľúč, cudzie kľúče, normalizácia.

15. **SQL Select, Join, Left Join** *(Lukáš)*
    * Základný výber dát (SELECT).
    * `JOIN`: kombinuje riadky podľa podmienky.
    * `LEFT JOIN`: všetky riadky z ľavej tabuľky + zhody z pravej.

16. **ADO.NET přístup k databázi (nebo Java ekvivalent)** *(Lukáš)*
    * V C#: používa sa `SqlConnection`, `SqlCommand`, `SqlDataReader`.
    * V Jave: JDBC – `Connection`, `Statement`, `ResultSet`.
    * **Postup:** otvorenie spojenia, vykonanie dotazu, čítanie dát, uzavretie spojenia.

---

1. **Co je funkční závislost?** *(Bača / Chovanec / Fasuga)*
   * Definícia: A → B znamená, že každá hodnota A má presne jednu hodnotu B.
   * Dôležitá pri normalizácii.
   * Môžu sa pýtať aj na príklady zo života alebo z databázy.

2. **Jaké jsou normální formy? (1NF, 2NF, 3NF, BCNF)** *(Chovanec / Fasuga)*
   * **1NF:** Atomické hodnoty, tabuľka bez opakujúcich sa skupín.
   * **2NF:** Odstránenie parciálnych závislostí (platí len pre zložené kľúče).
   * **3NF:** Odstránenie tranzitívnych závislostí.
   * **BCNF:** Každá determinanta je kandidátny kľúč.

3. **Co je transakce a jak funguje ACID?** *(Krátký / Fasuga)*
   * **Transakcia:** Jednotka práce (sekvencia príkazov).
   * **ACID:** Atomicita, Konzistencia, Izolácia, Trvácnosť.
   * Môžu sa pýtať aj na úrovne izolácie a konflikty medzi transakciami.

4. **Rozdíl mezi inner join a outer join.** *(Bača / Lukáš)*
   * **INNER JOIN:** Len záznamy, ktoré majú zhodu v oboch tabuľkách.
   * **OUTER JOIN:** Zahrňuje aj riadky bez zhody – LEFT, RIGHT, FULL OUTER.
   * Vyžiadajú si aj príklad (tabuľku alebo SQL).

5. **Jak fungují procedury, triggery, kurzory?** *(Fasugič / Chovanec)*
   * **Procedúry:** Blok SQL kódu volaný podľa potreby.
   * **Triggery:** Automaticky spustený kód po akcii (INSERT, UPDATE…).
   * **Kurzory:** Iterácia cez množinu záznamov – kedy sa používajú, výhody/nevýhody.

6. **Co je index a jak funguje?** *(Krátký)*
   * Umožňuje rýchle vyhľadávanie záznamov.
   * Implementovaný ako B-stromy alebo hash indexy.
   * Pýtať sa môžu aj na **primárny kľúč vs. unikátny index**.

7. Rozdíl mezi relačním a konceptuálním modelem.** *(Chovanec)*
   * **Konceptuálny model:** Vyššia úroveň – ER diagram, entity, vzťahy.
   * **Relačný model:** Implementačná forma – tabuľky, stĺpce, kľúče.
   * Môžu chcieť príklad prevodu.

8. **Co je DTO a DAO?** *(možno skôr v súvislosti s ORM, bez konkrétneho učiteľa)*
   * **DTO (Data Transfer Object):** Trieda na prenos dát bez logiky.
   * **DAO (Data Access Object):** Trieda pre komunikáciu s databázou – CRUD operácie.
   * Môžu sa pýtať na **rozdiel, využitie v MVC architektúre**.

9. **Co je rollback?** *(Krátký / Fasuga)*
   * **ROLLBACK:** Vráti databázu do stavu pred začatím transakcie.
   * Môžu sa pýtať na rozdiel medzi **ROLLBACK a COMMIT**, alebo kedy k nemu dochádza (napr. chyba v transakcii).

10. **ORM: výhody, nevýhody, kdy se používá.** *(pravdepodobne Lukáš, ak ide o Java/.NET prístup)*
   * **Výhody:** Méně SQL, typová bezpečnosť, rýchly vývoj.
   * **Nevýhody:** Zložité dotazy, výkonnostné problémy.
   * Môžu sa pýtať na konkrétne ORM nástroje – Hibernate, EF Core...

11. **Korelovaný vs. nekorelovaný dotaz.** *(možno Bača alebo Krátký)*
   * **Korelovaný:** Poddotaz závisí od vonkajšieho dotazu (napr. v WHERE).
   * **Nekorelovaný:** Samostatne vykonateľný poddotaz.
   * Môžu chcieť SQL príklad s vysvetlením.

12. **Plán vykonávání dotazu.** *(bez konkrétneho mena – skôr pokročilejší dotaz)*
   * **EXPLAIN PLAN** alebo podobné nástroje – ako databáza optimalizuje vykonanie dotazu.
   * Vysvetliť, ako sa plán tvorí – na základe indexov, veľkosti tabuliek, join strategii.
   * Môžu sa pýtať na **nested loop**, **merge join**, **hash join**.


## Architektury počítačů a operační systémy

### APPS
1. **RISC procesory** *(Stříbný)*
   * Rozdiel medzi RISC a CISC (Reduced vs. Complex Instruction Set).
   * Princípy RISC architektúry: jednoduché inštrukcie, pipeline, veľa registrov, pevná dĺžka inštrukcie.
   * Výhody/nevýhody RISC architektúry.
   * Príklady RISC procesorov (ARM, MIPS).
   * Porovnanie výkonu RISC vs. CISC.
   * Typický spôsob implementácie inštrukčného cyklu (fetch-decode-execute).
2. **GPU architektura, CUDA** *(Sojka a Gajdoš)*
   * Rozdiel medzi CPU a GPU architektúrou (SIMD vs. MIMD, počet jadier, účel).
   * CUDA – čo to je, ako sa programuje.
   * Bloky, thready, grid – organizačná štruktúra CUDA.
   * Výhody paralelizácie pomocou GPU.
   * Príklady použitia CUDA v praxi.
   * Synchronizácia threadov v CUDA, shared memory.

### OSY
1. **Správa paměti** *(Stříbný a Gajdoš)*
   * Virtuálna pamäť – čo to je, ako funguje.
   * Stránkovanie, segmentácia, preklad adries.
   * Page table, TLB (Translation Lookaside Buffer).
   * Alokačné stratégie: first-fit, best-fit, buddy system.
   * Fragmentácia – interná vs. externá.

2. **Komunikace mezi procesy, paralelismus**
   * IPC mechanizmy: rúrky, message passing, shared memory, semafory.
   * Synchronizácia procesov/threadov.
   * Race conditions, deadlocks, starvenie.
   * Paralelné vs. súbežné programovanie.
   * Multithreading vs. multiprocessing.

3. **Meziprocesní komunikace** *(Seidl)*
   * Detailný pohľad na mechanizmy IPC: POSIX shared memory, named pipes, sockets.
   * Signály, wait/notify, semafory.
   * Synchronizačné problémy: producer-consumer, reader-writer, dining philosophers.

4. **Procesy** *(Seidl)*
   * Definícia procesu vs. vlákna (thread).
   * Stavový diagram procesu.
   * Životný cyklus procesu (fork, exec, wait, exit).
   * Context switching, plánovanie procesov (scheduling).
   * Priorita procesov.

5. **Klopné obvody, Paměť počítače – virtuální paměť, stránkování, přepočet adres specializovaným obvodem**
   * Základné typy klopných obvodov (SR, JK, D, T).
   * Základná logika pamätí – RAM, ROM, cache.
   * Virtuálna pamäť – hardvérová implementácia (MMU).
   * Preklad logickej adresy na fyzickú pomocou stránkovania.

6. **Souběh, kritická sekce, procesy** *(Olivka)*
   * Definícia súbehu, problémy pri súbežnom prístupe.
   * Kritická sekcia a jej ochrana (mutex, spinlock).
   * Synchronizačné primitívy.
   * Monitor, semaphore, mutex – rozdiely a použitie.
   * Príklady z reálneho OS (napr. Linux pthreads).


## Počítačové sítě a komunikační technologie
1. **IP protokol, HTTP, DNS, email** *(Radecký)*
   * **IP (IPv4, IPv6)** – adresovanie, subnetting, NAT.
   * **HTTP/HTTPS** – požiadavky/responsy, hlavičky, metódy (GET, POST...).
   * **DNS** – hierarchia, A, CNAME, MX záznamy, preklad mien.
   * **Email** – protokoly SMTP, POP3, IMAP, rozdiely, porty.
   * Príklad: ako funguje odoslanie emailu alebo otvorenie webstránky.

2. **Přepínání v počítačových sítích** *(Stříbný)*
   * Rozdiel medzi **switchom a hubom**.
   * MAC adresy, ARP protokol.
   * Switching na L2 vs. routing na L3.
   * VLAN a trunkovanie.
   * Broadcast domény vs. collision domény.

4. **IPv4 vs IPv6** *(Stříbný)*
   * Formát IP adries, veľkosť, reprezentácia.
   * Nedostatok IPv4, riešenia: NAT vs. IPv6.
   * Novinky v IPv6: autokonfigurácia, odstránenie NAT.
   * Kompatibilita, dual stack.

<details>
  <summary>Stručná odpověď</summary>
  IPv4 je štvrtej generácie internetový protokol, ktorý používa 32-bitové adresy a umožňuje približne 4,3 miliardy jedinečných IP adries. Vzhľadom na rast internetu a IoT zariadení sa tieto adresy postupne vyčerpali, preto bol vyvinutý IPv6.

  IPv6 používa 128-bitové adresy, čo znamená, že umožňuje teoreticky až 3.4×10^38 adries. Základný formát IPv6 adresy je osem skupín po štyroch hexadecimálnych čísliciach (napr. 2001:0db8:85a3:0000:0000:8a2e:0370:7334).

  Hlavné rozdiely:

  Adresovanie: IPv4 používa NAT (Network Address Translation), zatiaľ čo IPv6 počíta s verejnými adresami pre každé zariadenie.

  Konfigurácia: IPv6 podporuje autokonfiguráciu (SLAAC), nepotrebuje DHCP.

  Bezpečnosť: IPv6 má nativne zabudované IPsec.

  Efektivita: IPv6 má jednoduchšiu hlavičku paketov, čo znižuje záťaž na routery.

  Prechod z IPv4 na IPv6 je postupný a prebieha cez techniky ako dual stack alebo tunneling.
</details>

5. **Router, Switch, Směrování**
   * Úlohy jednotlivých zariadení.
   * Rozdiel medzi prepínaním (switch) a smerovaním (router).
   * Typy smerovania: statické, dynamické (RIP, OSPF, BGP).
   * Forwarding vs. Routing.

6. **Zabezpečení webu, útoky, obrana** *(Moravec)*
   * Základné útoky: **XSS, SQLi, CSRF, DDoS, spoofing, sniffing**.
   * HTTPS – certifikáty, TLS handshake.
   * Obrana: firewall, IDS/IPS, WAF.
   * Tabuľka zraniteľností: CVE, OWASP Top 10.
   * Autentifikácia, autorizácia, šifrovanie.

7. **TCP/IP, internetové protokoly** *(Seidl)*
   * Architektúra TCP/IP vs. ISO/OSI.
   * Protokoly podľa vrstiev: TCP, UDP, IP, HTTP, DNS, FTP.
   * Rozdiel medzi TCP (spoľahlivé) a UDP (rýchle).
   * TCP segmentácia, three-way handshake.

8. **Směrování a OSI model** *(Olivka)*
   * ISO/OSI vrstvy: funkcie, príklady protokolov.
   * Previazanie TCP/IP modelu na OSI (napr. IP – sieťová vrstva).
   * Smerovacie algoritmy, metriky.
   * Príklady: traceroute, ping – ako fungujú na úrovni vrstiev.


## Počítačová grafika
### URO
1. **Standardní vykreslovací řetězec** *(Sojka)*
   * GPU pipeline: vertex shader, fragment shader.
   * Rasterizácia, z-buffer.
   * Prechod dát z aplikácie do GPU.

2. **Křivky v počítačovej grafike** *(Sojka)*
   * Bezierove krivky, B-splines.
   * Parametrické rovnice.
   * Využitie v modelovaní, fontoch, animáciách.

3. **Barevné modely** *(Fusek)*
   * Aditívne (RGB), subtraktívne (CMY(K)).
   * Použitie v rôznych zariadeniach (monitory vs. tlačiarne).
   * Farby v HTML/CSS, volba farebných paliet.

<details>
  <summary>Stručná odpověď</summary>
  Farebné modely slúžia na reprezentáciu farieb v počítači.

  Aditívne modely (napr. RGB – red, green, blue) miešajú farby pridaním svetla. Používajú sa v zariadeniach, ktoré svetlo vyžarujú – napr. monitory. Kombináciou všetkých troch farieb v maximálnej intenzite dostaneme bielu.

  Substraktívne modely (napr. CMYK – cyan, magenta, yellow, key/black) miešajú farby odčítaním svetla. Používajú sa v tlačiarňach. Kombináciou všetkých troch farieb dostaneme čiernu (v praxi tmavosivú, preto sa pridáva K – čierna).

  Farebné modely sú základom farebného zobrazenia aj konverzií medzi rôznymi médiami.
</details>

### ZPG
1. **Matice a maticové operace**
   * Matice transformácií: translácia, rotácia, mierka.
   * Zloženie transformácií – násobenie matíc.
   * Homogénne súradnice.

2. **Vykreslovací řetězec** *(Němec)*
   * Priebeh spracovania 3D scény – od modelu po obrazovku.
   * Pipeline fázy – vertex shading, clipping, projection.
   * Osvetľovanie, tieňovanie.

3. **Phongův osvětlovací model** *(Němec)*
   * Komponenty: ambient, diffuse, specular.
   * Normálové vektory, výpočet intenzity svetla.
   * Použitie vo fragment shadery.

4. **Transformace a projekce** *(Němec)*
   * Typy projekcie: ortogonálna, perspektívna.
   * Matice projekcie.
   * Zobrazenie 3D objektu na 2D obrazovku.


# Teoretické základy informatiky
## Algoritmy

### ALG
1. **Binární vyhledávací strom** *(Dohnálek)*
   * Vloženie, hľadanie, zmazanie.
   * Složitosti operácií – priemer vs. najhorší prípad.
   * Vlastnosti BST, AVL, red-black strom.
   * Rekurzívna a iteratívna implementácia.

2. **Strategie algoritmizace – hrubá síla, bubble sort** *(Dohnálek, Sojka)*
   * Hrubá síla (brute force) – vyčerpávajúce prehľadávanie, vhodné použitie.
   * Bubble sort – pseudokód, analýza časovej zložitosti.
   * Porovnanie s efektívnejšími algoritmami.
   * Diskusia, prečo môže byť O(n²) niekedy vhodné.

3. **Grafy, cesty, průchody** *(Kudělka, Dvorský)*
   * BFS, DFS – ako fungujú, pseudokód.
   * Sled, cesta, cyklus, komponenty súvislosti.
   * Zameranie na orientované/neorientované grafy.
   * Možné aplikácie (napr. najkratšia cesta).

4. **Třídící algoritmy, složitosti** *(Kudělka, Dvorský)*
   * Vyjmenovať algoritmy: bubble, insertion, merge, quicksort, heapsort, radix.
   * Pre každý z nich vedieť: časová zložitosť, stabilita, vhodnosť použitia.
   * Pseudokód – aspoň pre 1–2 z nich.

5. **Matematicky dokázat složitost algoritmu** *(Dohnálek)*
   * Rekurzívne rovnice (napr. T(n) = 2T(n/2) + n).
   * Výpočet cez Master Theorem, indukciu.
   * Porovnanie lineárneho a rekurzívneho algoritmu.

6. **Rozděl a panuj, Quicksort** *(Dohnálek, Sojka)*
   * Vysvetlenie princípu.
   * Najlepší, priemerný a najhorší prípad.
   * Pseudokód, výhody/nevýhody oproti iným sortom.

<details>
  <summary>Stručná odpověď</summary>
  Odpoveď:
  Rozdel a panuj je stratégia, ktorá rozdeľuje problém na menšie podproblémy, rieši ich rekurzívne a riešenia kombinuje.

  Quicksort funguje tak, že:

  Vyberie pivot (napr. náhodný prvok).

  Rozdelí pole na menšie/rovné/väčšie ako pivot.

  Rekurzívne zoradí obe časti.

  Zložitosti:

  Najlepší a priemerný prípad: O(n log n)

  Najhorší prípad (ak je pole už zoradené a pivot je krajné číslo): O(n²)

  Výhoda: veľmi rýchly v praxi a nevyžaduje veľa pamäte (in-place).
  Nevýhoda: nestabilný a citlivý na výber pivotu.
</details>

7. **Asymptotická složitost** *(Běhálek)*
   * O-veličiny: O, Ω, Θ.
   * Porovnanie algoritmov podľa zložitosti.
   * Typické funkcie: log n, n, n log n, n²...

8. **Hash table, binární strom, mapy** *(Janoušek, Vašínek)*
   * Ako funguje hash table: hash funkcia, kolízie (chaining, open addressing).
   * Složitosti operácií: priemer vs. najhorší prípad.
   * Mapy ako abstrakcia (napr. v STL: `std::map`, `std::unordered_map`).

9. **Strategie řešení algoritmických problémů** *(Běhálek, Kot)*
   * Backtracking, greedy, divide-and-conquer, dynamic programming.
   * Príklady použitia na klasických problémoch (napr. batoh, grafy, triedenie).
   * Rozpoznať, kedy sa ktorá stratégia hodí.

10. **Teorie grafů (definice)**
    * Orientované vs. neorientované, súvislosť, mosty, klika.
    * Stromy, kostry, acyklickosť.
    * Základné pojmy a ich vzťahy.

11. **Složitost algoritmů**
    * Teoretické porovnanie – triedenie, vyhľadávanie, grafy.
    * Význam asymptotickej analýzy.
    * Praktický dopad na výber algoritmu.

12. **Transformuj a panuj – Gaussova eliminace** *(Dvorský)*
    * Riešenie lineárnych rovníc.
    * Matematický postup + zložitosť.
    * Možné numerické problémy.

13. **Hladové algoritmy, kostra grafu** *(Dvorský)*
    * Greedy princíp – vždy najlepší lokálny krok.
    * Príklad: Kruskal, Prim – kostra grafu.
    * Výhody/nevýhody greedy prístupu.

14. **Sekvenční, binární vyhledávání**
    * Pseudokód oboch, časová zložitosť.
    * Kedy sa ktorý hodí – predpoklad zoradenia.

15. **Základní lineární datové struktury** *(Kudělka)*
    * Seznam (linked list), zásobník (stack), fronta (queue).
    * Operácie: vloženie, výmaz, vyhľadanie.
    * Implementácia: pole vs. ukazatele.

### ZSU
1. **Clustering, K-means, hierarchické** *(Janoušek, Vašinek)*
   * Algoritmus k-means – inicializácia, iterácie.
   * Hierarchické – aglomeratívne vs. divizívne.
   * Preprocessing – normalizácia, PCA.

2. **Strojové učení – základy** *(Gajdoš, Ochodková, Fusek)*
   * Rozdelenie: supervised, unsupervised, reinforcement learning.
   * Príklady algoritmov.
   * Datasety, overovanie, tréning vs. test.

3. **Klasifikace vs. Clustering** *(Fusek, Kudělka)*
   * Rozdiel – prítomnosť výstupných tried.
   * Klasifikačné algoritmy: SVM, Decision Tree, Naive Bayes.
   * Metriky: accuracy, precision, recall.

<details>
  <summary>Stručná odpověď</summary>
  Odpoveď:
  Klasifikácia a clustering sú dve základné úlohy v strojovom učení.

  Klasifikácia je supervised learning – model sa učí z označených dát, cieľom je predpovedať príslušnosť k triede.

  Príklad: Rozpoznávanie spamu.

  Algoritmy: Decision Trees, SVM, k-NN, Naive Bayes.

  Clustering je unsupervised learning – dáta nemajú priradené triedy, cieľom je nájsť vnútornú štruktúru.

  Príklad: Segmentácia zákazníkov.

  Algoritmy: K-means, DBSCAN, hierarchické zhlukovanie.

  Rozdiel: klasifikácia vyžaduje učebné dáta s odpoveďami, clustering 
</details>

4. **Datová analýza, korelace, kovariance** *(Kudělka)*
   * Vzťahy medzi atribútmi – Pearson, Spearman.
   * Korelácia vs. kauzalita.
   * Význam pre výber vstupov do modelov.

## Teoretická informatika

### ULM
1. **Množiny, relace, funkce** *(Menšík, Kot, Gaura)*
   * Operácie na množinách: zjednotenie, prienik, rozdiel.
   * Relácie: vlastnosti – reflexivita, symetria, tranzitivita.
   * Funkcie – zobrazenie, injektivita, surjektivita.

2. **Výroková a predikátová logika** *(Dráždilová, Gajdoš, Sawa)*
   * Syntax vs. sémantika formulí.
   * Pravdivostné tabuľky, rezolučná metóda.
   * Kvantifikátory, logické dôsledky.

3. **Grafy a stromy** *(Ochodková)*
   * Koreň, list, hĺbka stromu.
   * Binárny strom, binárne vyhľadávanie.
   * Použitie stromov v logike (napr. syntaktické stromy).

### UTI
1. **Automaty a regulárne jazyky** *(Bača, Dráždilová, Sawa, Menšík)*
   * DFA vs. NFA – ekvivalencia.
   * Regulárne výrazy, ich jazyk.
   * Uzavrenosť triedy regulárnych jazykov.

2. **Chomského hierarchie, bezkontextové gramatiky** *(Běhálek)*
   * Typy jazykov: regulárny, bezkontextový, kontextový, rekurzívne spočítateľný.
   * LL(1) gramatiky – význam pre prekladače.

3. **Správa paměti, chomp chomp, uzavrenosť** *(Stříbný, Dráždilová)*
   * Uzavrenosť regulárnych jazykov (zjednotenie, prienik).
   * Chomsky games (chomp chomp) – demonštrácia vlastností jazykov.

### PJP
1. **Překladače – úvod** *(Gaura, Běhálek)*
   * Rozdelenie do fáz: lexikálna, syntaktická, sémantická, generovanie kódu.
   * Rôzne typy prekladačov: interpret, kompilátor.

2. **Konečné automaty, regulární výrazy** *(Sawa, Dráždilová)*
   * DFA, NFA, transformácie, použitie pri lexikálnej analýze.
   * Regular expressions – syntax, použitie.

3. **Typy a průběh překladu, syntaktická analýza** *(Kot, Sawa)*
   * LL, LR gramatiky.
   * Parsovanie: top-down vs. bottom-up.
   * Význam AST (Abstract Syntax Tree).

<details>
  <summary>Stručná odpověď</summary>
  Syntaktická analýza (parsovanie) je fáza prekladu, ktorá overuje gramatickú správnosť kódu podľa formálnej gramatiky.

  Typy parserov:

  Top-down (LL): číta zľava, vytvára strom zhora.

  Bottom-up (LR): zhlukuje tokeny do vyšších konštrukcií, tvorí strom zdola.

  Výsledkom je syntaktický strom alebo abstraktný syntaktický strom (AST), ktorý sa následne využíva v sémantickej analýze.

  Parsery možno generovať automaticky zo špecifikácie gramatiky pomocou nástrojov ako Yacc alebo ANTLR.
</details>


## Matematika pro informatiku

### MA
1. **Derivace, integrály, význam** *(Dvorský)*
   * Derivácia jednej premennej – geometrický a fyzikálny význam.
   * Neurčitý vs. určitý integrál – výpočty, vzorce.
   * Rovnomerný pohyb – derivácia a integrál rýchlosti/akcelerácie.

### LA

1. **Matice, inverze, operace** *(Gaura, Sojka)*
   * Sčítanie, násobenie, inverzia matice.
   * Determinant – kedy existuje inverzná matica.
   * Časová zložitosť výpočtov.

<details>
<summary>Stručná odpověď</summary>
Inverzná matica $A^{-1}$ k matici $A$ je taká, že platí: $A \cdot A^{-1} = I$, kde $I$ je jednotková matica.

Podmienky existencie:
- $A$ musí byť štvorcová.

Determinant ≠ 0.

Výpočet: Gauss-Jordanova eliminácia.

$A$ sa rozšíri o jednotkovú maticu a aplikuje sa transformácia do tvaru (I | A⁻¹).

Použitie: Riešenie sústavy rovníc $A * x = b$ pomocou $x = A^{-1} * b$.

Výpočty v grafike a kryptografii.
</details>

2. **Lineární soustava rovnic** *(Němec)*
   * Riešenie: Cramer, substitúcia, Gaussova eliminácia.
   * Počet riešení – jednoznačné, nekonečné, žiadne.

3. **Vektorové prostory, lineární zobrazení**
   * Bázové vektory, dimenzia.
   * Lineárne zobrazenia a ich matice.
   * Spektrálna teória – vlastné čísla, vlastné vektory.

### DIM
1. **Grafy – definice, využití** *(Dohnálek)*
   * Vrchol, hrana, multigraf, orientovaný/neorientovaný.
   * Modelovanie problémov grafmi – sociálne siete, mapy.
   * Matematická definícia grafu.

<details>
  <summary>Stručná odpověď</summary>
  Graf je množina vrcholov a hrán. Formálne: $G = (V, E)$, kde $V$ je množina vrcholov a $E$ množina hrán (dvojíc vrcholov).

  Typy grafov:
  - Orientované / Neorientované.
  - Slučky, viacnásobné hrany (multigraf).
  - Cyklické / Acyklické.

  Využitie:
  - Cestovanie a mapy (navigácia).
  - Sociálne siete (vrcholy = ľudia, hrany = spojenia).
  - Počítačové siete, databázy (ER diagramy).

  Základné pojmy: stupeň vrcholu, cesta, cyklus, komponent súvislosti.
</details>

2. **Kongruentní rovnice** *(Kudělka)*
   * Definícia, vlastnosti, príklady riešení.
   * Modulárna aritmetika – využitie v kryptografii.
