## Zadatak 1: Kategorije Događaja & Filtriranje

### Opis
Dodaj mogućnost kategorizacije događaja kako bi korisnici mogli lakše pronaći događaje koji ih zanimaju.

### Zahtjevi
- Dodaj `category` polje na događaje (dropdown s opcijama: "Sports", "Music", "Social", "Other")
- Na Home stranici dodaj gumbe za filtriranje javnih događaja po kategoriji
- Prikaži `category` značku na karticama događaja
- U EventManagement-u omogući filtriranje svojih događaja po kategoriji
- Zadržavaj kategoriju pri ažuriranju događaja

### Tehnički detalji
- **Firestore polje**: `category: string`
- **Firestore upit**: Koristi `where("isPrivate", "==", false)` i `where("category", "==", selectedCategory)`
- **Komponente za izmjenu**: Home.jsx, EventManagement.jsx

### Temeljne vještine
- Firestore `where()` upiti
- Form `<select>` elementi
- Signal filtriranje
- Conditional rendering s `<Show>`

## Zadatak 2: Sustav Prisustva na Događajima

### Opis
Omogući korisnicima da se prijave za događaje i prati koji su korisnici registrirani.

### Zahtjevi
- Dodaj `attendees: []` niz na događaje (sličan strukturi kao `favorites`)
- Na Home stranici korisnici mogu kliknuti "Pridruži se" ili "Napusti" događaj
- Prikaži broj prijavljenih korisnika na karticama događaja
- Prikaži "Prisutni ste ✓" indikator ako je korisnik već prijavljeni
- U EventManagement-u prikaži listu tko je prijavljeni na svaki događaj

### Tehnički detalji
- **Firestore polje**: `attendees: [] (array of userIds)`
- **Firestore operacije**: `arrayUnion(userId)` i `arrayRemove(userId)`
- **Komponente za izmjenu**: Home.jsx, EventManagement.jsx

### Temeljne vještine
- `arrayUnion()` i `arrayRemove()` operacije
- Sinkronizacija stanja nakon ažuriranja
- Uvjetno renderiranje s `<Show>`
- Array `includes()` provjere

## Zadatak 3: Razina Težine Događaja & Preporuke

### Opis
Klasificiraj događaje po razini težine kako bi se korisnici lakše orijentirali.

### Zahtjevi
- Dodaj `difficulty` polje na događaje (dropdown: "Beginner", "Intermediate", "Advanced")
- Na Home stranici dodaj filtriranje javnih događaja po razini težine (gumbi ili dropdown)
- Prikaži `difficulty` značku na karticama događaja s razičitim bojama (npr. zeleno=Beginner, žuto=Intermediate, crveno=Advanced)
- U EventManagement-u omogući filtriranje svojih događaja po težini

### Tehnički detalji
- **Firestore polje**: `difficulty: string`
- **Firestore upit**: Koristi `where("difficulty", "==", selectedDifficulty)`
- **Komponente za izmjenu**: Home.jsx, EventManagement.jsx

### Temeljne vještine
- Firestore upiti s filteriranjem
- Conditional CSS klase za bojanje značaka
- Signal filtriranje
- Array operacije za preporuke (bonus)

## Zadatak 4: Trajanje Događaja & Praćenje Statusa

### Opis
Prati trajanje i trenutni status događaja kako bi korisnici znali što očekivati.

### Zahtjevi
- Dodaj `duration` polje (broj sati, npr. 2, 3.5) na događaje
- Dodaj `status` polje s opcijama: "Upcoming" (Dolazi), "Ongoing" (U tijeku), "Completed" (Završeno)
- Na Home stranici prikaži trajanje događaja
- Dodaj toggle gumb "Prikaži samo nadolazeće" koji filtrira događaje po statusu
- U EventManagement-u omogući označavanje svojih događaja kao "Ongoing" ili "Completed"
- Prikaži obojane status indikatore (zeleno=Upcoming, žuto=Ongoing, sivo=Completed)
- Status se može ažurirati samo tijekom uređivanja događaja

### Tehnički detalji
- **Firestore polja**: `duration: number`, `status: string`
- **Firestore upit**: Koristi `where("status", "==", "Upcoming")`
- **Komponente za izmjenu**: Home.jsx, EventManagement.jsx

### Temeljne vještine
- Firestore ažuriranja dokumenata s `updateDoc()`
- Conditional CSS klase za obojavanje
- Uvjetno filtriranje u UI-u
- Form select elementi za izbor statusa