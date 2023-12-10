---
Title: Load Analysis
Template: analysis
Description: Load Analysis
---

# Rapport om laddningstidsanalys
=======================

Uppgiften handlar om att analysera laddningstider och prestanda för tre utvalda webbplatser. 

Urval
-----------------------

Jag valde YouTube, Netflix och Amazon då dessa är hemsidor som jag använder regelbundet.

A1. https://www.amazon.com/<br>
A2. https://www.amazon.com/Kindle-Paperwhite-16-adjustable-Lockscreen/dp/B0B9YSHFJR/ref=sr_1_1?__mk_de_DE=%C3%85M%C3%85%C5%BD%C3%95%C3%91&crid=1PS0Q0JPPIA8G&keywords=kindle&qid=1702169124&sprefix=kindl%2Caps%2C205&sr=8-1&th=1<br>
A3. https://www.amazon.com/b/?_encoding=UTF8&ld=AZUSSOA-sell&node=12766669011&ref_=nav_cs_sell<br>
![amazon-bild](../assets/img/amazon-laddning.jpg)<br>


B1. https://www.youtube.com/<br>
B2. https://www.youtube.com/premium<br>
B3. https://www.youtube.com/feed/guide_builder<br>
![youtube-bild](../assets/img/youtube-laddning.jpg)<br>

C1. https://www.netflix.com/browse<br>
C2. https://help.netflix.com/legal/termsofuse<br>
C3. https://help.netflix.com/de/node/412<br>
![netflix-bild](../assets/img/netflix-laddning.jpg)<br>

Metod
-----------------------

För denna uppgift användes Google Sheets för att skriva ner resultat och Google Pagespeed samt Google devtools nätverksflik för att mäta laddningstid.

Resultat
-----------------------

<iframe class="sheet" src="https://docs.google.com/spreadsheets/d/e/2PACX-1vQjHomFrgvBw1xYSOMsSRE0sMaJWAMHAE8bpQP3rTfGtVNLtwpV5uykeKImz8x94X4FSHS4d1oMQJ3v/pubhtml?gid=0&amp;single=true&amp;widget=true&amp;headers=false"></iframe>

Netflix (C1) fick ett genomsnittligt betyg 52 på mobil och 77 på dekstop. YouTube (B1) fick betyget 33 på mobil och 42 på desktop. Amazon (A1) fick 54 på mobil och 72 på desktop.

När det gäller network-fliken i devtools så fick Netflix (C1) en genomsnittilg laddningstid på 3.36 sekunder, 24.37 MB resurser och 14.27 MB total överförd data. YouTube (B1) fick 5.78 sekunder, 18.53 MB resurser och 6.27 MB överförd data. Amazon (A1) fick 2.9 sekunder, 7.7 MB resurser och 5.4 MB överförd data.

Enligt pagespeed så kan Netflix minska på oanvänd JavaScript, speciellt på mobilversionen. Detsamma gäller YouTube mobilversion. För Amazon gäller bättre bildhantering, t.ex. hantering av osynliga bilder, bättre dimensionering av bilder, använda mer moderna format etc.

Analys
-----------------------

För YouTube och Netflix, vilka fokuserar mycket på videoinnehåll och liknande, så var den rekommendation som skulle ge absolut störst förbättring var att minska på oanvänd JavaScript. För Amazon så var det korrekt hantering av bilder som stod för absolut största förbättringsmöjlighet. För Netflix (C3) så var bättre hantering av bilder största källan till förbättring.

1. Amazon
2. Netflix
3. YouTube

Vid jämförelse av A1, B1 och C1 så presterade Amazon överlag bäst, förutom på pagespeeds desktop betyg där Netflix fick ett högre betyg. Netflix presterade bättre på laddningstid än YouTube men resurser och överförd data var större. Eftersom Netflix hanterar video och Amazon hanterar text och bilder så är det kanske svårare att optimera Netflix och YouTube i jämförelse.

Jag tänker mig runt 3 sekunder är accepterbart. Längre än så och då undrar jag om jag bör starta om min router eller liknande. Amazon klarar detta kriterie och Netflix klarar det nästan. YouTube klarar det å andra sidan inte. Å andra sidan när jag går in på sidorna och refreshar (inklusive cachad data) så tycker jag att samtliga sidor är snabba nog. 2 sekunder till på YouTube så hade jag nog känt annorlunda.

Referenser
-----------------------

pagespeed.web.deb
https://www.amazon.com/
https://www.youtube.com/
https://www.netflix.com/browse

Övrigt
-----------------------

William Matkaselkä skrev denna rapport.