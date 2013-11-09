Nu är det äntligen dags att ta de första spadtagen till applikationen! Följande arbetsgång rekommenderas: 

1.  Börja med att **fundera över din applikationsidé**, alltså vad du skall bygga. Här i RIA-kursen kommer vi inte vara lika formella som i OOAD-kursen vad gäller formalia kring datamodeller och dylikt, så det är upp till dig hur du väljer att dokumentera din idé. Dokumentationen kan inkludera:
    *   Beskrivning i **klartext**
    *   Enkla **mockups** som visar flödet genom applikationen
    *   **Use cases** som beskriver funktionaliteten
    *   **Domänmodeller** och/eller **klassdiagram** (kanske via [yUML.me][1]). 
    *   **Kodstubbar** i repositoriet

5.  Kursen är ganska fritt hållen, så utöver själva applikationsidén har du också en del andra **vägval** att göra. Som du har sett i kurspresentationen, Backboneinformationen och på andra ställen så finns ett antal stigar att följa: 
    *   Användning av [RequireJS][52] är obligatoriskt, men hur djupt du väljer att sjunka i det kaninhålet är upp tilld dig. Förståelse för modulproblematiken i JavaScript är central vid organisering av applikationer, och Require är bara en möjlig lösning, så för högre betygssteg är det viktigt att du inte bara fokuserar på RequireJS:s API, utan på den bakomliggande anledningen till att vi gör som vi gör.
    *   Läs på om [koddokumentering][53] och fundera på hur du vill göra.
    *   Kika på [Twitter Bootstrap][54] och se om du vill använda det. Om du redan är bekväm i annan, liknande lösning så är det helt ok att använda denna istället. Det är inget krav att använda ett "UI-hjälpmedel" över huvud taget, men det ger bonuspoäng att göra det.
    *   Fundera över om du vill använda **relationer** i Backbone, och hur dessa i så fall skall upprättas.
    *   Skall du använda Backbones [vanliga localStorage-modul][510], eller vågar du dig på den elakare [asynkrona versionen][59]?
    *   Kanske vill du göra din applikation [offline-säker][55]?
    *   En större fråga: vill du [arbeta testdrivet][56]? Detta beslut kommer ha ganska stor påverkan på hur du arbetar framöver. Tröskeln för att komma igång med testdriven utveckling kan vara ganska hög, men när man väl är över den så kommer du aldrig vända dig om. Om du ger dig på detta så måste du välja vilket bibliotek du skall använda för dina test.

        Notera också att det finns möjlighet till synergi med den parallella Test-kursen som Daniel Toll håller, ifall du går även den!
    *   Förmodligen har du hört talas om [CoffeeScript][57] - kanske är detta läget att prova, om du inte redan gjort det?

    När du bestämt dig för vilka stigar du vill utforska, dokumentera detta genom att titta igenom vapnen i [The armoury][9] i guilden, och använd **yearn**-kommandot på de som korresponderar mot dina val!

2.  Och så börjar vi gräva! Fyll på projektets repositorium med de **verktyg** du valt att använda:
    *   Backbone, Underscore och jQuery
    *   localStorage-plugin till Backbone (den [vanliga][6] eller den [elakare asynkrona][7])
    *   Eventuella övriga Backboneplugins såsom relationshanterare, Marionett, etc
    *   Brocco, om du valt det som dokumentationslösning
    *   Testbibliotek, om du skall utveckla testdrivet
    *   [RequireJS][3], tillsammans med eventuella plugins om du tänker testa exempelvis Jade eller [coffeescript][5]
    *   eventuellt Twitter Bootstrap eller annan UI-lösning
    *   kanske AsyncJS
    *   övriga favoritleksaker du vill använda

    Glöm inte att projektet skall publiceras på Github Pages, så du måste jobba i en gh-pages branch!

4.  Och så skall vi **hälsa på världen**! Lägg en grund till din applikation genom att initiera en app som skriver ut en välvald hälsningsfras. Detta skall inte göras i HTML-koden, utan du måste i detta steg ha en initierad Backbone-app som renderar en vy.

5.  Om du inte gjorde det redan förra veckan så måste du också se till att få ett introducerande **handledningspass** med David!

5.  Slutligen, i sedvanlig ordning, skall steget sammanfattas i ett **blogginlägg** som i sin tur annonseras med **complete**-kommandot i guilden.

 [1]: http://yuml.me/
 [2]: https://github.com/krawaller/riaprojekt2013/ 
 [3]: https://coursepress.lnu.se/kurs/ria-utveckling-med-javascript/require/
 [4]: https://coursepress.lnu.se/kurs/ria-utveckling-med-javascript/sweet-js/
 [5]: https://coursepress.lnu.se/kurs/ria-utveckling-med-javascript/coffeescript/
 [6]: https://github.com/jeromegn/Backbone.localStorage
 [7]: https://gist.github.com/4450947
 [8]: https://coursepress.lnu.se/kurs/ria-utveckling-med-javascript/git-github/
 [9]: http://krawaller.github.io/riacastle/#armoury

 [52]: https://coursepress.lnu.se/kurs/ria-utveckling-med-javascript/require/
 [53]: https://coursepress.lnu.se/kurs/ria-utveckling-med-javascript/dokumentation/
 [54]: https://coursepress.lnu.se/kurs/ria-utveckling-med-javascript/twitter-bootstrap/
 [55]: https://coursepress.lnu.se/kurs/ria-utveckling-med-javascript/offline-applikationer/
 [56]: https://coursepress.lnu.se/kurs/ria-utveckling-med-javascript/test-driven-utveckling/
 [57]: https://coursepress.lnu.se/kurs/ria-utveckling-med-javascript/coffeescript/
 [58]: https://coursepress.lnu.se/kurs/ria-utveckling-med-javascript/applikationsideer/  
 [59]: https://gist.github.com/4450947
 [510]: https://github.com/jeromegn/Backbone.localStorage/blob/master/backbone.localStorage.js
 [511]: https://coursepress.lnu.se/grupper/ria-utveckling-med-javascript-vt13/forum/topic/steg-1-vagval/
 [512]: https://coursepress.lnu.se/kurs/ria-utveckling-med-javascript/kodorganisering/