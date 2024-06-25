# Alkuvalmistelut

- Asenna itsellesi tietokoneelle [QGISin viimeisin vakaa versio (LTR)](https://qgis.org/fi/site/forusers/download.html).
- Asenna puhelimeesi [QField-sovelluksen sovelluskaupastasi](https://qfield.org/).
- Lataa GeoPackage-tiedosto [täältä](https://drive.google.com/file/d/1OJ9KtAqWKQuaK5Cl08BDRTUrdqtmAsgr/view?usp=sharing).

## Projektin lavaaminen
GeoPackage-tiedosto sisältää QGIS-projektin, sekä kaikki tarvittavat tasot ja taulukot. Avaa QGIS tietokoneellasi ja raahaa lataamasi GeoPackage-tiedosto QGIS-ohjelmaan. Kun päästät irti tiedostosta niin uusi ikkuna aukeaa. Valitse tästä ainoastaan *QField-pilotti-projekti* (kuten kuvassa). Silloin QGIS avaa projektin sinulle suoraan, tasot ovat valmiiksi kytketty projektiin, joten tämän takia niitä ei lisätä erikseen.

![Projektin avaaminen GeoPackagesta](img/Projektin_avaaminen_geopackagesta.png)

## Lisäosan asentaminen
Jos et ole aiemmin asentanut QGISin lisäosan "QField Sync" niin tee se nyt. Jos et ole varma miten lisäosia lisätään voit katsoa seuraavan videon.

![QField Sync lisäosan asentaminen](img/asenna_qfield_lisaosa.gif)

Tässä kuvassa näet miltä projekti näyttää oletusasetuksilla. 

![QGIS-projekti](img/projektinakyma.png)

**Tasot**-näkymässä näet, seuraavia tasoja

| Taso | Muoto | Selite |
|----------|----------|----------|
| Pääkohde| Piste| Jokaisella inventointikohteella on ainoastaan yksi pääkohde|
| Alakohteet | Piste| Pääkohteilla voi olla useampia alakohteita. Alakohde liittyy aina yhteen pääkohteeseen|
| Alue | Polygoni| Pääkohteilla pitäisi aina olla jokin aluemainen geometria myös, mikä piirretään tälle tasolle|
| Valokuvat| Taulukko| Pääkohteilla ja alakohteilla voi olla liittenä valokuvia, tiedostopolku valokuviin tallennetaan tähän taulukkoon|

Ryhmässä "Koodistot" on myös taulukkotasoja, mutta nämä ovat stattisia tauluja, mistä haetaan tietoja yllä oleviin tasoihin, joten näihin ei kannata koskea. 

## Taustakartan lisääminen
Jos haluat jotain tiettyjä taustakarttoja tai muita tasoja mukaan projektiin niin lisää ne tässä vaiheessa. Taustakartta on oletuksena OpenStreetMap, mutta tämä tulee varmaan useimmiten muokata jokskin muuksi. Lisää taso jonka haluat taustakartaksi ja avaa projektin ominaisuudet (Projekti-> Ominaisuudet -> QField). Valitse "Cable export"-välilehti. Näet "Base map"-osion missä voi valita taustakarttatasoa. Alla olevassa kuvassa tämä on OpenStreetMap niin voit vaihtaa sen. Voit esimerkiksi tarvita ilmakuvan, silloin vaihdat siihen ilmakuvatason. Tarkista myös, että "Base map"-osion yläpuolella, missä on listattuna tasot, niin oma ilmakuvasi "Action" on asetettu "Copy"-tilaan, milloin tiedostoa kopioidaan mukaan QFieldiin, eli voit käyttää tasoa myös ilman verkkoyhteyttä. Muista tallentaa projektia lopuksi.

![Projektin ominaisuudet](img/Projektin_ominaisuudet.png)

QGIS-projekti viedään seuraavaksi QField-projektiksi omaan puhelimeen. Voidaan ajatella, että QGIS-projektista tehdään kopio jonka QField-sovellus voi käyttää. QField-sovelluksessa kerätään tietoja ja tämän jälkeen viedään tietoja takaisin tietokoneelle QGISiin, missä voi muokata tietoja ja lopuksi voi viedä ulos tietoja QGISistä esimerkiksi taulukkomuotoon.