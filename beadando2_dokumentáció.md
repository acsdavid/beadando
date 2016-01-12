-----

####ELTE IK - Ács Dávid - GWOZ03 - Alkalmazások fejlesztése - 2. beadandó

-----

##Dokumentáció - ["2.beadandó - NEPTUM"](https://github.com/horvathgyozo/alkfejl_minta)

###Követelmények

####Funkcionális követelmények

Az oldal egy webes vastagkliens, azaz egyoldalas alkalmazás `Ember.js`. Feladatot illetően lehet a szerveroldali alkalmazásnak egy kliensoldali változata, de másik feladat is választható.

A feladatnak mininálisan tartalmaznia kell:

- legalább két modellt, egy-sok kapcsolatban
- legalább 1 űrlapot
- legalább 1 listázó oldalt
- legyen lehetőség új felvételére
- legyen lehetőség meglévő szerkesztésére
- legyen lehetőség meglévő törlésére
- `REST API` végpont kialakítása
- szerveroldali perzisztálás fájlba

####Nem funkcionális követelmények

Az oldalnak a kezelése egyszerűnek, letisztultnak és könnyen elsajátíthatónak kell lennie.

-----

###Fogalomjegyzék

- `subject` - A tantárgy adatait tároló objektum
  - `name` -  A tantárgy neve, string
  - `size` - A tantárgy férőhelyeinek száma, int
  - `location` - A tantárgy helyszíne, string
  - `teacher` - A tantárgy előadója, string

- `user` - Felhasználó
  - `neptun` - A felhasználó Neptun kódja
  - `password` - A felhasználó jelszava
  - `surname` - A felhasználó vezetékneve
  - `forename` - A felhasználó keresztneve
  - `email` - A felhasználó e-mail címe
 
- `list` - A tantárgyak listája
- `new` - Új tantárgy felvétele - űrlap
- `update` - Egy már létező tantárgy módosítása - űrlap
- `delete` - Egy már létező tantárgy törlése

-----

###Használatieset-modell

- Használatieset-diagram 

![Usecase](http://imgur.com/5dJ0PSd "")
-----

###Tervezés

####1. Architektúra terv

 - Oldaltérkép
   - Főoldal
   - Regisztráció
   - Vizsgák oldal
   - Vizsga felvétele oldal
   - Rólunk
 - Végpontok
   - `/` - Főoldal
   - `/registration` - Regisztráció
   - `subjects/list` - Vizsgák oldal
   - `subjects/new` - Vizsga felvétele oldal
   - `/about` - Rólunk       
        
####2. Felhasználói felület

   Főoldal 
   
   ![Index](http://imgur.com/VXMNw45 "")

   Vizsgák oldal 
   
   ![SubjList](http://imgur.com/Xtw2SYD "")

   Vizsga felvétele oldal 
   
   ![NewSubj](http://imgur.com/EQiWyPV "")
   
   Rólunk
   
   ![About](http://imgur.com/14Cn4xi "")

####3. Osztálymodell

- Osztálymodell 

![Classdia](http://imgur.com/NLpbe0O "")

####4. Dinamikus működés

![Dynamic](http://imgur.com/NLpbe0O "")

-----

###Implementáció

####Fejlesztői környezet

  A fejlesztésnél felhasznált technológiák:
  
  - `Cloud9 Web IDE` - [https://c9.io/](https://c9.io/)
  - `Ember.js` - [http://emberjs.com/](http://emberjs.com/)
  - `Bower` - [http://bower.io](www.bower.io)
  - `Bootstrap` - [http://getbootstrap.com](http://getbootstrap.com/)
  
  A projectben használt modulok:

  - `broccoli-asset`
  - `ember-cli`
  - `ember-data`
  - `bower`

####Forráskód

  A project forráskódja megtalálható a következő [GitHub](http://github.com)-os oldalon: [github.com/acsdavid/ember](https://github.com/acsdavid/ember)

-----

###Felhasználói dokumentáció

####Rendszerkövetelmény

- Aktív internetkapcsolat
- Grafikus felületet kezelő operációsrendszer
- 64MB RAM
- Mozilla, Safari, Chrome

####Futtatás

Az alkalmazás megfelelő futásához szükséges először az alkalmazás REST API részét elindítani, mely itt található: [rest_server](https://ide.c9.io/acsdavid/rest_server)

Az API indításához a `server.js` filet kell futtatni a `Run` opcióval. Amennyiben a szerver sikeresen fut, láthatóvá válik a `console`-on.

Ezután már elindíthatjuk a klienst is, mely ezen a címen érhető el: [acsdav](https://ide.c9.io/acsdavid/ember)

Lépjünk be a project mappájába: `cd targyfelvetel/`, majd a kliens az `ember serve` paranccsal futtatható.

Ha mindent jól csináltunk, akkor a [localhost:8080](http://http://ember-acsdavid.c9users.io:8080/) címen elérhető, a REST API-ból jövő adatokkal.
