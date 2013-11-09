### Introduktion

Testdriven utveckling (på engelska TDD eller BDD (Test/Behaviour-Driven Development) är en speciell approach till utveckling - innan du kodar ny funktionalitet, så kodar du en funktion som testar ifall den nya funktionaliteten fungerar. Det gör den såklart inte, eftersom den ännu inte finns! Först nu, med testet på plats, så påbörjar du skapandet av den nya funktionaliteten. Testfunktionen som du kodade innan kommer visa dig när den nya funktionen fungerar som det är tänkt.

Kortfattat kan man säga att **testfunktionerna ersätter de manuella tester du utför för att se om din nya kod fungerade**. Utvecklar du inte testdrivet så kommer du, efter att ha lagt till ny kod, utföra någon manuell test (i konsolen eller i browsern) för att se att det fungerar som tänkt. Utvecklade du ett test först så räcker det att exekvera testet för att se att allting fungerar som det skall.

### Varför test?

Vid en första anblick kan testdriven utveckling verka ruggigt ineffektiv. Den innebär ju nästan att du kodar allting två gånger! Testen kan många gånger dessutom vara mer omfattande än koden den testar, vilket gör att de kräver en rejäl tidsinvestering.

Fördelarna är dock väldigt stora:

*    Den största fördelen är att test så att säga **låser ner** funktionalitet. Varje gång du körs testsviten så exekveras samtliga test, vilket gör att du märker om din nya kod gjorde att någon äldre funktion slutar fungera.
*    Att formulera testen tvingar dig att **fundera på din design**. Hur skall den nya funktionen utformas? Eftersom du skall skriva ett test så kommer du designa funktionen att vara så lättestad som möjligt, vilket innebär att den är så löst kopplad som möjligt, vilket innebär att den är väl designad!
*    Test kan också fungera som en **dokumentation**, eftersom de tydligt visar vad det förväntade utfallet är.

Att utveckla testdrivet är därför standard i moderna JavaScriptprojekt. Exempelvis Backbone och jQuery har båda gigantiska test suites, som säkerställer att till och med de ursprungliga funktionerna, som gjordes för flera år sedan, fortfarande fungerar. När någon via pull requests vill lägga till ny kod, så krävs det att den ackompanjeras av en uppdatering av testen!


### Vad skall testas?

Vissa saker är svårare att testa än andra, och för vissa saker har test mindre värde. Klart är att man inte alltid måste testa allt. Exempelvis användarinteraktioner kan vara lite luriga (dock fullt möjliga).

Det finns också en spridd inställning att Backboneapplikationer är svåra att testa, men här håller jag inte med. Man måste ibland tänka några steg extra - här är ett [blogginlägg][4] som kan hjälpa lite på vägen.


### TDD i kursen

Varje år funderar vi på om det skall vara obligatoriskt att använda TDD i kursen, men varje år - så även nu - så landar vi i att tiden inte riktigt är mogen än. Att designa kod väl är ett problem stort nog för en kurs, och är man inte van vid TDD så tar det för mycket fokus att sätta sig in i det tänket. Idealiskt vore att ha TDD-vana som ett förkunskapskrav för kursen, men alltför få andra kurser har TDD för att det skall vara realistiskt. Därför är testdriven utveckling fortfarande **frivillig**.

Om du väljer att utveckla testdrivet - vilket vi varmt rekommenderar - så innebär det att ditt projekt förmodligen inte blir lika omfattande som de andras. Detta är dig inte till nackdel på något sätt, då testen kommer vara en del av bedömningsunderlaget.

Kom också ihåg kravet på att hela applikationen skall kunna köras via Github Pages. Detta innefattar testsviten! Du kan därmed inte använda ett bibliotek som kör tester via exempelvis Node, utan endast de som erbjuder exekvering i en html-sida. Denna sida skall du länka till i projektet, precis som med den genererade dokumentationen.

Om du läser Daniel Tolls testkurs parallellt, så kommer det finnas möjlighet att låta kurserna klia varandra på ryggen.

### Resurser

Det finns en uppsjö av testbibliotek att använda. Vi rekommenderar [Jasmine][1], men det finns många fler. I [litteraturlistan][2] hittar du boken *Test-driven development in JS*, som är en riktigt bra bok som hjälper dig både med hur och varför.

På kurswebben för 2010-11 finns en [guide][5] som visar tänket bakom testning - visserligen med andra bibliotek, men kanske kan den ändå tjäna som primer.

[1]: http://tryjasmine.com/
[2]: https://coursepress.lnu.se/kurs/ria-utveckling-med-javascript/kurslitteratur/
[4]: http://blog.involver.com/2012/01/26/testing-backbone-js-best-practices-2/
[5]: http://voyager.lnu.se/tekinet/kurser/dtt/2DV407/index.php?sida=html%2Fresurser%2Fjspec
