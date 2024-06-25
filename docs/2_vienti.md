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

QGIS-projekti viedään seuraavaksi QField-projektiksi omaan puhelimeen. Voidaan ajatella, että QGIS-projektista tehdään kopio jonka QField-sovellus voi käyttää. QField-sovelluksessa kerätään tietoja ja tämän jälkeen viedään tietoja takaisin tietokoneelle QGISiin, missä voi muokata tietoja ja lopuksi voi viedä ulos tietoja QGISistä esimerkiksi taulukkomuotoon.