### Varför Backbone?

Den applikation som vi bygger i kursen kommer vila på kodbiblioteket **Backbone**. Meningen är egentligen inte att ni skall lära er just Backbone - det finns ett otal andra bibliotek som löser samma problem på ett fullgott sätt. Meningen är istället att ni skall *förstå problemet*. Det Backbone, och dess konkurrenter, gör är att de erbjuder en grundläggande **infrastruktur för kommunikation** i appen, och ett sätt att **hålla koden modulär**.

Det är vikigt att förstå att Backbone inte är ett fullfjädrat ramverk som exempelvis ExtJS och Ember. Tvärtom är det ett väldigt litet bibliotek, som tillhandahåller grundläggande funktionalitet men lämnar allt beslutsfattande om hur det skall användas till dig. Två Backbone-applikationer med liknande funktionalitet kan därmed ha väldigt olika källkod.


### Backbone i kursen

För att använda Backbone så inkluderar ni helt enkelt biblioteket i ert git-repo. Det finns dock en liten hake - om ni tänker [modularisera er kod via RequireJS][15] (vilket rekommenderas) så bör ni vara medvetna om att Backbone inte är AMD-kompatibelt, vilket gör att Backbone (kanske) inte direkt kan användas med RequireJS (se diskussion [här][4]). Läs mer på [Require-sidan][15] för att se vad som behöver göras.

Likt jQuery så har Backbone en plugin-struktur. Här är några som skulle kunna vara relevanta:

*   [Backbone.localStorage][18] är så gott som obligatorisk att använda. Den sparar din applikations modeller i localStorage, vilket gör att appen kan köras i browsern utan backend. Vill du kan du istället använda [min asynkrona version av pluginen][20], som är designad att vänta i 3 sekunder innan den svarar. Detta för att du skall tvingas till utmaningar i ditt UI och din kod.
*   [Backbone.rel][9] är en ganska lättviktigt och därmed lättanvänt relationsplugin.
*   [Backbone Relational][10] är mer avancerat men väldigt kraftfullt. Det har en [bra tutorial][11] som visserligen använder MongoDB, men allt är applicerbart även när man bara kör local storage.
*   Vill ni inte uttryckligen deklarera relationer i Backbone så kan ni kika på denna [blogpost][12] om att lösa det själv.

En mängd övriga plugins finns listade på [Backbones wiki][17].

Det finns också större ramverksaktiga byggen som vilar på Backbone. [Marionette][19] är ett sådant, som lägger på en hel del funktionalitet. Inget måste att använda, men väl värt en titt om ni är nyfikna! 


### Resurser

Ett rekommenderat första steg för att sätta sig in i Backbone är att helt enkelt printa ut den [kommenterade källkoden][13] och läsa den. Gärna med den [officella hemsidan][14] som bredvidläsning - den är väldigt välskriven, och innehåller både API-detaljer och användningsråd.

På [bokfronten](https://coursepress.lnu.se/kurs/ria-utveckling-med-javascript/kurslitteratur/) så rekommenderas [Addy Osmanis Backbonebok](https://github.com/addyosmani/backbone-fundamentals/blob/gh-pages/index.md), som ni kan läsa gratis online. Det finns också ett kapitel om Backbone i [JavaScript Web Applications][2]. E-boken [Recipes for Backbone][3] kommer också varmt rekommenderad.

Det finns en uppsjö av övriga Backbone-resurser på nätet. Här kommer ett litet axplock:

*    [Videotutorial][6] av Nick Gauthier
*    Siten [Backbone Patterns][7]
*    Siten [Backbone Tutorials][8]
*    [Backboneavsnitt][16] av JavaScript Jabber (dock mycket fokus även på Ember)

För fler tips kan ni också slänga ett öga på tidigare års kurswebbar för denna kurs!



 [1]: https://github.com/addyosmani/backbone-fundamentals/blob/gh-pages/index.md "backbone-fundamentals"
 [2]: http://shop.oreilly.com/product/0636920018421.do "JavaScript Web Applications"
 [3]: http://recipeswithbackbone.com/
 [4]: https://github.com/documentcloud/underscore/commit/0d4b1247c45083c695cab4242c084a97aa600221#commitcomment-857644
 [5]: https://coursepress.lnu.se/kurs/ria-utveckling-med-javascript/require/
 [6]: https://www.youtube.com/watch?v=PqtYcHyyWJA
 [7]: http://ricostacruz.com/backbone-patterns/
 [8]: http://backbonetutorials.com/
 [9]: https://github.com/masylum/Backbone.Rel
 [10]: https://github.com/PaulUithol/Backbone-relational
 [11]: http://antoviaque.org/docs/tutorials/backbone-relational-tutorial/
 [12]: http://slashhashbang.com/2011/10/lightweight-relation-modeling-with-backbone/  
 [13]: http://backbonejs.org/docs/backbone.html
 [14]: http://backbonejs.org/
 [15]: https://coursepress.lnu.se/kurs/ria-utveckling-med-javascript/require/
 [16]: http://javascriptjabber.com/004-jsj-backbone-js-with-jeremy-ashkenas/
 [17]: https://github.com/documentcloud/backbone/wiki/Extensions%2C-Plugins%2C-Resources
 [18]: https://github.com/jeromegn/Backbone.localStorage
 [19]: http://marionettejs.com/
 [20]: https://gist.github.com/4450947