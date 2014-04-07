4. Laboratorijska vježba
Preopterećenje operatora

Osmisliti i implementirati sustav za obradu stanja tekućeg računa. Transakcije na osnovu kojih se određuje stanje tekućeg računa imaju podatke o vrsti transakcije (uplata/isplata), iznosu i datumu transakcije. Sustav za obradu stanja tekućeg računa sadrži sve transakcije u dvostruko vezanoj listi transakcija, sortiranih po datumu transakcije.
Transakcije trebaju imati mogućnost zbrajanja s drugim transakcijama (povratna vrijednost ukupni iznos transakcija) ili s float vrijednostima (povećanje/smanjenje iznosa transakcije), npr:
cTransakcija a,b,c;
a = a + 5.20;
b = b - 8.60;
c = c + 43.30;
float ukupniIznos = a + b + c;

Ukoliko se pokuša u iznos transakcije upisati negativna vrijednost, treba se spremiti u iznos, kao pozitivna, ali se kao vrsta transakcije, označava „isplata“, odnosno u protivnom „uplata“.
Transakcija treba imati samo jedan konstruktor koji prima samo datum transakcije. Isto tako transakcija ne smije imati nikakve „set“ metode.

Domaći rad
Izraditi klasu cTransakcije, prema gore definiranim zahtjevima.

Zadatak za laboratorijske vježbe
Izraditi sustav za obradu stanja tekućeg računa, i glavni program, koji će uz pomoć izbornika omogućiti:
1. Kreiranje transakcija i njihovo dodavanje u sustav
2. Ispis stanja tekućeg računa
3. Ispis svih transakcije
