# Tehtava5

# Keskeiset osat ja liitettävyys

## Homecontroller.cs
Tämä on keskeinen osa tuotetietojen käsittelyssä sekä lokitietojen käsittelyssä. Tällä luokalla on kaksi keskeistä metodia product() ja get products().
product() metodi kutsuu get products metodia joka hakee tuotetietoja wwwroot/product.json tiedostosta ja palauttaa näkymän tuotteet. Metodit yhdessä mahdollistavat totetietojen hakemisen ja esittämisen käyttäjille.

## products.json
Tämä on JSON-muotoinen tiedosto, joka sisältää tuotteiden tiedot, kuten nimi, hinta, kuvaus ja kuva. Tämän mallin avulla voidaan luoda ja käsitellä tuotteen tietoja ohjelmassa.

## Product.cshtml
Tämä on Razor-näkymä, joka vastaa tuotetietojen esittämisestä käyttäjälle. Se vastaanottaa IEnumerable<Product>-mallin, joka sisältää listan tuotteista, ja luo HTML-rakenteen jokaiselle tuotteelle.
Näkymässä käytetään @foreach-silmukkaa, joka käy läpi kaikki tuotteet ja luo niistä HTML-elementit, kuten kuvat, nimet, kuvaukset ja hinnat.
Tämä tiedosto yhdistää tiedot sekä määrittää miten ne näytetään käyttöliitymässä. 
<script src="~/js/site.js"></script> Tämä scripti liittää site.js tiedoston näkymään, ja siinä määritellyt JavaScript-funktiot parantavat tuotetietojen näyttämistä käyttöliittymässä.

## site.js
Tämä tiedosto sisältää js tiedoston joka parantaa tuotetietojen näyttämistä käyttöliittymässä. Tässä jouduin vaihtaa yhden funktion p tagia näyttämään toiseen ei neljänteen p tagiin, jotta hinnat näkyvät oikein käyttöliittymässä.

## cite.css 
Tämän tiedoston sisällön säännöt muokkaavat käyttöliittyymää kuinka tiedot näytetään käyttäjälle. 

## Yhteenveto
HomeController lukee tuotetiedot products.json-tiedostosta ja toimittaa ne Product.cshtml-näkymälle, joka näyttää ne korttimaisena asetteluna site.css-tyylien avulla. site.js-skripti viimeistelee ulkoasun ja muotoilun latauksen jälkeen, varmistaen, että tuotenimet ja hinnat esitetään johdonmukaisesti. Näin järjestelmä hakee, käsittelee ja näyttää tuotetiedot käyttäjälle.






