# Nash Trade — sajt

Prezentacioni sajt firme Nash Trade (kelnerski vadičepovi, poklon kutije, vino).

Sajt je `index.html` plus folder `slike/`.

Slike proizvoda su isečene iz kataloške fotografije dobavljača
(`slike/izvornik-kataloska.jpg`) — bela pozadina je uklonjena i svaki
pogled je snimljen kao zaseban WebP sa providnom pozadinom.

Zamena slike: ubaci novi fajl u `slike/` i promeni putanju u `index.html`.
Slike sa providnom pozadinom treba da budu isečene bez svetlog oboda,
jer se sajt prikazuje na tamnoj podlozi.

## Gde je live

Sajt se objavljuje preko GitHub Pages iz ovog repozitorijuma.

## Kontakt forma

Dugme „Pošalji upit na WhatsApp" ne šalje mejl — ono otvara WhatsApp sa već
popunjenom porukom, koju kupac samo pošalje. Upiti tako stižu na telefon
060 6316025.

Broj se menja na jednom mestu, u `index.html`, u liniji:

    var WA_BROJ = "381606316025";

Format je pozivni broj države bez plusa i bez prve nule:
`060 6316025` → `381606316025`.

## Cene

Cene i količinski rangovi stoje na dva mesta u `index.html` i moraju da se
menjaju **oba**, inače će tabela i kalkulator prikazivati različite cene:

1. u tabeli cenovnika (HTML, sekcija `id="cenovnik"`),
2. u kalkulatoru (JavaScript, niz `var tiers=[...]`).
