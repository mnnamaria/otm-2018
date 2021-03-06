# KESKEN

## harjoitustyö, viikko 5

Palautuksen deadline ti 24.4. klo 23:59

Muista pushata  harjoitustyöhön liittyvät asiat GitHubiin ennen viikkodeadlinea.
- Jos pushaus tapahtuu myöhässä, mutta deadlinea seuraavaan aamuun klo 07 mennessä, saat viikkopisteet vähennettynä yhdellä. 
- Klo 07 jälkeen tulevia repositorion päivityksiä ei huomioida pisteytyksessä, eli ne tuovat 0 pistettä.

Palautuksesta on tarjolla 3 kurssipistettä.

Arvostelussa kiinnitetään huomiota seuraaviin seikkoihin

- Ohjelmasta pystyy tekemään suorituskelpoisen [jar](https://github.com/mluukkai/otm-2018/blob/master/web/maven.md#jarin-generointi)-tiedoston komennolla _mvn package_ (0.5p) 
  - jos käytät käytössäsi on joku muu kieli kuin Java, oletuksena on että teet kyseiselle kielelle mielekkään suoritettavan version   
- Ohjelma on kasvanut edellisestä viikosta (0.75p)
  - Ohjelmasta on olemassa suoritettava versio, joka on kasvanut edellisestä viikosta _ja_ toteuttaa edellisen viikon versiota suuremman osan määrittelydokumentin toiminnallisuudesta
- Projektista on tehty _github release_ (0.25p) 
  - Release sisältää ohjelman suorituskelpoisen jar-tiedoston
  - [Ohje](https://github.com/mluukkai/otm-2018/blob/master/web/release.md) releasen tekemiseen
- Testaus on edennyt (0.5p)
  - Sovellukselle tulee pystyä generoimaan testikattavuusraportti komennolla <code>mvn test jacoco:report</code>
  - Käyttöliittymän rakentava koodi [jätetään pois](https://github.com/mluukkai/otm-2018/blob/master/web/maven.md#koodin-huomiotta-jättäminen-kattavuusraportissa) testikattavuusraportista
  - Sovelluksen testien rivikattavuuden tulee olla vähintään 40%
  - Jos teet projektisi jollain muulla kielellä kuin Javalla, lisää README-tiedostoon ohje testien suorittamiselle ja kattavuusraportin generoimiselle
- Koodin laatu (0.5p)
  - Sovelluslogiikka on riittämässä määrin eriytetty käyttöliittymästä
    - Vihjeitä [täällä](https://github.com/mluukkai/otm-2018/blob/master/web/java.md) ja [referenssisovelluksessa](https://github.com/mluukkai/OtmTodoApp/blob/master/dokumentaatio/arkkitehtuuri.md)
  - Ohjelman [pakkausrakenne](https://github.com/mluukkai/otm-2018/blob/master/web/koodin_laatuvaatimukset.md#5-pakkaukset) heijastaa ohjelman loogista rakennetta ja on nimennältään järkevä
  - Checkstyle on otettu käyttöön 
    - Ohje Checkstylen käyttöönottoon [täällä](https://github.com/mluukkai/otm-2018/blob/master/web/checkstyle.md)
    - Täydet pisteet Checkstylestä ainoastaan jos ohjelmassa on alle 5 Checkstyle-virhettä
    - Käyttöliittymän rakentavan koodin ei tarvitse olla Checkstyle-tarkastelun alla
    - Jos teet projektisi jollain muulla kielellä kuin Javalla, tulee olla käytössä kielen _Checkstyleä_ vastaava työkalu, määrittele se järkevästi ja laita README-tiedostoon ohje tyylitarkastusten suorittamisele
- Ohjelman ssa on ainakin yksi sen jotain oleellista toiminnallisuutta kuvaava sekvenssikaavio (0.5p)
  - Mallia voi ottaa [referenssisovelluksesta](https://github.com/mluukkai/OtmTodoApp/blob/master/dokumentaatio/arkkitehtuuri.md#sovelluslogiikka)
  - Lisää kuva [edellisellä viikolla](https://github.com/mluukkai/otm-2018/blob/master/tehtavat/harjoitustyo_viikko4.md) tehtyyn dokumenttiin _arkkitehtuuri.md_ 
  - Tiedostoon _arkkitehtuuri.md_ tulee olla linkki repositorion README:stä [referenssisovelluksen](https://github.com/mluukkai/OtmTodoApp) tavoin
 
Seuraavien kohtien puutteet vähentävät pisteitä

- Tuntikirjanpito on ajantasalla
  - **Tuntien summan tulee olla merkittynä**
  - Tuntikirjanpitoon ei merkitä laskareihin käytettyä aikaa
- Repositorion README.md kunnossa
  - tiedosto on kurssin tämän vaiheen osalta relevantin sisällön suhteen samankaltainen  kuin [referenssisovelluksen](https://github.com/mluukkai/OtmTodoApp) README.md
  - kaikki ylimääräinen, mm. linkit laskareihin on poistettu 
- Repositorio siisti
  - ei ylimääräistä tavaraa (mm. hakemistoa target)
  - laskarit jätetään hakemiston _laskarit_ alle
  - järkevä .gitignore-tiedosto olemassa