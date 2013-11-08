Så har vi kommit till kursens absoluta kärna: **kodorganisering**. Flexibiliteten i JavaScript är extremt kraftfull, men den gör också att man kan göra mycket dummare saker än i många andra språk, framför allt vad gäller organisering i och med JavaScripts modell med globala objekt.

Lite forcerat kan man dela in kodorganiseringskoncepten på **fyra olika nivåer**:

*    Utformning av enskilda satser och uttryck - **kodstil**, helt enkelt.
*    Använding och organisering av enskilda **funktioner**. Här kommer vi lägga mest krut.
*    Organisering av **moduler** och filer. Med andra ord alternativ till att bara slänga in allt i det globala objektet.
*    **Kopplingar** mellan objekt och moduler. 


###Kodstil

Det finns lika många kodstilar som programmerare, och många gånger inget rätt eller fel. Skall vi använda mellanslag eller tabbar för indentering? Hur många mellanslag? Deklarera alla variabler högst upp i varje scope? Camel-case-namngivning? Indikera interna variabler med inledande understreck i namnen? Inga rätt eller fel, som sagt, men det viktiga är att man är **konsekvent**. Kod som byter stil fram och tillbaka blir väldigt svår att läsa.

Saker och ting blir ännu svårare när man är flera personer i ett projekt. Hur kan man vara **konsekvent som grupp**? Klart är att det inte är något som händer av sig själv. Stora företag och opensource-projekt har därför ofta stilguider som alla inblandade förväntas följa. Att vara konsekvent när man är ensam om ett litet projekt, som i fallet i denna kurs, är inga problem. Men nu skall vi som sagt låtsas att vi är Google, just för att lära oss best practices i stora JS-projekt. Därför skall du i [steg 1][6] fundera igenom just detta. Hur skall kodstilen i ditt projekt se ut?

Här är några bra resurser: 

