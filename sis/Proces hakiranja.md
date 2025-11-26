Hakiranje (engl. hacking) s gledišta informacijske sigurnosti je proces iskorištavanja ranjivosti sustava i zaobilaženja sigurnosnih kontrola s ciljem dobivanja nedozvoljenog ili neprikladnog pristupa sustavu. Haker (engl. hacker) je u tom kontekstu osoba koja provaljuje u sustav ili mrežu bez dozvole s ciljem uništenja ili krađe osjetljivih podataka ili izvođenja drugih oblika zlonamjernih napada. Naravno, ova definicija se odnosi na kriminalne radanje, no nisu svi hakeri nužno kriminalci. S obzirom na aktivnosti i motive, hakere možemo klasificirati na sljedeći način:

- Engl. black hat, crackers - kriminalci koji provode ilegalne i nedozvoljene radnje.
- Engl. white hat, penetration testers - prvode iste ili slične aktivnosti kao i kriminalci ali imaju dozvolu, njihova je uloga defenzivne prirode, odnosno cilj je pronaći i iskoristiti ranjivosti s ciljem njihova otklanjanja.
- Engl. gray hat - provode s jedne strane legalne, a s druge ilegalne aktivnosti.
- Engl. red hat - hakeri koji napadaju black hat hakere; iako napadaju kriminalce njihove se radnje također smatraju ilegalnima.
- Engl. blue hat - može imati dvostruko značenje; s jedne strane označavati hakere koji ilegalno napadaju iz osvete, a s druge strane može označavati vanjske hakere koje unajmljuje organizacija kao sigurnosne stručnjake s ciljem provođenja legalnih aktivnosti.
- Engl. green hat - početnici na području informacijske sigurnosti.
- Hakeri samoubojice (engl. suicide hackers) - provode ilegalne aktivnosti za neki "viši" cilje bez obzira na posljedice.
- Engl. script kiddies - najčešće mlađi hakeri, iako nije nužno, koji imaju ograničeno ili nikakvo znanje i izvode ilegalne aktivnosti isključivo korištenjem postojećih alata, često ne znajući kako ti alati stvarno funkcioniraju.
- Engl. cyber terrorists - hakeri koji provode ilegalne aktivnosti s ciljem izazivanja straha i najčešće su religiozno ili politički motivirani.
- Hakeri sponzorirani od strane države (engl. state-sponsored hackers) - kao što sam naziv govori, sponzorira ih država, često skriveno ili neslužbeno, i provode ilegalne aktivnosti protiv neprijateljskih ili konkurentskih država.
- Haktivisti (engl. hacktivists) - hakeri koji provode ilegalne aktivnosti s različitim motivima od protesta, drušvenih ili političkih razloga, utjecaja na vlastitu reputaciju itd.

Proces hakiranja (engl. hacking) s gledišta hakera obično obuhvaća sljedeće faze:

1. Izviđanje (engl. reconnaissance) - podrazumijeva skupljanje podataka o meti napada koji će nam biti od važnosti u kasnijim fazama.
2. Pasivno - ne dolazimo u interakciju s metom i koristimo javno dostupne podatke ili engl. OSINT - Open Source INTelligence.
3. Aktivno - dolazimo u direktnu interakciju s metom iako je vjerojatnost otkrivanja naših aktivnosti relativno mala.
4. Skeniranje (engl. scanning) - ova faza se smatra fazom prije samog napada u kojoj koristimo podatke prikupljene u prethodnoj fazi i koristeći alate za skeniranje (mreže, čvorova, ranjivosti) pokušavamo dobiti detaljni uvid i specifične informacije o mreži koju napadamo.
5. Dobivanje pristupa (engl. gaining access) - poduzimamo razne vrste napada s ciljem dobivanja pristupa mreži, operacijskom sustavu i/ili aplikacijama. U ovoj fazi ćemo i često pokušati povećati svoje dozvole u sustavu poželjno do razine administratora (engl. escalate privileges). Neki primjeri napada koje ovdje poduzimamo mogu biti otkrivanje zaporki, engl. buffer overflow (ranjivost aplikacija), denial of service (uskrata pristupa usluzi), session hijacking (engl. otimanje sesije), spoofing (pretvaranje)...
6. Održavanje pristupa (engl. maintaining access) - u ovoj fazi ćemo najčešće manipulirati podacima, aplikacijama i konfiguracijom s ciljem održavanja vlasništva nad sustavom i pokretanja drugih napada. Često ćemo koristiti zlonamjerne programe poput engl. backdoors, rootkits ili trojanskih konja (engl. trojans).
7. Brisanje tragova (engl. clearing tracks) - u ovoj fazi pokušavamo sakriti svoj identitet i prisustvo i ukloniti sumnju uz upotrebu tehnika poput engl. tunneling, steganografije, enkripcije itd. Ova je faza često faza izviđanja u novom ciklusu napada na sustav koji smo prethodno kompromitirali.

