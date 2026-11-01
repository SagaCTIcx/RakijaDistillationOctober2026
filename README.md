# Oktobar uz lampek · 2026

Gotov statičan sajt na srpskom i engleskom, pripremljen za GitHub Pages.
Nema instalacije, npm paketa, build koraka, API ključeva niti plaćenih servisa.

## Lokalni pregled

Otvori `index.html` dvoklikom u savremenom browseru (Chrome, Edge, Firefox ili Safari).
Sve funkcije rade lokalno: SR/EN, izbor dana, detalji lampeka, galerija i uvećavanje.
Internet je potreban samo za spoljne linkove ka mapama i stručnoj literaturi.

## Ručno postavljanje na GitHub Pages

1. Napravi **public** GitHub repozitorijum, na primer `oktobar-uz-lampek`. GitHub Free podržava Pages u javnim repozitorijumima.
2. U koren repozitorijuma prenesi **sadržaj ovog foldera**: `index.html`, folder `assets`, `.nojekyll` i ovaj README. Nemoj staviti sve unutar još jednog foldera `OktobarUzLampek`.
3. Ako koristiš ZIP, prvo ga raspakuj. GitHub ne raspakuje ZIP za prikaz sajta. Možeš kroz **Add file → Upload files** da prevučeš raspakovane fajlove i folder `assets`, pa sačuvaš izmene (commit).
4. Otvori **Settings → Pages**. Kao izvor izaberi **Deploy from a branch**, granu **main** i folder **/(root)**. Sačuvaj.
5. Sačekaj da GitHub završi objavljivanje. Adresa će biti prikazana u Pages podešavanjima; za običan projektni repozitorijum obično izgleda kao `https://TVOJE-IME.github.io/oktobar-uz-lampek/`.

Zvanično uputstvo: https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site

Sajt nije objavljen automatski i nije povezan sa tvojim GitHub nalogom.

## Šta je u folderu

```text
index.html
.nojekyll
README.md
assets/
  style.css
  app.js
  data.js
  favicon.svg
  images/
    photo-01-640.jpg
    photo-01-1920.jpg
    ...
```

- `app.js`: srpski i engleski tekstovi, stranica, grafikoni i ponašanje galerije.
- `data.js`: fotografije (originalni naziv, datum, lokacija, kategorija, SR/EN opis) i vremena svakog lampeka.
- `style.css`: boje, izgled i mobilni prikaz.
- Fotografije od 640 px po dužoj strani su za galeriju; od najviše 1920 px za velike prikaze. Originalne proporcije su sačuvane. EXIF rotacija je primenjena, a fotografije su ponovo zapisane bez originalnih EXIF podataka.
- Svih 40 fotografija je uključeno; nema identičnih duplikata po SHA-256 proveri. Slični, ali različiti kadrovi su namerno zadržani.
- Optimizovane fotografije zauzimaju oko 17,1 MB ukupno, naspram oko 113,9 MB originala. Originali nisu menjani.

## Korišćenje

- **SR / EN** menja sve tekstove i opise; izbor se pamti u browseru kad je lokalno skladište dostupno.
- U analitici izaberi dan, pa lampek. Tačna vremena dostupna su i u tabeli.
- U galeriji izaberi aktivnost. Dugme „Prikaži još“ otkriva naredne fotografije.
- Klik otvara celu fotografiju. Koristi dugmad levo/desno ili strelice na tastaturi. Escape zatvara prikaz.
- „Pogledaj pejzaže“ prikazuje fotografije odabranog mesta. Izbor bilo koje kategorije ponovo prikazuje tu kategoriju za oba mesta.
- Google Maps linkovi vode na koordinate koje je dao domaćin. Ugrađena mapa i API ključ nisu potrebni.

## Tačnost i uredničke odluke

- Gornja Crnuća je ispravno ime druge lokacije; Donja Crnuća nije korišćena.
- 7. oktobar: približan raspon 07:30–15:30, bez izmišljenih pojedinačnih satnica.
- 24. oktobar: u 07:20 je već bilo naloženo; prvi interval je označen kao nepotpun, a ukupno kao najmanje 14 h 55 min. Priprema pre dolaska i kasnije sklanjanje nisu uračunati.
- 25. oktobar: 5 h 15 min pokriva pečenje, bez nepoznatog vremena pripreme i sklanjanja.
- Razlike između početka i kraja dana nisu predstavljene kao vreme neprekidnog proticanja.
- Procene količina su označene; nije izračunat lažno precizan prinos sorti ili ukupan alkohol.
- 18 gradi je prikazano kao približno 45% vol.; pitkost je lični izbor domaćina, ne zdravstvena tvrdnja.
- Odvajanje prve litre opisano je kao postupak domaćina, ne kao garancija uklanjanja metanola ili laboratorijske ispravnosti.
- Datumi fotografija preuzeti su iz naziva fajlova. U detaljnom prikazu ne tvrdimo tačan trenutak snimanja fotografija prosleđenih aplikacijama.
- Na samoj stranici ne pominje se „zapisnik“.

## English

A self-contained, bilingual family album and distillation timeline. Open `index.html` locally or upload this folder's contents to the root of a public GitHub repository and enable Pages from the `main` branch. No build step or external dependencies. Use the EN button for the complete English version.

