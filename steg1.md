Nu är det äntligen dags att ta de första spadtagen till applikationen! Följande arbetsgång rekommenderas: 

1.  Börja med att **fundera över din applikationsidé**, alltså vad du skall bygga. Här i RIA-kursen kommer vi inte vara lika formella som i OOAD-kursen vad gäller formalia kring datamodeller och dylikt, så det är upp till dig hur du väljer att dokumentera din idé. Dokumentationen kan inkludera:
    *   Beskrivning i **klartext**
    *   Enkla **mockups** som visar flödet genom applikationen
    *   **Use cases** som beskriver funktionaliteten
    *   **Domänmodeller** och/eller **klassdiagram** (kanske via [yUML.me][1]). 
    *   **Kodstubbar** i repositoriet
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
5.  Slutligen, i sedvanlig ordning, skall steget sammanfattas i ett **blogginlägg**.

 [1]: http://yuml.me/
 [2]: https://github.com/krawaller/riaprojekt2013/ 
 [3]: https://coursepress.lnu.se/kurs/ria-utveckling-med-javascript/require/
 [4]: https://coursepress.lnu.se/kurs/ria-utveckling-med-javascript/sweet-js/
 [5]: https://coursepress.lnu.se/kurs/ria-utveckling-med-javascript/coffeescript/
 [6]: https://github.com/jeromegn/Backbone.localStorage
 [7]: https://gist.github.com/4450947
 [8]: https://coursepress.lnu.se/kurs/ria-utveckling-med-javascript/git-github/