Nu är det äntligen dags att ta de första spadtagen till applikationen! Följande arbetsgång rekommenderas: 

1.  Börja med att närmare **definiera din applikationsidé** från förra kurssteget. Beskrivande meningar räcker inte - när bygget väl skall påbörjas så behöver vi vägledas av mer detaljerad information. Här i RIA-kursen kommer vi inte vara lika formella som i OOAD-kursen vad gäller formalia kring datamodeller och dylikt, så det är upp till dig hur du väljer att dokumentera din idé. Dokumentationen kan inkludera:
    *   Enkla **mockups** som visar flödet genom applikationen
    *   **Use cases** som beskriver funktionaliteten
    *   **Domänmodeller** och/eller **klassdiagram** (kanske via [yUML.me][1]). 
2.  Och så börjar vi gräva! Din applikation skall bo i ett repositorium på Github, så vi måste inleda med att skapa ett sådant. Det gör du genom att forka [mallrepositoriet][2]. Mallen innehåller inga filer, utan är ett sätt för kursledningen att enkelt ha överblick över kursdeltagarnas repositorier.
3.  När du har repositoriet på plats skall det fyllas med de **verktyg** du valt att använda:
    *   Backbone, Underscore och jQuery
    *   localStorage-plugin till Backbone
    *   Eventuell relations-plugin till Backbone
    *   Brocco, om du valt det som dokumentationslösning
    *   Testbibliotek, om du skall utveckla testdrivet
    *   RequireJS om det skall användas
    *   eventuellt Twitter Bootstrap eller annan UI-lösning
    *   kanske AsyncJS
    *   övriga favoritleksaker du vill använda
4.  Och så skall vi **hälsa på världen**! Lägg en grund till din applikation genom att initiera en app som skriver ut en välvald hälsningsfras. Detta skall inte göras i HTML-koden, utan du måste i detta steg ha en initierad Backbone-app som renderar en vy.
5.  Slutligen, i sedvanlig ordning, skall steget sammanfattas i ett **blogginlägg**.

 [1]: http://yuml.me/
 [2]: https://github.com/krawaller/riamall2013/  