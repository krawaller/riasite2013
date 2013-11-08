### Begrepp

Följande JavaScriptbegrepp bör vara bekanta: 

*   **Scope**, variablers synlighet i JavaScript
*   Hur scopes kan skapas via **closures**
*   **Context**, vad det är, hur den avgörs/påverkas/används
*   **Prototype chain**. Bra länk: [Prototypediskussion på DailyJS][1]

Ett bra sätt att se till att man är up to speed med dessa begrepp (som dessutom är obligatoriskt i [Steg 0][3]) är att gå igenom [Resig's Learn app][2]. Ni kan också slänga ett öga på [JS Scope Quiz][4].


### The Bad Parts

Likaså bör du vara familjär med de många "bad parts" som JavaScript också har. En genväg till det är att kika på [JavaScript Garden][5], som utgör en utomordentlig sammanfattning över "weird edge cases" i språket.


### Objekthantering

Du bör över huvud taget vara väldigt trygg med att hantera objekt i JavaScript. Ett hett tips, som hjälper denna resa på vägen, är att sätta dig in i det utmärkta biblioteket [Underscore][6]. [Backbone][13], som ni kommer använda i projektet, är beroende av Underscore, så ni kommer automagiskt ha tillgång till det. Ju bättre ni förstår Underscore, ju mer kommer ni kunna utnyttja det i projektet, och ju vassare kommer era JS-ninja-förmågor att bli!


### Funktionell programmering

Nästa steg är att lära sig utnyttja att JavaScript är ett **funktionellt programmeringsspråk**, vilket innebär att funktioner är första klassens medborgare och därmed kan utgöra värden i variabler och parametrar. Det gör bland annat att vi kan skicka in funktioner till moduler som de är beroende av, så kallar inversion of control.

En alldeles väldigt utmärkt artikel om funktionell programmering finns i [allra första numret av JSMag][14] (som dock kostar $5). Här får ni också länkar till ett antal bra presentationer:

*   [Christian Johansson @ Web Rebel 2012-07: pure, functional JavaScript][7]: Berör också asynkron programmering.
*   [Douglas Crockford @ YUI Theater 2010-02: Function the ultimate][9]: Klassiker, men fortfarande en väldigt bra föreläsning av mr Crockford.
*   [Jim Weirich @ Scotland JS 2012-06: adventures in functional programming][8]: Lite far out there, men ganska kul om man förlåter den lite väl akademiska approachen.

Men främsta resursen är Michael Fogus bok, [Functional JavaScript][16]. Ett utmärkt sätt att ta din JS-förståelse till nästa nivå!

### Asynkron programmering

I och med att JavaScript traditionellt utgör byggstenen i ett frontend som i sin tur måste tala med ett backend, så måste en hel del funktionalitet ske asynkront. Detta är inget problem då JavaScript är funktionellt, som sagts ovan, vilket gör att vi kan ha hänvisningar till funktioner som skall exekveras när serversvaret väl kommit åter (så kallade callbacks). 

Detta, och liknande, måste ni vara ganska trygga i. Det är ett lite speciellt tankesätt att sätta sig in i, framför allt om man kommer från en helt synkron värld som serversidan ofta är.

Boken [AsyncJS][15] av Trevor Burnham rekommenderas mer än varmt för den som vill gräva lite extra djupt i konsten att bemästra asynkron programmering i JavaScript.

Ni kan också med fördel titta närmre på [biblioteket med samma namn][10]. Välavvägd användning av detta bibliotek är ett mycket bra sätt att inkassera bonuspoäng i kursen! Projektet har ingen hemsida, men readme-filen på Github är väldigt utförlig.



 [1]: http://dailyjs.com/2012/11/26/js101-proto/
 [2]: http://ejohn.org/apps/learn "Learn app"
 [3]: http://coursepress.lnu.se/kurs/ria-utveckling-med-javascript/steg-1-kratta-manegen/ "Steg 0 – Kratta manegen"
 [4]: http://madebyknight.com/javascript-scope/
 [5]: http://bonsaiden.github.com/JavaScript-Garden/ "JavaScript Garden"
 [6]: http://underscorejs.org/ "Underscore"
 [7]: http://vimeo.com/43382919 "Christian Johansen @ Web rebel"
 [8]: https://vimeo.com/45140590
 [9]: http://www.youtube.com/watch?v=ya4UHuXNygM
 [10]: https://github.com/caolan/async "AsyncJS"
 [11]: http://www.amazon.com/Async-JavaScript-Trevor-Burnham/dp/1475247362
 [12]: https://leanpub.com/asyncjs  
 [13]: https://coursepress.lnu.se/kurs/ria-utveckling-med-javascript/backbone/
 [14]: http://www.jsmag.com/main.issues.description/id=1/
 [15]: http://www.amazon.com/Async-JavaScript-Trevor-Burnham/dp/1475247362
 [16]: http://blog.fogus.me/2013/03/20/fun-js/