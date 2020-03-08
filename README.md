# ITAcademy - Javascript Frontend Development kurs
## Zadaci za samostalni rad i rešeni zadaci

### Zadatak 1

Napisati program koji radi konverziju celzijusa u farenhajte. Korisnik unosi vrednost celzijusa u input polje, a vrednost farenhajta se prikazuje u okviru paragrafa. Konverzija se pokreće klikom na dugme "Konvertuj". Za samu konverziju potrebno je napisati funkciju **c2f** koja prihvata kao argument vrednost celzijusa, a vraća vrednost farenhajta.

**Pomoć:** [Formula za konverziju](https://www.rapidtables.com/convert/temperature/how-celsius-to-fahrenheit.html)

### Zadatak 2

Napisati program koji radi konverziju celzijusa u farenhajte. Korisnik unosi vrednost celzijusa u input polje, a vrednost farenhajta se prikazuje u okviru paragrafa. Konverzija se pokreće onog trenutka kada korisnik u input unese numeričku vrednost. Ne treba pokretati vrednost ako je vrednost input polja prazna. Za samu konverziju potrebno je napisati funkciju **c2f** koja prihvata kao argument vrednost celzijusa, a vraća vrednost farenhajta.

**Pomoć:** [Formula za konverziju](https://www.rapidtables.com/convert/temperature/how-celsius-to-fahrenheit.html)

### Zadatak 3

Napisati program koji radi računanje i zapremine određenih geometrijskih tela. Geomatrijska tela koja su na raspolaganju su valjak, kupa, lopta i kvadar. Za računanje korisnik ima mogućnost izbora tela čiju površinu i zapreminu želi da izračuna i koristi radio grupu da izabere telo. U zavisnosti od izbora tela treba da se pojave odgovarajuća polja za unos:

1. Za valjak potrebno je da korisnik dobije polja za unos *r* i *H*.
2. Za kupu potrebno je da korisnik dobije polja za unos *r*, *s* i *H*.
3. Za loptu potrebno je da korisnik dobije polja za unos *r*.
4. Za kvadar potrebno je da korisnik dobije polja za unos *a*, *b* i *c*

Treba voditi računa o iskoristivosti koda. Ne želite da svaki element ima svoja polja za unos već da imaju tri polja čija se uloga menja od tela koje je izabrano. Ako korisnik izabere loptu, treba da vidi samo jedno polje za *r*. Ako korisnik izabere kvadar treba da vidi tri polja za *a* (odnosno to polje može biti polje i za *r*), za *b* (takođe *s*) i *c* (takođe *H*). Znači treba prikazati polje i dati mu odgovarajuću labelu pored prikaza. Koristite CSS display svojstvo za kontrolu prikaza (none/inline-block) i atribut *style* za kontrolu prikaza elemenata.

Na kraju rezultate je potrebno prikazati u paragrafu.

**Pomoć**: [Formule za površinu i zapreminu geometrijskih tela](https://www.opsteobrazovanje.in.rs/matematika/osnovna-skola/povrsine-i-zapremine-geometrijskih-tela/)

### Zadatak 4

Napisati program koji pomaže prodavcu obračun troškova za slanje robe. Paketi se pakuju kao kvadri. Od prodavca se traži da za paket unese zapreminu (m³) i težinu (kg) za paket koji šalje. Takođe prodavac ima izbor službe za slanje iz padajuće liste:
 - Economy
 - Small packets
 - Standard Shipping
 - Premium Shipping
 - UPS

U zavisnosti od izbora potrebno je proveriti da li se paket može uopšte slati:
 - Economy - prihvata pošiljke čija zapremina ne prelazi 1m³, i koji nisu teži od 1kg.
 - Small packets - prihvata pošiljke čija zapremina ne prelazi 500cm³ i nisu teži od 500g.
 - Standard - prihvata pošiljke čija zapremina ne prelazi 3m³ i koji nisu teži od 5kg.
 - Premium - prihvata pošiljke čija zapremina ne prelazi 10m³ i koji nisu teži od 20kg.
 - UPS - prihvata sve pošiljke.

Nakon unetih izbora treba izračunati troškove slanja. Troškovi slanja paketa se obračunavaju po težini paketa, ne po zapremini i tabela izgleda ovako:

| Način slanja  | <= 500g | 501g - 1kg | 1kg - 5kg | 5kg - 10kg | 10kg+ |
| --- | --- | --- | --- | --- | --- |
| Economy  | 10RSD/50g | 9RSD/50g | / | / |
| Small packets  | 5RSD/50g | / | / | / | / |
| Standard Shipping  | 20RSD/50g | 18RSD/50g | 15RSD/50g | / | / |
| Premium Shipping  | 50RSD/50g | 45RSD/50g | 30RSD/50g | 25RSD/50g | 23RSD/50g |
| UPS  | 500RSD | 1200RSD | 60RSD/50g | 55RSD/50g | 100RSD/200g |

Računanje se izvršava klikom na dugme "Troškovi slanja". Podaci treba za računanje treba da se čuvaju kao objekti koji su deo niza i na osnovu izabrane opcije iz padajuće liste (hint: value čuvajte kao indeks niza) potrebno je da se iskoriste za računanje cene slanja. Svi podaci o ograničenju i cenama slanja trebaju biti u okviru objekta. Vama se ostavlja izbor dizajna strukture samih objekata.
