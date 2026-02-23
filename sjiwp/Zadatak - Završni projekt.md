# Završni projekt: Razvoj Web aplikacije (SolidJS & Firebase)

## 1. Opis i cilj projekta

Cilj ovog projekta je samostalna izrada cjelovite Web aplikacije koristeći suvremene tehnologije za razvoj korisničkog sučelja i pozadinske logike. Projekt se provodi kao završni rad u sklopu predmeta **Skriptni jezici** i **Web programiranje**.

**Tehnološki stog:**

* **Frontend:** SolidJS (JavaScript ES6+)
* **Stil:** TailwindCSS + DaisyUI
* **Pozadina:** Firebase (Authentication, Firestore, Hosting)
* **Verzioniranje:** GitHub

## 2. Vremenski plan i organizacija (~ 20 školskih sati)

Projekt traje ukupno 2 mjeseca (2 sata tjedno).

| Faza | Opis | Trajanje | Vrednovanje | 
| ----- | ----- | ----- | ----- | 
| **Faza 1** | Planiranje i specifikacija | 4 sata | Ocjena dokumentacije | 
| **Faza 2** | Priprema i osnovna funkcionalnost | 4 sata | Provjera stanja projekta | 
| **Faza 3** | Implementacija i objava | 10 sati | Povremeno praćenje stanja | 
| **Završna** | Prezentacija i obrana | 2 sata | Završna ocjena | 

## 3. Faze projekta

### Faza 1: Planiranje (fond: 4 sata)

Rezultat ove faze je datoteka `README.md` unutar GitHub repozitorija projekta.

**Dokumentacija mora sadržavati:**

1. **Detaljan opis (min. 500 riječi):** Što aplikacija rješava, tko su korisnici i zašto je odabrana ta tematika.
2. **Tablica funkcionalnosti (popis za kontrolu):** Popis planiranih mogućnosti. Preporuča se podjela na:
   * *Osnovne mogućnosti* (bez kojih aplikacija nema smisla).
   * *Napredne mogućnosti* (dodatna vrijednost ako ostane vremena).
3. **Scenarij korištenja (korisnički tijekovi):** Opis koraka koje korisnici poduzimaju od prijave do ostvarenja cilja.
4. **Vizualni prototip:** Slike, ilustracije, okviri, prezentacija, statična Web stranica ili link na alat poput Figme koji prikazuje planirani izgled stranica.

### Faza 2: Priprema (fond: 4 sata)

Fokus na postavljanju okruženja i sigurnosti.

**Zadaci:**

* **Postavljanje projekta**: Inicijalizacija SolidJS projekta i konfiguracija TailwindCSS/DaisyUI. Povezivanje s Firebase projektom.
* **Modeliranje baze:** Kratka skica strukture dokumenata u Firestoreu.
* **Autentifikacija:** Implementacija registracije, prijave i odjave.
* **Uloge:** Razlikovanje korisnika (npr. obični korisnik vs. administrator).
* **Korisnički profil:** Pregled i uređivanje podataka trenutnog korisnika.
* **Sigurnost:** Implementacija funkcionalnosti za oporavak zaporke.

### Faza 3: Implementacija (fond: 10 sati)

Izrada kompletne logike aplikacije i njezino javno objavljivanje.

**Zadaci:**

* **Firestore operacije:** Implementacija spremanja, čitanja, ažuriranja i brisanja podataka specifičnih za temu.
* **Logika korisničkog sučelja:** Korištenje SolidJS platforme i njenih mogućnosti (reaktivnost, optimizacija).
* **Responzivni dizajn:** Aplikacija mora biti funkcionalna na mobilnim uređajima i stolnim računalima.
* **Hosting:** Objava aplikacije putem Firebase Hostinga.
* **Završna provjera:** Ažuriranje popisa mogućnosti u `README.md` (što je napravljeno, a što nije).

## 4. Prezentacija i vrednovanje (fond: 2 sata)

Učenik prezentira gotov projekt uz uvid u GitHub repozitorij i objavljenu Web stranicu.

**Bodovne kategorije:**

1. **Kvaliteta dokumentacije:** Je li specifikacija jasna i iscrpna? Prati li `README.md` napredak projekta?
2. **Tehnička izvedba:** Ispravnost koda, korištenje SolidJS koncepata i ispravna konfiguracija Firebasea.
3. **Dizajn i korisničko iskustvo:** Upotreba TailwindCSS i DaisyUI komponenti, estetika i intuitivnost.
4. **Realizacija plana:** Postotak ostvarenih mogućnosti iz Faze 1.
5. **Obrana projekta:** Razumijevanje koda i odgovori na pitanja o implementaciji.

## 5. Pravila

* **Jedinstvenost:** Svaki učenik mora imati različitu temu (prijavljena do kraja 1. sata).
* **Samostalnost:** AI je dopušten kao pomoćni alat, ali učenik mora znati objasniti logiku svakog dijela aplikacije.
* **Verzioniranje:** Obvezno korištenje Git-a s jasnim porukama uz commit-ove.