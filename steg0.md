I detta prequel-steg skall vi kratta manégen inför kursen. Det innebär följande:


1.  **Introduktion:** Sätt dig in i kursen genom att läsa igenom kurswebben. Du behöver inte memorisera allt, men se till att ge lite uppmärksamhet till [presentationen][12] och kursstegen.
1.  **Blogg:** Arbetet under kursens gång redovisas via en blogg. Om du har en befintlig blogg är det helt ok att använda den (ett villkor är dock att den har kommentarsfunktion, så statiska sidor är ej godkänt). Inför gärna en unik tagg (typ "RIA") som gör det lätt att hitta de kursrelaterade inläggen. Om inte har någon blogg så måste du skapa en. Kolla på sidan om [enkelt bloggupplägg][1] under Resurser.
2.  **Githubkonto:** Koden du skriver i kursen kommer bo i ett repositorium på Github. Om du inte redan har ett konto där så måste du upprätta ett! Det krävs också att du har versionshanteringssystemet Git installerat på din dator (om du inte enbart jobbar i molnet via [C9][2]). Kolla in [Git &amp; Github][3] under Resurser för mer information. Har du inte jobbat med Git förut så rekommenderas det att du lägger tid på att läsa in dig. När du skapat ett konto så skall du också skapa ett tomt repositorium, som kommer vara bostad för applikationen du skall bygga i kursen.
4.  **Utvecklingsmiljö:** Om du inte redan har en bra editor för JavaScriptutveckling så är det av stor vikt att du investerar tid i att hitta en sådan och bli bekväm med den. Hur avancerad den skall vara är helt upp till dig, men det är obligatoriskt att ha tillgång till [JSLint][5]/[JSHint][6] eller liknande.
5.  **JavaScript refresher:** Kolla igenom [Avancerad JavaScript][7] under Resurser, och säkerställ att du är up to speed med allting som nämns där. Förmodligen har du koll på det allra mesta sedan tidigare kursen. [John Resig's Learn App][8]&nbsp;är obligatorisk att gå igenom! Läs också på om [kodkvalitét][9] och [kodorganisering][10].
5.  Du behöver också göra en tidsinvestering på att **sätta dig in** i [Backbone][16]. Beroende på hur mycket förkunskaper du har så kommer detta ta olika lång tid, men det är av vikt att du inte slarvar här! Kursen i sig handlar egentligen inte om Backbone utan om organisering av JS-applikationer, men det är Backbone vi kommer använda både för att förstå och lösa problemet.
5.  Kursen är ganska fritt hållen, så du har en del **vägval** att göra. Som du har sett i kurspresentationen, Backboneinformationen och på andra ställen så finns ett antal stigar att följa: 
    *   Användning av [RequireJS][52] är obligatoriskt, men hur djupt du väljer att sjunka i det kaninhålet är upp tilld dig. Förståelse för modulproblematiken i JavaScript är central vid organisering av applikationer, och Require är bara en möjlig lösning, så för högre betygssteg är det viktigt att du inte bara fokuserar på RequireJS:s API, utan på den bakomliggande anledningen till att vi gör som vi gör.
    *   Läs på om [koddokumentering][53] och fundera på hur du vill göra.
    *   Kika på [Twitter Bootstrap][54] och se om du vill använda det. Om du redan är bekväm i annan, liknande lösning så är det helt ok att använda denna istället. Det är inget krav att använda ett "UI-hjälpmedel" över huvud taget, men det ger bonuspoäng att göra det.
    *   Fundera över om du vill använda **relationer** i Backbone, och hur dessa i så fall skall upprättas.
    *   Skall du använda Backbones [vanliga localStorage-modul][510], eller vågar du dig på den elakare [asynkrona versionen][59]?
    *   Kanske vill du göra din applikation [offline-säker][55]?
    *   En större fråga: vill du [arbeta testdrivet][56]? Detta beslut kommer ha ganska stor påverkan på hur du arbetar framöver. Tröskeln för att komma igång med testdriven utveckling kan vara ganska hög, men när man väl är över den så kommer du aldrig vända dig om. Om du ger dig på detta så måste du välja vilket bibliotek du skall använda för dina test.
    *   Förmodligen har du hört talas om [CoffeeScript][57] - kanske är detta läget att prova, om du inte redan gjort det?

6.  **Blogginlägg:** Alla kurssteg redovisas med (minst) ett blogginlägg. Nu är det dags att skriva kursens första! Ta med...
    *   en **presentation** av dig själv
    *   din **erfarenhet av JavaScript**, med en kommentar till John Resigs Learn-app - hade du full koll sedan tidigare, eller fick du nya kunskaper?
    *   vilka **JavaScriptresurser** du nyttjar. Har du köpt någon/några av böckerna på litteraturlistan? Några siter du vänder dig till?
    *   dina **förhoppningar** på kursen
    *   hur din **utvecklingsmiljö** ser ut. Vilken editor använder du? Plugins? Build tools? Bonus om du som en förberedelse för kursen vidtar åtgärder för att vässa din miljö ytterligare, lista i så fall dessa åtgärder också! Det kan innebära att byta editor, eller bemästra din gamla ännu lite mer (kortkommandon, effektiviserande plugins, etc).
    *   de **vägval** du (preliminärt) gjort. Detta huggs inte i sten så givetvis är det fritt fram att ändra sig senare, men, vi vill ändå att du ger en första redogörelse redan nu över hur du tänker!

    När du har skrivit ditt inlägg, länka till det i den korresponderande [tråden i forumet][13]!

7.  **Handledning:** Du rekommenderas också försöka få till ett första handledningspass med David. Det är inte ett supermåste att göra under denna vecka, men gör du det inte nu så måste du göra det under nästa steg!

7.  **Deltagarlistan:** Nu i höst så kommer vi ha koll på varandra via [The JavaScript Guild][14], där du som en del av detta steg skall bli medlem. Se närmre på [resurssidan][15] för hur du går till väga för att komma med! En del av datan du måste föra in (projektinfo och fördjupningsval) kommer du förmodligen inte ha bestämt ännu, skriv bara något tillfälligt här så länge. Sammantaget, i detta steg, så skall du..
    *    Registrera dig själv
    *    Utföra "join"-kommandot
    *    Utföra "complete"-kommandot på "phase0", som motsvarar detta kurssteg.

 [1]: http://coursepress.lnu.se/kurs/ria-utveckling-med-javascript/enkelt-bloggupplagg/ "Enkelt bloggupplägg"
 [2]: http://coursepress.lnu.se/kurs/ria-utveckling-med-javascript/cloud9-editor/
 [3]: http://coursepress.lnu.se/kurs/ria-utveckling-med-javascript/git-github/ "Git &amp; Github"
 [4]: https://github.com/krawaller/riadeltagare2013/
 [5]: http://www.jslint.com
 [6]: http://www.jshint.com
 [7]: http://coursepress.lnu.se/kurs/ria-utveckling-med-javascript/asynchronous-javascript/ "Avancerad JavaScript"
 [8]: http://ejohn.org/apps/learn "Learn"
 [9]: https://coursepress.lnu.se/kurs/ria-utveckling-med-javascript/kodkvalitet/
 [10]: https://coursepress.lnu.se/kurs/ria-utveckling-med-javascript/kodorganisering/ 
 [11]: https://coursepress.lnu.se/kurs/ria-utveckling-med-javascript/steg-2-hello-world/
 [12]: https://coursepress.lnu.se/kurs/ria-utveckling-med-javascript/om/
 [13]: https://coursepress.lnu.se/grupper/ria-utveckling-med-javascript-ht13/forum/topic/steg-0-kratta-manegen-1/
 [14]: http://krawaller.github.io/riacastle/
 [15]: https://coursepress.lnu.se/kurs/ria-utveckling-med-javascript/guilden/
 [16]: https://coursepress.lnu.se/kurs/ria-utveckling-med-javascript/backbone/


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