## Testni scenariji

### Testiranje obveznih vnosnih polj
- Registracija in prijava uporabnikov
    1. Pritisnemo gumb za prikaz obrazca prijave
    2. Vnos pri polju pustimo prazen za vsako polje
    3. Pritisnemo gumb, ki izvede prijavo
    4. Ponovimo to za registracijo
    PRIČAKOVAN REZULTAT: Zavrnitev prijave/registracije v kolikor obvezna polja niso izpolnjena
    
### Testiranje dostop do admin nadzora za osebe, ki imajo ali nimajo status admina
- Admin nadzor nad vsebino in uporabniki
    1. Preverjanje povelnic osebe (če je admin ali ne)
    2. Poskus dostopa do adminskih funkcij z admin računom in z računom brez admin statusa
    3. Spreminjanje statusa uporabnika brez admin statusa v admin za en račun in obratno za drug
    4. Ponovitev koraka 2 z spremenjenimi računi
    PRIČAKOVAN REZULTAT: Uporabnik brez admin pravic ne more dostopati do funkcij admina, tudi če je bil admin v preteklosti in admin lahko dostopa, tudi če ni imel pravic v preteklosti

### Preverjanje rezervacije storitev7spletnih vsebin glede na bančni račun uporabnika
-Ogled in rezervacija storitev/spletnih vsebin
    1. Vnos podatkov plačilne storitve če še niso bili vnešeni v nastavitvah uporabnika
    2. Preverjanje, če je denar v bančnem računu manjši od cene rezervacije storitev
    PRIČAKOVAN REZULTAT: Če je denar manjši, rezervacija ne gre skozi in uporabniku sporoči zakaj, drugače pa denar-cena
