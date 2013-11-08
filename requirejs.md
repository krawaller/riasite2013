###Introduktion

[RequireJS][11] är ett bibliotek som erbjuder **modulhantering** i JavaScript. Det är ett väldigt avancerat bibliotek, men det viktigaste är att det implementerar de två globala funktionerna `define` och `require`. Med hjälp av dessa kan vi deklarera moduler och ladda in andra moduler vi är beroende av, istället för att lagra allt i det globala objektet. Se [sidan om kodorganisering][7] för mer diskussion kring problemdomänen.



###Modulstandarder

Det finns ett otal idéer om hur moduler skulle kunna implementeras i JavaScript. De två vanligaste (I think) är **AMD** och **CommonJS**. AMD är den standard som RequireJS bygger på, och CommonJS är implementerat i Node. För en utmärkt genomgång av likheterna och skillnaderna mellan dessa två, kolla in [John Hanns föreläsning][2] från [JSEverywhere2011][3]. De slides han använder i presentationen finns online [här][4] (de syns lite dåligt ibland i videon).

I **EcmaScript Harmony** (nästa generations JavaScript) så finns också [planer på en modulstandard][6].


###RequireJS i kursen

Som ni såg på [kodorganiseringssidan][7] och i [steg 1][8] så är det helt frivilligt att använda RequireJS. Om ni väljer att göra det så vill vi ge er några tips på vägen:

*    RequireJS är, som sades i inledningen, ett **väldigt avancerat** bibliotek. Vi vill därför påpeka samma sak som apropå Backbone - målet är att ni skall förstå problemet (modulhantering), inte att ni skall bli experter på just RequireJS. **Gräv därför inte ned er för djupt!** Om ni inte vill, förstås. :)
*    Det kan vara lite lurigt att använda **AMD-moduler parallellt med "vanliga" JavaScriptfiler**. Det finns lite förenklat två olika lösningar på detta:

    1.    man kan **stöpa om alla filer** så att de verkligen blir AMD-moduler. Exempelvis finns jQuery, underscore och Backbone i [AMD-varianter][1].
    2.    man kan **acceptera att ha vissa yttre beroenden** (såsom Backbone osv) som vanliga globala variabler, och bara modularisera sin egen kod. Detta är helt ok. Välj alternativ 1 endast om ni verkligen vill komma in i RequireJS.
*    RequireJS innehåller också en **optimerare**, som man kör för att göra sina filer produktionsredo. Den minifierar all JavaScript, och konkatenerar allt till en enda fil (vilket den kan göra eftersom alla beroenden är definierade). Detta kan ni helt strunta i inom ramen för kursen, om ni inte är väldigt sugna på att sätta er in i hur den används.



###Resurser

Förutom [John Hanns föreläsning][2] som nämndes ovan (och [RequireJS officiella hemsida][11]) så tänker jag bara ge er en enda länk, nämligen Addy Osmanis artikel [Writing modular JavaScript][5]. Den utgör **riktigt bra läsning**, så om ni bara tar er tid att plöja den så tror vi att ni är på god väg sedan.

För att komma igång kan ni också slänga ett öga på [kursens demoprojekt][9], där RequireJS används. Det innehåller också en setup med RequireJS och Jasmine, vilket kan vara av intresse för er som samtidigt kör [testdrivet][10]. 



 [1]: https://github.com/amdjs
 [2]: http://www.everytalk.tv/talks/913-JSEverywhere-AMD-vs-CommonJS
 [3]: http://2011.wakanday.org/
 [4]: http://unscriptable.com/code/AMD-vs-CommonJS/
 [5]: http://addyosmani.com/writing-modular-js/
 [6]: http://wiki.ecmascript.org/doku.php?id=harmony:modules
 [7]: https://coursepress.lnu.se/kurs/ria-utveckling-med-javascript/kodorganisering/
 [8]: https://coursepress.lnu.se/kurs/ria-utveckling-med-javascript/steg-1-vagval/
 [9]: https://github.com/krawaller/riademo
 [10]: https://coursepress.lnu.se/kurs/ria-utveckling-med-javascript/test-driven-utveckling/
 [11]: http://requirejs.org/