## Etičko hakiranje

Etičko hakiranje je strukturirana i organizirana procjena sigurnosti sustava. Dio je procesa procjene rizika u sustavu i smatra se dobrom praksom na području informacijske sigurnosti. U osnovi radi se o identificiranju rizika i definiranju akcija koje treba poduzeti kako bi se rizici uklonili ili ublažili s ciljem smanjenje troškova korištenja informacijsko-komunikacijskih tehnologija u organizaciji. Troškovi uspješnog napada na organizaciju mogu biti značajni i uvijek će biti veći po organizaciju od proaktivnog pristupa i prevencije napada. Etičko hakiranje provode etički hakeri ili tzv. white hat hakeri. Prilikom angažiranja etičkog hakera organizacija mora imati jasne ciljeve i razloge zašto to radi, te zaključke koji su rezultat etičkog hakiranja mora primijeniti, ukloniti nedostatke i postaviti odgovarajuće zaštite.

Posao etičkog hakera, nakon što pribavi dozvolu za početak procesa, jest pronaći ranjivosti, dokumentirati ih i predožiti mjere koje treba poduzeti kako bi se ranjivosti sustava uklonile. Etički haker nikada ne smije namjerno izazvati štetu, prilikom provođenja procesa testiranja sustava mora izbjegavati nastanak štete po svaku cijenu i držati se ograničenja testiranja dogovorenih prije samog početka. Obično se prethodno početku potpisuju određeni pravni dokumenti koji definiraju opseg usluge i ograničenja:

- ROE, engl. Rules of Engagement - dokument koji predstavlja formalnu dozvolu za početak procesa i definira ograničenja i dogovoreni opseg usluge.
- NDA, engl. Non-Disclosure Agreement - predstavlja sporazum o tajnosti podataka.

Možemo općenito promatrati tri osnovne razine ili postupke procjene sigurnosti sustava:

- Revizija sigurnosti (engl. security audit) - predstavlja provjeru i reviziju sigurnosnih politika i procedura i obično je samo početak procesa procjene sigurnosti sustava, te nije dostatan za potpunu procjenu sigurnosti. Organizacije trebaju implementirati princip zaštite u dubinu (engl. defense-in-depth) kroz proces simulacije napada i napadača i proboja u vlastite mreže kroz otkrivanje i iskorištavanje ranjivosti.
- Procjena ranjivosti (engl. vulnerability assessment) - predstavlja proces otkrivanja ranjivosti sustava bez postupka iskorištavanja tih ranjivosti.
- Penetracijsko ispitivanje (engl. penetration testing) - obuhvaća kompletan proces procjene sigurnosti od revizije sigurnosti, otkrivanja ranjivosti i iskorištenja ranjivosti.

Etički haker će identificirati ranjivosti koristeći alate i tehnike koje koriste napadači i dat će odgovor na pitanja: što napadač vidi?, što napadač može učiniti? i možemo li identificirati napadačeve pokušaje u našem sustavu?