
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
  
<br><br><br>

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
