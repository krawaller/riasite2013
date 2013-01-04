När man på egen hand knåpar ihop applikationer är dokumentationskraven ofta låga eller obefintliga. I en grupp blir däremot dokumentationen livsviktig, både för **samarbete mellan programmerare** i stunden, men också för att göra det **enklare att underhålla koden**. I kursen så låtsas vi som bekant att vårt lilla projekt i själva verket är en jättelik kollaboration a là jQuery med massa inblandade, och att vi kommer behöva underhålla koden under lång tid framöver. Därför skall vi agera utifrån det även vad gäller löpande dokumentation av vår kod. Lite slarvigt kan man säga att **koddokumentation kan ske på 3 nivåer**; 

1.  **Övergripande** om hur koden används/hänger ihop
2.  **Kommenterad källkod**, vad gör de olika delarna. Ett vanligt verktyg här är Docco, som genererar dokumentation direkt från källkodsfilerna genom att lyfta ut kommentarerna och visa dem bredvid koden. Exempelvis [Backbones källkod][1] finns att tillgå på detta sätt (jämför med [källkodsoriginalet][2] så ser ni hur Doccoprincipen fungerar).
3.  **API-detaljnivå**, vilket i JavaScriptvärlden oftast innebär att vi använder JSDoc. Här dokumenterar vi detaljerat varje funktion - vilka argument den tar, vilka beroenden den har och vad den returnerar. Även nu lägger vi själva dokumentationen som kommentarer i källkoden och genererar dokumentationen utifrån det. En sådan genererad dokumentation kan se ut [så här][3].


Den första nivån kommer ni löpande göra via bloggen. Sedan får ni välja om ni vill fokusera på nivå 2 eller 3. Ni behöver inte köra båda, men minst en är obligatorisk.

Om ni väljer att köra kommenterad källkod (nivå 2), så vill vi att ni använder [Brocco][4]. Det är en fork av Docco som fungerar direkt i browsern (därav "Br"). Det innebär att ni kan ha dokumentationen som en del av själva appen, utan att själv behöva generera den. Ni kan se ett exempel av Brocco-implementation i [demoprojektet][6].

Vill ni hellre API-dokumentation (nivå 3) så kan ni använda onlinetjänsten [jsdoc.info][5]. Den kan automagiskt generera API-dokumentation utifrån ett Github-repositorium, förutsatt att den aktuella koden har JSDoc-kommentarer. Det enda ni då behöver göra är att länka till den genererade dokumentationen på jsdoc.info!

Oavsett lösning ni gäller så skall dokumentationen integreras i själva appen via en synlig länk/knapp/menyalternativ.

 [1]: http://backbonejs.org/docs/backbone.html
 [2]: https://github.com/documentcloud/backbone/blob/master/backbone.js
 [3]: http://jsxgraph.uni-bayreuth.de/docs/index.html
 [4]: http://toolness.github.com/brocco/
 [5]: http://jsdoc.info/  
 [6]: http://krawaller.github.com/riademo/