*    Zakas bok [Maintainable JavaScript][2]
*    Den communitydrivna siten [Idiomatic JavaScript][3]
*    [Google's JavaScript Style Guide][4]
*    Föreläsning av Crockford på YUIconf 2011-03: [JavaScript and your brain][5]
*    Det finns också lite kodstilstester i JSHint, som jQuery-kändisen Elijah Manor har [skrivit om][7].


###Funktioner

Hjärtat i ett JavaScript-projekt är **funktionerna**. Därför är det av största vikt att de är genomtänkta och lätthanterade. En stor del av bedömningen av din kod kommer fokusera på kvalitén i ditt funktionsanvändande. Här är ett antal punkter att ha i åtanke:

*    Det skall vara **tydligt vad en funktion gör**. Namnet bör därför väljas med omsorg.
*    En funktion skall vara expert på **en enda sak**. Om du har en funktion med alltför många statements - slå sönder den i fler funktioner. En bra regel är "at-a-glance test" - om det inte går att med blotta ögonkastet förstå vad en funktion gör, då är den alltför komplicerad och bör delas upp.
*    En funktion skall ha **tydligt definierade beroenden**. Det finns tre sätt att använda yttre data i en funktion:

     1.    Via **funktionsparametrar**. Detta är det vanligaste, och ofta bästa, sättet.
     2.    Via **kontexten**, det vill säga användning av `this`. Även detta kan vara en fullgod lösning, men ställer ofta högre krav på genomtänkt använding.
     3.    Via **scopevariabler**, alltså variabler som existerar i samma scope (eller i den globala kontexten). Detta är ofta en väldigt dålig idé, eftersom det gör funktionen hårt knuten till just detta scope och därmed svår att återanvända och testa. Med möjligt undantag av vissa projektglobala variabler såsom `Backbone` och `jQuery` så medför användning av globala objekt mycket dålig karma i kursen. Om du någonstans är frestad att använda scopevariabler - kolla om du inte kan skicka in dem som argument till en parameter istället!

     Om det är otydligt vilka resurser en funktion använder så bör detta förtydligas med kommentarer.
*    En funktion skall ha **genomtänkta effekter**. Dessa kan delas in i ett antal kategorier:

     1.   Det bästa är om en funktion helt **saknar effekter**, en så kallad *pure function*. En sådan funktion jobbar endast med returvärde, och påverkar ingenting i övrigt. Det gör den lätt att återanvända och testa. Förvånansvärt många funktioner kan via smart applikationsdesign omvandlas till pure functions!
     2.   En funktion kan **mutera objekt**. Ibland är det ofrånkomligt, men ofta kan man som sagt arbeta med returvärden istället.
     3.   En funktion kan **anropa andra funktioner**.
     4.   En funktion kan **påverka DOM:en**. Förvisso genom funktionsanrop, dvs punkten ovan, men detta brukar ofta sorteras in under en egen kategori. Funktioner som rör DOM:en bör vara få och tydligt utmärkta.
     5.   En funktion kan **skicka events**, antingen från sig själv eller via en global event-bus (i vårt fall Backbone-objektet). Även detta är egentligen funktionsanrop, men man brukar förtydliga just event-användning för att få en tydlig struktur i sin applikation.

     Som generell regel: Fundera igenom, och försök minimera, effekterna av dina funktioner. Ju större andel pure functions ju bätre!

###Moduler

Små enkla applikationer skulle kunna bo i en enda fil, och definiera massa funktioner och variabler direkt i det globala objektet. När applikationerna växer så blir detta dock snabbt ohanterligt - för vår egen skull behöver vi **dela upp koden i filer**, och för att inte alltför lätt dra på oss buggar så måste vi på något sätt **kompartementalisera koden**. Detta är egentligen två helt olika problem, men de har samma lösning - ett modulsystem.

De flesta andra språk har detta inbyggt - ett enkelt sätt att i en fil importera andra filer och resurser. I JavaScript saknas dock detta helt (än så länge)! Därför måste vi själva fixa fram en lösning. Man kan säga att modularisering i JavaScript kan ske i tre nivåer:

1.    Inte alls, dvs **lagra allt i det globala objektet**. Detta är i denna kurs absolut förbjudet.
2.    Lagra i det globala objektet, men på ett organiserat sätt via en **singleton**. Vi skapar ett objekt som håller vår applikation, och alla filer vi laddar in kommer sedan utöka detta objekt. Filerna kommer därmed vara hårt knutna till just denna struktur, men vi har ändå någon sorts organisation av våra beståndsdelar. Detta är bättre än inget, och genom lite smart användning av Inversion of Control kan man komma undan med att begränsa strukturberoendet till enstaka objekt på hög nivå. Singletons är ok i kursen, så länge det görs väl. 
3.    Användandet av ett **modulsystem**. Det finns ett flertal bibliotek som implementerar en traditionell modulladdare i JavaScript. Ett av de mest populära är [RequireJS][8], vars användning är obligatoriskt i kursen.


###Kopplingar och använding

Förvånansvärt mycket i bra koddesign ligger i hur objekt och moduler interagerar med varandra. Detta beror såklart på vilken modulapproach vi använder, men inte bara. I [litteraturlistan][2] hittar du boken *Learning JS Design Patterns* av Addy Osmani, som vi varmt rekommenderar att du tittar på. Den definierar ett antal *patterns*, mönster, som innebär god koppling av objekt.



###Allmäna resurser

I [litteraturlistan][2] finns flera böcker som ger allmäna och breda råd vad gäller kodorganisering:

*    *JavaScript Web Applications*
*    *Single Page Web Apps*
*    Om du har någon av tegelstenarna från tidigare kurser ([JS: The Definitive Guide][9] eller [Professional JS for Web Developers][10]) så har båda dessa också en hel del material om kodorganisering.

Övriga resurser:

*    Onlineboken [Single Page App Book][11] har en hel del bra stoff.
*    Framför allt vill vi uppmana er att utnyttja **handledningen** som erbjuds i kursen. Att organisera JavaScriptkod är *svårt*, och inget man lär sig på någon vecka genom att läsa denna hastigt ihopknåpade sida. Att aktivt fånga läraren och diskutera din kod är bästa sättet att komma in i rätt tänk!

 

 [1]: http://www.amazon.com/JavaScript-Web-Applications-Alex-MacCaw/dp/144930351X/ "JavaScript Web Applications"
 [2]: https://coursepress.lnu.se/kurs/ria-utveckling-med-javascript/kurslitteratur/
 [3]: https://github.com/rwldrn/idiomatic.js#table-of-contents
 [4]: http://google-styleguide.googlecode.com/svn/trunk/javascriptguide.xml
 [5]: http://www.youtube.com/watch?v=taaEzHI9xyY&amp;feature=youtube_gdata_player
 [6]: https://coursepress.lnu.se/kurs/ria-utveckling-med-javascript/steg-1-vagval/
 [7]: http://www.elijahmanor.com/2012/09/control-complexity-of-your-javascript.html
 [8]: https://coursepress.lnu.se/kurs/ria-utveckling-med-javascript/require/
 [9]: http://www.bokus.com/bok/9780596805524/javascript-the-definitive-guide-6th-edition/
 [10]: http://www.bokus.com/bok/9781118026694/professional-javascript-for-web-developers-3rd-edition/
 [11]: http://singlepageappbook.com/
