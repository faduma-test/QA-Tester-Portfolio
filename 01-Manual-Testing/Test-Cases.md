SauceDemo – Manuel QA-testdokumentation
Projekttype: Øvelsesprojekt
Testtype: Manuel funktionel test
Testet hjemmeside: https://www.saucedemo.com/
1. Projektoversigt
Dette projekt dokumenterer manuel funktionel test af webshoppen SauceDemo.

Testede områder:

Loginfunktion
Produktkatalog
Indkøbskurv
Checkout og gennemførelse af køb
Produktsortering
Testbrugere:

standard_user – Normal bruger
problem_user – Bruger til test af fejlscenarier
Formål: At kontrollere hjemmesidens funktioner, sammenligne forventede og faktiske resultater, finde fejl og dokumentere testresultaterne.

2. Samlet testresultat
Testresultat	Antal
Samlet antal test cases	10
Bestået (Passed)	7
Fejlet (Failed)	3
Fundne fejl (Bugs)	3
3. Gennemførte test cases
TC-01 – Login
Testtrin: Åbn SauceDemo, indtast standard_user og secret_sauce, og klik på Login.
Forventet resultat: Brugeren logges ind og kommer til produktsiden.
FaktiTesttrin: Log ind som standard_user, find Sauce Labs Backpack, og kontrollér navn, beskrivelse og pris.
Forventet resultat: Korrekt produktnavn, beskrivelse og pris på $29.99 vises.
Faktisk resultat: Produktnavn, beskrivelse og pris blev vist korrekt.
Status: BESTÅET
TC-03 – Læg vare i indkøbskurven
Testtrin: Log ind som standard_user, find Sauce Labs Backpack, og klik på Add to cart.
Forventet resultat: Knappen ændres til Remove, og indkøbskurven viser 1.
Faktisk resultat: Knappen ændrede sig til Remove, og indkøbskurven viste 1.
Status: BESTÅET
TC-04 – Se indkøbskurv
sk resultat: Produktsiden blev vist uden problemer.
Testtrin: Tilføj Sauce Labs Backpack, og klik på indkøbskurvens ikon.
Forventet resultat: Indkøbskurven viser rygsækken, antal 1 og prisen $29.99.
Faktisk resultat: Varen, antal og pris blev vist korrekt.
Status: BESTÅET
TC-05 – Start checkout
Testtrin: Åbn indkøbskurven, og klik på Checkout.
Forventet resultat: Siden Your Information åbner med tre indtastningsfelter.
Faktisk resultat: Checkout-formularen åbnede med tre felter.
Status: BESTÅET
TC-06 – Checkout-overblik
Testtrin: Indtast fornavn, efternavn og postnummer. Klik på Continue.
Forventet resultat: Ordreoversigten viser varen, moms og en samlet pris på $32.39.
Faktisk resultat: Ordreoversigten viste ordren og totalprisen $32.39.
Status: BESTÅET
TC-07 – Gennemfør køb
Testtrin: Klik på Finish på ordreoversigten.
Forventet resultat: En ordrebekræftelse vises.
Faktisk resultat: Beskeden "Thank you for your order!" blev vist.
Status: BESTÅET
TC-08 – Produktbilleder
Testbruger: problem_user
Testtrin: Log ind som problem_user, åbn produktkataloget, og kontrollér produktbillederne.
Forventet resultat: Hvert produkt viser det korrekte produktbillede.
Faktisk resultat: Alle produkter viste et billede af en hund.
Status: FEJLET
Fejlrapport: BUG-01
TC-09 – Læg Fleece Jacket i indkøbskurven
Testbruger: problem_user
Testtrin: Log ind som problem_user, åbn Sauce Labs Fleece Jacket, og klik på Add to cart.
Forventet resultat: Knappen ændres til Remove, og indkøbskurven opdateres til 1.
Faktisk resultat: Knappen reagerede ikke på klik, og varen blev ikke lagt i kurven.
Status: FEJLET
Fejlrapport: BUG-02
TC-10 – Sortering af produkter efter pris
Testbruger: problem_user
Testtrin: Log ind som problem_user, åbn sorteringsmenuen, og vælg Price (low to high).
Forventet resultat: Produkterne sorteres fra laveste til højeste pris.
Faktisk resultat: Produkternes rækkefølge ændrede sig ikke.
Status: FEJLET
Fejlrapport: BUG-03
4. Konklusion
Der blev gennemført 10 manuelle test cases på SauceDemo.

7 test cases blev bestået med standard_user.
3 test cases fejlede med problem_user.
3 fejl blev identificeret og dokumenteret i separate fejlrapporter.
Te5. Screenshots og dokumentation
Følgende screenshots bruges som dokumentation for de identificerede fejl:

BUG-01: Screenshot af produktoversigten med forkerte produktbilleder (hund).
BUG-02: Screenshot, der viser, at Add to cart-knappen ikke reagerer ved Sauce Labs Fleece Jacket.
BUG-03: Screenshot, der viser, at produkternes rækkefølge er uændret efter valg af Price (low to high).stene dækkede centrale funktioner på webshoppen, herunder login, produktvisning, indkøbskurv, checkout og produktsortering.


Status: BESTÅET
TC-02 – Produktkatalog
