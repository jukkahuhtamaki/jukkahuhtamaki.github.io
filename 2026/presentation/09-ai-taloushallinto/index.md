<style type="text/css">
  body {
    background-color: #0a0a0a;
    color: #c8c8c8;
  }
  #main {
    max-width: 760px;
    font-family: "Courier New", "SF Mono", Consolas, monospace;
  }
  .terminal {
    background: #000;
    border: 1px solid #2a2a2a;
    border-left: 3px solid #39ff14;
    padding: 1.5em 1.8em;
    box-shadow: 0 0 18px rgba(57, 255, 20, 0.08);
  }
  .terminal h2, .terminal h3 {
    font-family: inherit;
    text-transform: uppercase;
    letter-spacing: 0.08em;
    color: #39ff14;
    border-bottom: 1px dashed #333;
    padding-bottom: 0.4em;
  }
  .terminal h2::before { content: "root@puuhapaketti:~# "; color: #666; font-size: 0.6em; display: block; margin-bottom: 0.3em; }
  .terminal h3::before { content: "> "; color: #ff003c; }
  .terminal p, .terminal li { line-height: 1.6; }
  .terminal strong { color: #39ff14; }
  .terminal a { color: #39ff14; text-decoration: underline; }
  .terminal a:hover { color: #ff003c; }
  .terminal code {
    background: #111;
    color: #39ff14;
    padding: 0.1em 0.35em;
    border-radius: 2px;
  }
  .terminal blockquote {
    border-left: 2px solid #ff003c;
    margin-left: 0;
    padding-left: 1em;
    color: #999;
    font-style: italic;
  }
  .terminal ul, .terminal ol { margin-left: 0.2em; }
  .terminal hr {
    border: none;
    border-top: 1px dashed #333;
    margin: 2em 0;
  }
  .tag {
    display: inline-block;
    background: #111;
    color: #ff003c;
    border: 1px solid #ff003c;
    font-size: 0.75em;
    text-transform: uppercase;
    letter-spacing: 0.1em;
    padding: 0.15em 0.5em;
    margin-bottom: 1em;
  }
</style>

<div class="terminal" markdown="1">

<span class="tag">classified // synteettinen aineisto</span>

## Puuhapaketti: Tekoäly taloushallinnossa

Tämä puuhapaketti sisältää kaksi harjoitusta, joissa pääset kokeilemaan tekoälyn
(esim. Claude, ChatGPT tai muu vastaava työkalu) käyttöä taloushallinnon tehtävissä.
Molemmissa harjoituksissa aineisto on täysin synteettistä eli keksittyä — mikään
yritys- tai henkilötieto ei viittaa todellisiin tahoihin.

> Älä luota — tarkista. Tekoäly ei ole koskaan auktoriteetti, se on työkalu.

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

<hr/>

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

</div>
