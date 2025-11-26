### 1. **Što je "full stack" aplikacija?**

"Full stack" aplikacija obuhvaća dvije glavne komponente:

- **Front end**: Dio aplikacije koji korisnik vidi i s kojim neposredno komunicira. To uključuje sve vizualne elemente korisničkog sučelja, kao što su gumbi, obrasci, tekst i slike.
- **Back end**: Ovo je pozadinski dio aplikacije koji korisnik ne vidi, ali osigurava da aplikacija ispravno funkcionira. Obuhvaća poslužitelje, baze podataka, API-je i poslovnu logiku koja stoji iza aplikacije.

U sklopu ovog predmeta, fokusirat ćemo se na **front end** razvoj, koristeći **JavaScript** kao osnovni programski jezik i **SolidJS** kao platformu za izradu korisničkog sučelja.

### 2. **Uloga JavaScript-a i SolidJS-a u "front end" razvoju**

- **JavaScript** je temeljni jezik za razvoj interaktivnih web stranica. Njime možemo upravljati događajima na stranici, dinamički mijenjati sadržaj te omogućiti interakciju bez ponovnog učitavanja stranice s poslužitelja.
- **SolidJS** je platforma (framework) za JavaScript koji omogućava stvaranje korisničkih sučelja. Njegova ključna značajka je reaktivnost – automatski ažurira elemente na stranici kad se promijene podaci, što omogućava brži i učinkovitiji rad u usporedbi s klasičnim poslužiteljskim platformama.

### 3. **Što su IaaS, PaaS i SaaS?**

U računalstvu u oblaku (cloud computing) razlikujemo tri glavne vrste usluga:

- **IaaS (Infrastructure as a Service)**: Ova usluga pruža infrastrukturu kao što su poslužitelji, mreže i pohrana podataka na oblaku. Korisnici imaju potpunu kontrolu nad infrastrukturom, što omogućava fleksibilnost, ali zahtijeva tehničku stručnost i vrijeme za održavanje.
- **PaaS (Platform as a Service)**: PaaS omogućava razvoj aplikacija bez brige o infrastrukturi. Ova platforma pruža sve potrebne alate za razvoj, testiranje i implementaciju aplikacija, dok se pružatelj usluga brine o poslužiteljima i sigurnosti. To je idealno za brži razvoj uz minimalne administrativne obveze.
- **SaaS (Software as a Service)**: SaaS su gotovi softverski proizvodi koje korisnici mogu izravno koristiti putem interneta, poput Google Docs ili Dropboxa. Korisnici nemaju kontrolu nad kodom, već koriste unaprijed izgrađene aplikacije.

Za naš projekt, odlučili smo koristiti **PaaS** jer nam omogućava jednostavno postavljanje "back end" sustava bez potrebe za upravljanjem infrastrukturom i razvojem uobičajenih značajki potrebnih na strani poslužitelja.

### 4. **PaaS platforme: usporedba Google Firebase, Appwrite, Supabase i PocketBase**

Razmotrili smo nekoliko PaaS platformi koje mogu poslužiti kao "back end" našoj aplikaciji. Evo sažetka:

- **Google Firebase**: Popularna platforma za razvoj mobilnih i web aplikacija. Pruža jednostavno postavljanje baze podataka, autentifikaciju korisnika i obavijesti (push notifications). Nedostatak je što koristi NoSQL baze podataka, što nije uvijek pogodno za aplikacije s relacijskim bazama.
- **Appwrite**: Otvorena platforma koja omogućava jednostavnu integraciju s aplikacijama. Nudi veliki broj alata za upravljanje korisnicima, bazama podataka i autentifikacijom, no zahtijeva više tehničkog znanja za postavljanje.
- **Supabase**: Također otvorena platforma, ali s naglaskom na relacijske baze podataka (PostgreSQL). Nudi jednostavno postavljanje, autentifikaciju korisnika, real-time baze podataka i pohranu datoteka. Prikladan je za složenije aplikacije koje trebaju relacijsku bazu podataka.
- **PocketBase**: Laka i brza platforma s real-time mogućnostima, idealna za manje projekte i prototipe. Međutim, nije pogodna za složenije aplikacije s većim zahtjevima nad bazom podataka budući da se bazira na SQLite. Također, razvijena je Go jezikom, pa se pisanje proširenja razvija u istom jeziku.  