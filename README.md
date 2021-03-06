
Training360 - Angular Záróvizsga Feladatok Az alábbi dokumentum a záróvizsga gyakorlati feladatait tartalmazza, frontend szakirány esetén. Bevezetés A feladatokat egy már előre elkészített környezetben kell megoldani. Ez az alkalmazás felhasználók adatait kezeli. A felhasználók listázását, és a hozzá kapcsolódó osztályokat és szolgáltatásokat készen tartalmazza az alap-alkalmazás. A feladat hat darab jól elkülönülő funkció elkészítése az alap-alkalmazásra épülően. Beadás A kész feladatot 2021-03-16 23:00 -ig kell beadni ezen az űrlapon. Itt fel kell tüntetni a személyes adatokat és a feladat elérhetőségét is. Csak a határidőig beérkező feladatokat tudjuk értékelni. Űrlap linkje: https://forms.office.com/r/WE3vWyryZM Feltételek A feladatok elvégzéséhez az alábbi feltételek és programok megléte szükséges: 
1.  PC stabil internet kapcsolattal. 
2.  Legalább 8GB RAM. 
3.  Legalább 2 magos CPU. 
4.  Telepített Git kliens. 
5.  Telepített Visual Studio Code alkalmazás. 
6.  Telepített NodeJS futtatókörnyezet, NPM csomagkezelővel. 
Kezdő lépések 
1.  Telepítsd a prog-teacher csomagot a parancssorban: `npm i -g prog-teacher` 
2.  Töltsd le a alap-alkalmazást: `prog-teacher str-final-exam` 
3.  Hozz létre egy Github repozitorit a saját fiókodban, a neve legyen: `str-final-exam` 
4.  Lépj be a mappába: `cd str-final-exam` 
5.  Állítsd be a VSCode gyökerének az aktuális mappát: `code . -r` 
6.  Telepítsd a függőségeket: `npm i` 
7.  Állítsd be a Github repozitorid távoli forrásnak:  `git init` `git add .` `git commit -m "first commit"` `git branch -M main` `git remote add origin https://github.com/<username>/str-final-exam.git` 
`git push -u origin main` Figyelem: a username helyére a te github fiókod neve kerül. 
8.  Indítsd el a json-server -t és az Anagular dev-server -t:  `json-server .\server\db.json --watch` `npm start` 
Feladatok

1.  A megjelenő táblázatban készítsd el a törlés funkcionalitást! 
A törlés gombra kattintva a példa adatbázisból törlődjön az adott rekord. 
Törlés előtt jelenjen meg egy megerősítő kérdés. 
A törléshez a UserService osztályban is hozd létre a szükséges metódust.
 
2.  Tedd szűrhetővé a táblázatban megjelenő adatokat! 
A táblázat felett hozz létre egy beviteli mezőt. 
A beviteli mező értékének módosítása esetén a táblázat azon rekordjai maradjanak láthatóak, amelyek `name` mezője részben vagy egészben tartalmazza a beviteli mezőbe gépelt szöveget. 

3.  Tedd rendezhetővé a táblázatban megjelenő adatokat! Ha a felhasználó a táblázat fejléceire kattint, akkor a megjelenő rekordok rendeződjenek az adott oszlop szerint növekvő sorrendbe. Ha egy másik oszlop fejlécére kattint, akkor pedig a szerint az oszlop szerint, amelyre utoljára kattintottak. Csak növekvő sorrendbe kell rendezni. 
4.  Tedd módosíthatóvá a táblázatban megjelenő rekordokat! A táblázat sorainak utolsó cellájában lévő szerkesztés gombra kattintva jelenleg megjelenik a szerkesztő oldal. Az oldalon már létre vannak hozva a beviteli mezők. Ha a mentés gombra kattint a felhasználó, akkor az adatbázisban kerüljenek frissítésre az adott rekord adatai. A módosításhoz a UserService osztályban is hozd létre a szükséges metódust. 
5.  Validáld az adatokat a szerkesztő űrlapon! Minden input elem előtt kommentben feltüntettük a validálás szabályait. Attribútumok és reguláris kifejezések használatával validáld a mezőkbe írt adatokat. Ha nem megfelelő az adat, akkor jelenjen meg releváns hibaüzenet közvetlenül a hibás adatot tartalmazó mező alatt. Ha az űrlap bármely mezője hibás adatot tartalmaz, a mentés gomb legyen letiltva és ne legyen az űrlap elküldhető. Sikeres módosítás után navigáljon vissza az alkalmazás a táblázathoz.
6.  Tedd lehetővé új rekord rögzítését. Hozz létre egy teljes szélességű gombot a lista oldalon a táblázat felett, amelyre kattintva szintén a szerkesztő űrlap jelenik meg, de üres állapotban. Az adatbevitel során ugyanazok a validációs szabályok legyenek érvényesek, mint a szerkesztés esetén. Megfelelő kitöltés után a mentés gombra kattintva történjen meg az új rekord beszúrása az adatbázisba és navigáljon vissza az oldal a táblázathoz. A beszúráshoz a UserService osztályban is hozd létre a szükséges metódusokat. 
