# Arab–római számkonverter – TDD

## A projekt bemutatása

A projekt célja egy JavaScript nyelven megvalósított arab–római számkonverter elkészítése a Test Driven Development (TDD) módszertan alkalmazásával.

A program az 1 és 3999 közötti egész számokat alakítja át római számokká, a hagyományos római számírás szabályai szerint.

## Alkalmazott technológiák

- **JavaScript:** a számkonverter megvalósítása.
- **HTML:** a program és a tesztkörnyezet futtatása.
- **QUnit 2.24.1:** az automatizált tesztek végrehajtása.
- **Git és GitHub:** a verziókezelés és a TDD-fejlesztési folyamat dokumentálása.

## Funkcionalitás

A konverter támogatja a római számírás alapvető és kivonásos alakjait, beleértve az IV, IX, XL, XC, CD és CM jelöléseket.

Példák:

| Arab szám | Római szám |
|---|---|
| 1 | I |
| 4 | IV |
| 9 | IX |
| 14 | XIV |
| 58 | LVIII |
| 1994 | MCMXCIV |
| 3999 | MMMCMXCIX |

A program a 0, a negatív számok, a 3999-nél nagyobb számok, a nem egész számok és a nem megfelelő típusú bemenetek esetén üres karakterláncot (`""`) ad vissza.

## A program futtatása

1. Töltsd le vagy klónozd a GitHub-repositoryt.
2. Nyisd meg az `index.html` fájlt egy webböngészőben.
3. A QUnit tesztfelülete automatikusan megjelenik, és lefuttatja a teszteket.

A QUnit külső CDN-ről töltődik be, ezért a tesztek futtatásához internetkapcsolat szükséges.

## Tesztelés

A projekt automatizált tesztelése a QUnit keretrendszerrel történik.

A tesztek az alábbi területeket fedik le:

1. Az 1-es szám átalakítása.
2. Egyszerű római számok átalakítása.
3. Kivonásos római számok kezelése.
4. Összetett számok átalakítása.
5. A legnagyobb megengedett érték (3999) ellenőrzése.
6. Érvénytelen bemenetek kezelése.

A végleges projekt **6 QUnit-tesztet és 22 ellenőrzést** tartalmaz.

## TDD-fejlesztési folyamat

A fejlesztés során a RED–GREEN–REFACTOR ciklust alkalmaztam:

- **RED:** először elkészítettem az új teszteket, amelyek a hiányzó funkciók miatt sikertelenek voltak.
- **GREEN:** megvalósítottam a tesztek sikeres teljesítéséhez szükséges kódot.
- **REFACTOR:** egyszerűsítettem az algoritmus szerkezetét úgy, hogy a tesztek továbbra is sikeresek maradjanak.

A fejlesztés különböző állapotai és a TDD-ciklusok a GitHub-repository commitelőzményeiben követhetők.

## Projektfájlok

- `index.html` – a JavaScript-konverter és a QUnit-tesztek.
- `README.md` – a projekt dokumentációja.