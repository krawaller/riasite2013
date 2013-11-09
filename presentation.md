### Introduktion

Kursen RIA-utveckling med JavaScript syftar till att lära ut best-practices gällande just RIA-utveckling med JavaScript. Detta görs genom att - you guessed it - **bygga en RIA** (Rich Internet Application) i JavaScript! Dessa publiceras sedan på webben via Github Pages, och också på mobila plattformar via Phonegap.

Den största delen av kursen handlar om detta bygge. Fokus är inte på målet utan på **processen**. Applikationens omfattning kommer därför vara något mindre än vad ni kanske är vana vid från andra kurser, just för att ge plats åt påläsning, reflektion och diskussion angående metodiken i bygget.

Även om omfattningen på projektet är liten så kommer vi dock arbeta som om detta vore ett **stort projekt** med många kollaboratörer, som skall underhållas över lång tid. Därför skall vi under byggets gång använda verktyg och metoder som man gör i dylika projekt. Vi kommer alltså använda bibliotek och arbetssätt som är vanliga ute i det vilda. Exempelvis kommer ni bygga projektet med hjälp av ramverket **Backbone**, och hosta koden på **Github**.

Under arbetets gång kommer du dokumentera vad du gör i en **blogg**. Denna blogg tjänar tre olika syften - den...

*    dokumenterar för dig själv vad du gör
*    underlättar för dina kurskamrater lättare att sätta sig in i ditt projekt vid kollaboreringsstegen
*    tjänar som betygsunderlag för lärare.

Genom kursen kommer ni ha regelbunden **handledning** av lärare, just för att hålla diskussionen levande. JavaScript är ett ovanligt dynamiskt och expressivt språk vilket gör det väldigt kraftfullt, men samtidigt också mindre självklart hur applikationer bäst konstrueras och kod organiseras. Ni uppmuntras att utnyttja tillfällena till handledning så mycket som möjligt. Kursen innebär ett stort eget ansvar, men det är inte liktydigt med att stöttning saknas! Handledningen är en stor resurs i både projektandet och lärandet.

Ni kommer också få tillfällen att **diskutera med varandra**, både generellt på kursens forum men också mer direkt via **kollaborering** i varandras projekt.

Ni kommer också dokumentera era göranden i [The JavaScript Guild][5], där jag kan ha koll på er och ni på varandra!

Kursen avslutas med en **djupdykning** i någon av de tekniker eller teknologier ni använt i er applikation. Denna djupdykning resulterar sedan i en **presentation** som alla kursdeltagare kan ta del av. 

Förhoppningen är att detta sammantaget kommer ge en god bild av vad det innebär att **strukturera applikationer i JavaScript**!

### Förkunskapskrav

Följande kurser, alternativt motsvarande kunskaper, utgör förkunskapskraven för RIA-kursen: 

*   [Webbteknisk introduktion][1]: Att vara trygg i **HTML och CSS** är ett absolut måste. Inget utrymme ges för att sätta sig in i dessa tekniker, utan omfattande förkunskaper förutsätts.
*   [Webbteknik I][2]: Likaså krävs en god befintligt grund i **JavaScript och DOM-manipulering**. Denna kurs lär inte ut JavaScript, utan utgår ifrån att du redan från början har goda kunskaper.
*   [Inledande programmering med C#][3]: RIA-kursen förutsätter en förståelse för **objektorienterad programmering**, vilket ges i C#-kursen.
*   [ObjektOrienterad Analys &amp; Design (OOAD)][4]: Även om vi i RIA-kursen inte är alltför formella vad gäller **UML-terminologi** och liknande, så förutsätts du ha tillgodogjort dig de bakomliggande filosofierna angående hur en domain model definieras och hur design patterns tillämpas.


### Betygsättning

I och med att kursen har ganska lösa tyglar så blir betygsnivåerna diffusa. Givetvis kommer generell kvalitét i vad du gör väga tyngst. Likväl så vill vi lyfta fram ett antal tillfällen att visa framfötterna:

*   **Kvalitét i bloggandet** utgör en god grund för högre betyg! Det betyder inte att vi kommer rätta med linjal, men att det går lätt att följa arbetsprocess och tankegång i vad du skriver.
*   Utnyttja **twitter bootstrap** (eller andra importerade verktyg) väl. Så gott som alla hjul är uppfunna, så att kunna tillgodogöra sig externa resurser på ett effektivt sätt är A och O.
*   Bli en **Backbone ninja**! Genom att använda Backbone väl så kommer du få en djupare förståelse för problemområdet, och därmed bli bättre på att utnyttja även andra liknande resurser.
*   Pröva på att utveckla **testdrivet**. Det kan vara en hög tröskel att komma igång med, men när du väl är över den så kommer en hel del av det nyttiga organisationstänket att bli automatiserat.
*   Nyttja **avancerade Git-funktioner**. I kursen använder vi endast de mest grundläggande funktionerna, men Git är otroligt kraftfullt. Att utforska möjligheterna här är ännu ett sätt att samla guldstjärnor.
*   Modulhantering med **RequireJS** är ett bra sätt att dopa sin kodorganisering. Om du dessutom tittar lite närmare på RequireJS mer avancerade möjligheter så är detta ett ypperligt sätt att imponera på lärare.
*   Tillämpa **design patterns** uttryckligt! Om du i dokumentation och bloggande använder den vedertagna terminologin och kan diskutera patterns direkt, så lyfter det genast till en högre nivå.
*   Gör en riktigt bra **fördjupning**. Omfattningen behöver inte vara stor, men det skall märkas att du lagt ned den tillbörliga tiden. För högre poäng här uppmanas ni att _inte_ förklara API:er i detalj, utan fokusera på att diskutera användningsområden, för och nackdelar, etc.
*   Kvalitativa **pull requests**. Om du på ett framgångsrikt sätt sätter dig in i andras kodbaser och bidrar till deras projekt, så skjuter din poängmultiplier snabbt i höjden!
*   **Investera tillräcklig tid**! I och med att projektet är ovanligt litet för en 7.5-poängskurs om man tittar på slutresultatet, och en hel del tid är avsatt för påläsning, så kan det vara frestande att tro sig komma undan med att lägga ganska lite tid och investera blott en bråkdel av sitt hjärta. Detta kommer direkt slå igenom i slutresultatet.
*   Utnyttja **handledningen**! Den är ett tillfälle att föra diskussioner med lärare om ditt projekt, vilket ger dig möjlighet att visa kvalitét i dina tankegångar som kanske inte alltid är lätt att få fram i bloggtexterna.
*   Viktigast av allt är **organiseringen av din kod** i projektet, vilket ju utgör kursens huvudsakliga existensberättigande. En genomtänkt, välarbetad kodorganisation är en förutsättning för högre betyg (och näst intill också för att komma över ribban).




 [1]: https://coursepress.lnu.se/kurs/webbteknisk-introduktion/ "Webbteknisk introduktion"
 [2]: http://voyager.lnu.se/tekinet/kurser/dtt/wp_webbteknik/index.php "Webbteknik I"
 [3]: https://coursepress.lnu.se/kurs/inledande-programmering-med-csharp/ "Inledande programmering med C#"
 [4]: http://voyager.lnu.se/tekinet/kurser/Dtt/DT2380/ "OOAD"
 [5]: http://krawaller.github.io/riacastle/