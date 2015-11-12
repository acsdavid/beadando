# Dokumentáció

## Követelményanalízis

#### 1. Követelmények:
Az ügyfél szeretne egy olyan weboldalt, melyen online vezetheti a kiadásait és bevételeit. A weboldalon jelenjelen meg egy alkalmazás, mely egységesen a kiadás és bevétel táblázat formájában.
- A weboldalon megtalálható alkalmazással szemben támasztott funkcionális követelmények a kiadások és bevételek egy közös táblában való megjelenítése. Csak a bejelentkezett felhasználók számára legyen elérhető weboldalon lévő alkalmazás
- A weboldalnak legyen szép dinamikus felülete

```
Fejlesztési módszertan:
    Egységesített Eljárás
A fejlesztéshez szükséges hardver:
    CPU: Pentium 4, RAM: 512 GB, videó: 1024x768
A fejlesztéshez használt szoftverek:
    Operációs rendszer: Windows 7.
    Követelmény elemzés: Github szövegszerkesztővel
    Fejlesztőeszköz: Node.js
A futtatáshoz szükséges operációs rendszer:
    Tetszőleges operációs rendszer, melyhez létezik JRE 6 implementáció
A futtatáshoz szükséges hardver:
    Windows, Linux, Cloud9
Egyéb követelmények:
    Design-os felhasználói felület, könnyű kezelhetőség
```
    
#### 2. Szakterületi fogalomjegyzék:
* Statikus és dinamikus weboldal: A statikus oldalt egy plakátra tudnám hasonlítani. Az van, amit látunk, ahhoz         hozzátenni nem tudunk, eszi nem eszi, nem kap mást. Míg a dinamikus weboldalaknál a tartalom mindig dinamikusan generálódik. Dinamikus, mert képlékeny, alakítható.
* Webalkalmazás: Az alkalmazásszerver egy szoftver keretrendszer, amely olyan környezetet biztosít, amelyben tetszőleges alkalmazások futhatnak, függetlenül attól, hogy mit is csinálnak. Fő feladata eljárások hatékony végrehajtása (programok, rutinok, szkriptek) és nagyobb alkalmazások készítésének támogatása.

#### 3. Használatieset-modell:
1. Szerepkörök: 
Az oldalon két szerepkörű felhasználó van. A felhasználó és a vendég. Vendég nem lát mást csak a bejelentkezési felületet és a főoldalt. A felhasználó már korábban regisztrált, ezért ő eléri az oldal összes funkcióját.
2. A weboldalon lévő fő alkalmazásfunkciót, azaz a pénztárcát csak a bejelentkezett felhasználók érhessék el. Lehetőség legyen bárkinek regisztrálni. A regisztrálást követően azonnali bejelentkezés legyen elérhető. A táblát, mely a felhasználók tételeit tartalmazza, legyen lehetőség azok módosítására, vagy törlésére.
    KÉÉÉP
3.A felhasználó a weboldal betöltését követően a főoldalra kerül. A nem bejelentkezett felhasználók nem érik el a weboldalon lévő alkalmazást, emiatt bejelentkezés szükséges. Ha nem rendelkezik a felhasználó fiókkal, regisztráción megjelenő mezők kitöltésével megteheti. Regisztrálást követően azonnal lehetőség nyílik bejelentkezni. Bejelentkezést követően elérhetővé válik a Kiadások listája, melyen látható táblázat formályában a felhasználók kiadási vagy éppen a bevételei. Lehetőség van új tétel felvételére, mely a tábla legaljára kerül rögzítésre.

#### 4. Tervezés
    1. Architektúra terv:
    A bejelentkezési adatok szerveoldalon történnek eltárolásra, így amikor a felhasználó bejelentkezni készül, az oldal az adatbázisból lekéri a szükséges adatokat, megnézi helyességét, majd helyesség alapján dönt.
    Végpontok listája:
    /login
    /login/signup
    /errors/list
    /errors/new
    /errors/update/{id}
    /errors/delete/{id}
    2. Felhasználóifelület-modell
leírását tartalmazza. A megrendelő számára is érthető termék, mely segíti a megrendelő és a
fejlesztő közti kommunikációt. A használati eseteket a teljes fejlesztési folyamat során
figyelembe kell venni.

## Tervezés

fs
df
sd
asdas

## Implementáció
    1.asda  
    2.  asfasf
    3.asfasfa
sadasda
   asdas
   asdas
asdasd
## Tesztelés
## Felhasználói dokumentáció
