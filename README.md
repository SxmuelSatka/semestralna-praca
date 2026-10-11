# MoneyTracker

Samuel Šatka

5ZYI34

## Stručný opis projektu
MoneyTracker je webová aplikácia určtená na správu osobných financié. Ponúka používateľom jednoducho sledovať svoje príjmy, výdaje a finančný stav
Používateľ si bude môcť zaznamenávať jednotlivé transakcie, rozdelovať ich do kategórií (napr. podľa dôležitosti), a tvoriť si ciele.
Hlavným cieľom aplikácie je hlavne pomôcť a zjednodušeniť manažovanie financií.

## Role v projekte
 - Návštevník - bude mať prístup iba na úvodnu stránku aplikácie, bude sa môcť prihlásiť alebo zaregistrovať.

 - Registrovaný/prihlásený užívateľ - Bude mať prístup ku všetkým hlavným funkciam aplikácie, bude môcť upravovať svoje príjmy, výdaje, ciele.

 - Administrátor - Bude mať práva na spravovanie a základnu administráciu aplikácie a užívateľov, bude vedieť účty mazať, recoverovať.

## Prípady použitia podľa rolí
 - Návštevník - Zobrazí si zobrazí základnu stránku aplikácie
           - Vytvorí si účet v aplikácií
           - Prihlási sa na už vytvorený účet v aplikácií

 - Registrovaný používateľ - Prihlási / odhlási sa zo svojho účtu
                        - Zobrazí si prehľad financií, výdajov a cieľov
                        - Pridá si nový cieľ, príjem, výdaj
                        - Odstráni si cieľ, príjem, výdaj
                        - Vie si vyfiltrovať ciele, príjmy, výdaje podľa dátumu, sumy atď...

 - Administrátor - Prihlási/odhlási sa do administratívneho konta
              - Zobrazí zoznam používateľov
              - Deaktivuje/zmaže/pridá používateľa
              - Zobrazí základné štatistiky o aplikácií

## Plánované entity
 - Používateľ - registrovaný používateľ aplikácie<br>
Atribúty - id, username, pass, is_active

- Transkacia - predstavuje jednotlivý finančný príjem/výdaj používateľa<br>
Atribúty - id, user_id, category_id, amount, type, date

 - Kategória - predstavuje rozdelenie transkacií do jednotlivých skupín<br>
Atribúty - id, user_id, name, type , color
 - Rozpočty - predstavuje finančný ciel/limit, ktorý si používateľ nastaví<br>
Atribúty - id, user_id, category_id, amount, month, year

## Vzťahy medzi entitami
 - Používateľ - Transkacia (1:N) <br>
 - Používateľ - Kategória (1:N) <br>
 - Kategória  - Transkacia (1:N) <br>
 - Používateľ - Rozpočet (1:N) <br>
 - Kategória - Rozpočet (1:N) <br>

## Hlavné stránky aplikácie
 - Úvodná stránka - bude obsahovať základné informácie o aplikácií, a jej funkciách <br>
 - Prihlásenie a registrácia - umožní vytvorenie a prihlásenie používateľského účtu, pomocou emailu<br>
 - Dashboard - Prehľad informácií, príjmov a výdajov<br>
 - Správa transkacií - Slúži na pridávanie a odstraňovanie transkacií<br>
 - Správa kategórií - Slúži na pridávanie a odstraňovanie kategórií <br>
 - Mesačné rozpočťy - Umožňuje používateľovi pridávať limity, ciele pre jednotlivé kategórie
 - Štatistiky - Bude zobrazovať štatistiky používateľa
 - Profil používateľa - Zobrazí profil používateľa
 - Administrácia - Bude dostupná len pre administrátora, bude obsahovať zoznamy, a možnosť spravovať účťy

## Rozdelenie funkcionality
### Základne funkcie

- Registrácia, prihlásenie, odhlásenie používateľa
- Rozdelenie typov používateľov
- Autorizácia a prístupy podľa typu používateľa
- Pridávanie, odstraňovanie a zobrazovanie transakcií/kategórií/rozpočtov
- Responzívny dizajn aplikácie

### Rozširujúce funkcie

- Grafické zobrazenie štatistík
- Porovnávanie výdajov medzi rôznymi mesiacmi
- Export do CSV súborov
- Light/dark mode
- Pravideľné pridávanie výdajov na základe nejakého predplatného
- pridanie rôznych mien (czk, doláre...)
 
 

