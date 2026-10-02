## Puuhapaketti: Tekoäly taloushallinnossa

Tämä puuhapaketti sisältää kaksi harjoitusta, joissa pääset kokeilemaan tekoälyn
(esim. Claude, ChatGPT tai muu vastaava työkalu) käyttöä taloushallinnon tehtävissä.
Molemmissa harjoituksissa aineisto on täysin synteettistä eli keksittyä — mikään
yritys- tai henkilötieto ei viittaa todellisiin tahoihin.

### Tehtävä 1: Ostolaskujen automaattinen käsittely

Kansiossa [`10_synteettista_ostotositetta`](10_synteettista_ostotositetta/) on
kymmenen synteettistä ostotositetta (PDF) kuvitteellisilta ohjelmisto- ja
AI-palveluntarjoajilta.

**Tehtävänanto:**

1. Syötä tositteet tekoälytyökaluun (esim. lataamalla PDF:t keskusteluun).
2. Pyydä tekoälyä poimimaan jokaisesta tositteesta ainakin seuraavat tiedot:
   toimittaja, laskun päivämäärä, eräpäivä, summa (alv 0 % ja sis. alv),
   kuvaus ostetusta palvelusta.
3. Pyydä tekoälyä kokoamaan poimitut tiedot yhteen taulukkoon (esim. CSV tai
   Markdown-taulukko).
4. Jatkokysymyksiä pohdittavaksi:
   - Minkä toimittajan kanssa kuluu eniten rahaa?
   - Miten tositteet kannattaisi luokitella kirjanpidon tileille?
   - Miten varmistaisit, ettei tekoäly "keksi" tietoja, joita tositteessa ei ole?

### Tehtävä 2: Asiakkaiden CLV-ennustaminen

Kansiossa [`clv-data`](clv-data/) on kaksi synteettistä CSV-tiedostoa:

- [`asiakkaat.csv`](clv-data/asiakkaat.csv) — 60 kuvitteellista yritysasiakasta
  (toimiala, segmentti, maa, liittymispäivä ym.)
- [`tapahtumat.csv`](clv-data/tapahtumat.csv) — 1000 osto­tapahtumaa näiltä
  asiakkailta kahden vuoden ajalta (2024–2025)

**Tehtävänanto:**

1. Syötä molemmat CSV-tiedostot tekoälytyökaluun.
2. Pyydä tekoälyä laskemaan jokaiselle asiakkaalle asiakkuuden elinkaariarvo
   (Customer Lifetime Value, CLV) — esim. keskimääräinen tapahtuman arvo,
   ostotiheys ja asiakassuhteen pituus huomioiden.
3. Pyydä tekoälyä tunnistamaan:
   - 10 arvokkainta asiakasta
   - segmentit tai toimialat, joissa CLV on korkein
   - asiakkaat, joiden ostoaktiivisuus on hiipumassa (mahdollinen churn-riski)
4. Jatkokysymyksiä pohdittavaksi:
   - Millä oletuksilla tekoäly laski CLV:n — pyysitkö sen kertomaan laskukaavan?
   - Miten tulosta voisi hyödyntää myynnin tai asiakkuudenhoidon priorisoinnissa?
   - Mitä lisätietoa (esim. kate, hankintakustannus) tarvittaisiin tarkempaan
     CLV-laskentaan?
