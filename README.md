# Angular Tech Interview
### Vitajte na technickom interview uchádzača o pozíciu Angular Developer.

Prosíme, aby ste pri vypracovaní zadania používali git repozitár, a pravidelne commitovali jednotlivé hotové alebo rozpracované logické časti kódu.

Angular aplikáciu bez prvotného kódu treba commitnúť ako prvú, pod commit message “App Init”
Po tomto commite nasledujú ďalšie v tomto prípade už commity týkajúce sa riešenia.


## Zadanie č.1: EČV Validator
Vytvorte komponent, ktorý bude obsahovať vstup (input typu text), a bude sledovať validitu vstupnej hodnoty. Prosím použite prístup `Reactive form`.

### Vzor pre validný vstup:
Formát: (`okres OO (2 znaky)` zhodný s jedným so zdroju `resources/districts.json`), `číslo 0-9 (3 znaky) CCC`), `písmeno (2 znaky) PP`)
teda `OOCCCPP` [BN737CG].

### Stavy
**Pozitívny scenár:**
Ak vstup bude validný, input bude mať zelený rám a pod ním hlášku: Zadané EČV má správny formát.

**Negatívny scenár:**
Ak vstup validný nebude, input bude mať červený rám a pod ním hlášku: Zadané EČV má nesprávny formát.


## Zadanie č.2: Employees Autocomplete Search
Vytvorte komponent, ktorý bude obsahovať vstup (input typu text) a bude vyhľadávať a ponúkať relevanté dáta zo zdroja `resources/employees.json`.
Po kliknutí na tzv. "Autocomplete suggestion" položku, Zobrazí detail obsahu z vyhľadanéhej položky (zamestnanca). Prosím použite prístup `Reactive form`.

**Detail vyhľadaného zamestnanca by mal vyzerať nasledovne:**

<table>
  <tr>
    <th>Email</th>
    <td>carmela@sultrax.nhk</td>
  </tr>
  <tr>
    <th>Meno a Priezvisko</th>
    <td>Carmela Shaffer</td>
  </tr>
  <tr>
    <th>Dátum narodenia</th>
    <td><strong>25. januára 1992</strong></td>
  </tr>
  <tr>
    <th>Adresa</th>
    <td>69 Moffat Street, Caron, Northern Mariana Islands</td>
  </tr>
  <tr>
    <th>Spoločnosť</th>
    <td>Sultrax</td>
  </tr>
</table>
