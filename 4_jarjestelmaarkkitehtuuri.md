##  Järjestelmäarkkitehtuuri

* Pyri kuvailemaan tässä luvussa järjestelmäarkkitehtuuri yleisellä tasolla
* Mitä komponentteja järjestelmään tarvitaan jotta se pystyy palvelemaan määritettyjä käyttötapauksia?


Komponentit:

Kirjautuminen:
Järjestelmään kirjaudutaan käyttäen metropolian omaa kirjautumisjärjestelmää. Näin sovelukseen ei tarvita omaa tietokantaa käyttäjänimille ja salasanoille.


Paikannuskomponentti:
Paikannuskomponentti toimii keräämällä wifi-signaalien voimakkuuksia. Komponentti sisältää tiedon siitä missä huoneissa näkyy mitkäkin wifi-signaalit. Voimakkuuksista päätellään käyttäjän sijainti halutulla hetkellä.


Lukujärjestyskomponentti:
Kirjautumisen onnistuttua järjestelmä hakee käyttäjän nimen perusteella tämän ryhmän ja ryhmän perusteella tämän hetkisen oletuslukujärjestyksen.


Chattikomponentti:
Chattikomponentin kautta voidaan viestittää muille henkilöille pikaviestejä. Chattikomponentti sisältää tietokannan käyttäjän lisäämistä kavereista.


Huonetiedot:
Huoneiden tiedot haetaan metropolian omasta tietokannasta. Tiedoissa näkyy huoneen nimen lisäksi tietokoneiden määrä ja asennetut ohjelmat.


Karttakomponentti:
Sisältää kartat Metropolian kampuksista. Huoneita voi klikata jolloin huonetiedoista haetaan valitun huoneen data. Karttakomponentilla näytetään myös käyttäjän sijainti ja lukujärjestyskomponentin avulla seuraavan luennon sijainti.