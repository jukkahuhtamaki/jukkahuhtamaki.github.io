<style type="text/css">
  body {
    background-color: #141414;
    color: #d4d4d4;
  }
  #main {
    max-width: 760px;
    font-family: "Courier New", "SF Mono", Consolas, monospace;
  }
  .terminal {
    background: #191919;
    border: 1px solid #2e2e2e;
    padding: 1.6em 1.9em;
  }
  .terminal h2, .terminal h3 {
    font-family: inherit;
    font-weight: normal;
    color: #8fd19e;
    border-bottom: 1px solid #2e2e2e;
    padding-bottom: 0.4em;
  }
  .terminal h3::before { content: "> "; color: #666; }
  .terminal p, .terminal li { line-height: 1.6; }
  .terminal strong { color: #8fd19e; }
  .terminal a { color: #8fd19e; text-decoration: underline; }
  .terminal a:hover { color: #d4d4d4; }
  .terminal code {
    background: #111;
    color: #8fd19e;
    padding: 0.1em 0.35em;
    border-radius: 2px;
  }
  .terminal blockquote {
    border-left: 2px solid #444;
    margin-left: 0;
    padding-left: 1em;
    color: #999;
    font-style: italic;
  }
  .terminal ul, .terminal ol { margin-left: 0.2em; }
  .terminal hr {
    border: none;
    border-top: 1px solid #2e2e2e;
    margin: 2em 0;
  }
  .tag {
    display: inline-block;
    color: #888;
    font-size: 0.75em;
    letter-spacing: 0.05em;
    margin-bottom: 1em;
  }
</style>

<div class="terminal" markdown="1">

<span class="tag">synteettinen aineisto — ei oikeita yrityksiä tai henkilöitä</span>

## Puuhapaketti: Tekoäly taloushallinnossa

Tämä puuhapaketti sisältää kaksi harjoitusta, joissa pääset kokeilemaan tekoälyn
(esim. Claude, ChatGPT tai muu vastaava työkalu) käyttöä taloushallinnon tehtävissä.
Molemmissa harjoituksissa aineisto on täysin synteettistä eli keksittyä — mikään
yritys- tai henkilötieto ei viittaa todellisiin tahoihin.

> Älä luota — tarkista. Tekoäly ei ole auktoriteetti, se on työkalu.

### Tehtävä 1: Ostolaskujen automaattinen käsittely

Kymmenen synteettistä ostotositetta (PDF) kuvitteellisilta ohjelmisto- ja
AI-palveluntarjoajilta:

1. [Nordic AI Services](10_synteettista_ostotositetta/01_nordic_ai_services.pdf)
2. [Cloud North Europe](10_synteettista_ostotositetta/02_cloud_north_europe.pdf)
3. [Open Model API](10_synteettista_ostotositetta/03_open_model_api.pdf)
4. [UX Lab](10_synteettista_ostotositetta/04_ux_lab.pdf)
5. [Data License Partners](10_synteettista_ostotositetta/05_data_license_partners.pdf)
6. [SecureByte](10_synteettista_ostotositetta/06_securebyte.pdf)
7. [DevTools Europe](10_synteettista_ostotositetta/07_devtools_europe.pdf)
8. [AI Quality House](10_synteettista_ostotositetta/08_ai_quality_house.pdf)
9. [Promptworks](10_synteettista_ostotositetta/09_promptworks.pdf)
10. [Vector Hosting](10_synteettista_ostotositetta/10_vector_hosting.pdf)

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

<hr/>

### Tehtävä 2: Asiakkaiden CLV-ennustaminen

Kaksi synteettistä CSV-tiedostoa:

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

</div>
