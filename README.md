
<h1>Laten we het weer eens checken</h1>
<hr>
<h3><i>Officieel de eerste landelijke tropische dag</i></h3>
<p>DE BILT (ANP) - De eerste landelijke tropische dag van het jaar is een feit. Om 14.40 uur werd het in De Bilt 30,7 graden, aldus Weeronline. <b>Het is eveneens de warmste 29 mei sinds de metingen in 1901 zijn begonnen.</b> Het oude dagrecord voor 29 mei stond op 30 graden en werd gemeten in 1944.
<p>De laatste keer dat het in De Bilt tropisch warm werd is ruim elf maanden geleden, op 22 juni vorig jaar.
<p>Het Gelderse Hupsel behaalde maandag al een plekje in de weer-recordlijst. Met 30 graden werd daar om 15.10 uur de eerste lokale tropische dag van 2018 behaald.
<p>Vorig jaar werd het op 27 mei voor het eerst tropisch in De Bilt. In 2016 was dat op 20 juli. De vroegste officiële tropische dag ooit was op 9 mei in 1976. 
<hr>
<br><br>
<p>Om te kunnen checken of het inderdaad de warmste 29 mei was sinds 1901, kunnen we terecht bij het KNMI: https://www.knmi.nl/nederland-nu/klimatologie/daggegevens
<br>
<ul>
  <li>Kies voor station De Bilt.
  <li>Sla het bestand op, unzip het en open het in Excel.
  <li>Je ziet dat het bestand uit twee delen bestaat: een serie beschrijvingen (metadata) en de daadwerkelijke data.
  <li>De metadata kun je het best op een apart tabblad opslaan.
  <li>De tabel met de data is gevormd als een csv: comma separated values. Die kunnen we netjes in kolommen plakken met 'gegevens->tekst naar kolommen'
  <li>Het datumveld is ingedeeld als 'jjjjmmdd'. Zo kun je het makkelijk sorteren, maar Excel herkent dit niet als datum. Met de functie DATUM kun je dit aanpassen.
  <li>Met 'beeld->blokkeren->titels blokkeren' kun je de regel- en kolomkoppen altijd zichtbaar houden.
  <li>De stappen tot nu toe zijn ook in <A HREF="https://github.com/ArlenPoort/excel2018/raw/master/KNMI002.xlsx">dit Excel-bestand</A> te vinden.
  <li>We kunnen het bestand een beetje opschonen, door overbodige kolommen op te ruimen. Beter is het om alles toch te bewaren, maar in een nieuw werkblad wijzigingen aan te brengen.
  <li>Je ziet ook dat het KNMI geen decimalen gebruikt in de temperaturen. 23,1 graad wordt geschreven als 231. Om het voor ons beter leesbaar te maken, kunnen we die kolommen aanpassen. Dan zie je ook dat er overbodige spaties in de kolommen staan.
  <li>Om het bestand toch een beetje handzaam te maken, heb ik <A HREF="https://github.com/ArlenPoort/excel2018/raw/master/KNMI003.xlsx">een nieuw Excel-bestand</A> gemaakt met alleen de relevante gegevens. 
  <li>In dit nieuwe bestand gaan we een draaitabel aanmaken. Als je het datumveld toevoegt aan het rijengebied, dan zie dat Excel uit zichzelf al iets bijzonders heeft gedaan, al hangt het van de versie op je eigen pc af wat er precies gebeurt. Het datumveld is gegroepeerd. Je kunt zelf bepalen hoe dit gebeurt door met je rechter muisknop op de data in kolom A te klikken. Als je dagen, maanden en jaren aanklikt en de rest uit, dan komen er drie datumonderdelen te voorschijn in het rijenvak rechts op je scherm. Die verschillende elementen kun je afzonderlijk naar aparte vakken slepen (filter, kolommen).
  <li>Door daarmee te spelen, kun je bijvoorbeeld een indeling maken met jaren als rijen, maanden als filter en dagen als kolommen. Als je dan filtert op mei, heb je een handig overzicht.
  <li>Dan kun je ook de waarden toevoegen aan de tabel: het veld Tmax naar waarden. Dan zie je dat er overal 1 komt te staan. Dat kun je aanpassen door te klikken op het pijltje->waardeveldinstellingen.
  <li>Nu zie je dat 29 mei 2018 inderdaad de warmste 29 mei was sinds het begin van de metingen. De max van 29 mei 2018 is namelijk gelijk aan de max van alle 29 mei's.
  <li>Maar voor wie de nuance zoekt: dat is niet het hele verhaal. Je kunt met bijvoorbeeld een voorwaardelijke opmaak snel ontdekken dat het op andere meidagen soms warmer is geweest. Vaak ook eerder in mei. Dus over een echt record kun je niet spreken. Dat zou je pas kunnen zeggen als het bijvoorbeeld nooit eerder in het jaar zo warm werd.
  <li>Er is <A HREF="https://github.com/ArlenPoort/excel2018/raw/master/KNMI004.xlsx">een versie van het bestand</A> beschikbaar inclusief de draaitabel en voorwaardelijke opmaak.
