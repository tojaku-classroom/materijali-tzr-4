# Zadatak 1: Brojač klikova s temom

- Broj klikova držite u **signalu**.
- Dodajte drugi **signal** za prebacivanje teme (svijetla/tamna).
- Poruka “Bravo!” prikazuje se kada broj klikova pređe 10 – koristi **memo**.
- Stil komponente se mijenja ovisno o signalu teme (inline stil ili klasa).
- Prikažite naslov aplikacije kroz **props**.
- Koristite jednu od metoda životnog ciklusa (npr. `onMount`, `onCleanup`) za konzolnu poruku ili inicijalizaciju.

# Zadatak 2: Todo lista s filtrima

- Zadaci se čuvaju u **signalu** (niz objekata).
- **Signal** filtera ("svi", "završeni", "nezavršeni").
- Korištenje **memo** za filtriranu listu zadataka.
- Svaki todo zadatak je zasebna komponenta kojoj tekst/status dolazi kroz **props**.
- **Efekt** koristi za prikaz upozorenja kada broj zadataka postane veći od 5.
- Različiti stil za završene zadatke (npr. tekst precrtan, siv).

# Zadatak 3: Prikaz stanja semafora

- **Signal** trenutnog stanja (crveno, žuto, zeleno).
- **Efekt** automatski mijenja signal svake 3 sekunde (`setInterval` + `onCleanup`).
- Trenutni signal boje i mijenjanje osvježava preko **memo** za poruku (“Stani”, “Priprema”, “Kreni!”).
- Stil semafora se mijenja prema vrijednosti signala, koristeći inline-stil ili klasu.
- Tekstualni opis ide kroz **props**.
- Prilikom montaže ispišite početno stanje u konzoli (`onMount`).

# Zadatak 4: Kalkulator zbroja i prosjeka

- Unosi (niz brojeva) se drže u **signalu**.
- **Memo** izračunava zbroj i prosjek.
- **Efekt** upozorava ako je unesen broj veći od 100.
- Rezultati zbroja i prosjeka prikazuju se u posebnoj komponenti kojoj vrijednosti dolaze kroz **props**.
- Stil pozadine rezultata dinamički mijenjajte ovisno o veličini prosjeka (plava <10, narančasta 10-50, crvena >50).
- Prilikom pokretanja aplikacije neka se automatski unese nekoliko inicijalnih vrijednosti (**onMount**).