</ul>
<hr>
<h3>Rekenen aan hittegolven</h3>
<p>Met hetzelfde bestand kunnen we tal van andere berekeningen uitvoeren. Een voorbeeld is: hittegolven. Volgens het KNMI is er sprake van een hittegolf als het minimaal vijf dagen achtereen warmer is dan 25 graden. Bovendien moet het gedurende drie dagen warmer zijn dan 30 graden. Maar hoe herkent Excel een hittegolf? Hoeveel hittegolven zijn er sinds 1901 geweest? Hoe lang duurden ze? En komen ze vaker voor?
<p>Aan de hand van <A HREF="https://github.com/ArlenPoort/excel2018/raw/master/KNMI005.xlsx">dit bestand</A> worden al die vragen beantwoord.
<hr>
<br>
<h1>Een webservice gebruiken</h1>
Hiervoor gebruiken we dit bestand: https://github.com/ArlenPoort/excel2018/raw/master/excelAPI.xlsx
<br><br>

<h3>De coördinaten bij een adres zoeken, zodat je ze op een kaart kunt zetten</h3>
<p>Het Kadaster onderhoudt een zogeheten locatieservice, een zogeheten API. Daar kun je een verzoek naar sturen. En je krijgt een antwoord met de gewenste informatie. Meestal geven API's antwoord in de vorm van een xml- of json-document.
<p>Informatie over de dienst van het Kadaster staat hier: https://github.com/PDOK/locatieserver/wiki/Zoekvoorbeelden-Locatieserver

<br><br>

<p>Hoe XPath precies werkt staat hier uitgelegd: 
<br>https://www.w3schools.com/xml/xpath_syntax.asp

<br><br>
<h3>Hoe lang duurt een reis van A naar B?</h3>
<p>Documentatie over de Google Maps Distance Matrix API:
<br>https://developers.google.com/maps/documentation/distance-matrix/intro
<br><br>

<p>ht<i></i>tps://maps.googleapis.com/maps/api/distancematrix/
<br>xml
<br>?origins=
<br>[CELINHOUD]
<br>&destinations=
<br>Marten%20Meesweg%2035%203068AV%20Rotterdam
<br>&mode=transit
<br>&departure_time=1528439400
<br>&key=AIzaSyCzgtvqLFA2ExQ-eM20GXqWs7NAOPE4grQ
<br><br>
<p>De tijd/datum is 8 juni 2018, 8.30 uur (zie https://www.epochconverter.com/)


<br><br>
<hr><h3>Trump Tweets</h3>
<p>Het Trump Twitter Archive: https://github.com/bpb27/trump_tweet_data_archive
<p>Maar om json te kunnen laden, heb je wel Excel Power Query nodig. Meer info daarover: https://support.office.com/nl-nl/article/inleiding-tot-microsoft-power-query-voor-excel-6e92e2f4-2079-4e1f-bad5-89f6269cd605
