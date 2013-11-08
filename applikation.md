Som ni förhoppningsvis sett vid det här laget så handlar kursen i huvudsak om ett **projekt** där ni skall utveckla en JavaScript-applikation. Vad innebär då detta?

###Krav

För det första så finns det ett par riktlinjer som inte är förhandlingsbara:

1.   Projekten kommer publiceras via [Github Pages][1], och måste vara körbara i sin helhet därifrån. Det innebär att ni **inte kan ha några serverside-komponenter**, utan helt kommer jobba mot local storage. Er kod bör inte heller kräva prekompileringssteg (som exempelvis LESS/SASS). CoffeeScript skulle därmed också vara utvisat, men det [går att lösa ändå][2].
2.   Projektet måste på något vis **hantera &amp; spara data från användaren**. Det kan ej bara handla om statisk bearbetning (typ miniräknare), utan måste *keep some state* i någon mening.

Utöver detta så är fältet dock helt fritt!

###Aspekter

Kursens titel, *RIA-utveckling med JavaScript*, är väldigt bred, så ock fokuset vad gäller era projekt. Detta är dock vad vi vill att ni skall fokusera på, och vad vi fokuserar på i vår bedömning:

*    **Utvecklingsmiljö och beståndsdelar:** Rätt verktyg till rätt uppgift blir allt mer viktigt ju mer avancerad uppgifter är. Därför skall vi lägga tid på efterforskning, göra genomtänkta val, och bemästra de verktyg vi väljer att använda.
*    **Kodorganisering:** Detta är kanske det mest primära. Just att organisera JavaScriptprojekt är riktigt lurigt, så en stor del av handledningen kommer handla om att hjälpa er på den fronten. Läs mer på [resurssidan][4].
*    **Datahantering**: Beroende på vad ni väljer att bygga så kommer detta kräva olika mycket kärlek. Oavsett vad så är er datamodell en del av det vi bedömer i slutändan!
*    **Användargränssnitt:** Kursen är väldigt tekniskt inriktad, så vi kommer inte kräva några estetiska mästerverk. Det är dock inte en ursäkt för ett dåligt användargränssnitt! Framför allt så vill vi att ni skall vara bekanta med *the problem space*, så att säga, vilket är anledningen till att vi uppmuntrar er att smaka på [Twitter Bootstrap][3].

###Projektförslag

Nog prokrastrinerat - vad skall ni bygga? Som sagt väljer ni själva, men här följer några förslag som kan få in era tankar på rätt spår:

*    En **Todo-applikation** är den klassiska (och därmed urtråkiga) exempelapplikationen. Detta av en bra anledning, då den innebär en väldigt bra grundnivå för datastrukturen: En todo har flera givna egenskaper (färdig eller inte, till exempel), och man kan stegvis utöka komplexiteten genom att införa kategorier, taggar, etc.
*    Även en **Projekthanteringsapp** skulle kunna funka. Vi har olika dataobjekt (projekt, delmål, milstolpar, personer) med relationer emellan, som erbjuder flera möjliga komplexitetsnivåer.
*    Kanske en enkel **personaldatabas**? Varje person har en given person som chef (förutom chefchefen såklart), vilket ger bra utrymme för relationer, listor och vyer av enskilda personer.
*    Varför inte en liten **Bank** eller motsvarande? Konton och transaktioner ger kul möjligheter till funktionalitet.
*    Enkla (observera *enkla*) **spel** skulle också kunna fungera, såsom Blackjack eller Roulette. Spel brukar dock innebära mer jobb med kontexten än vad man först kan tro, så, tänk er för före!

En sak vi vill trycka på är återigen att **projektet inte kommer vara särskilt stort i omfattning**, eftersom såpass mycket fokus läggs på processen. Tjuvkika gärna på tidigare års projekt så förstår ni nog - de flesta är ganska "enkla", och vid en första anblick kan de se ut som att de knappast tagit 20*5 timmar att utveckla. Men det beror som sagt på att de studerande parallellt har forskat, bloggat, diskuterat och omprövat. Vilket också ni skall göra! Håll därför ner ambitionsnivån i projektplanerandet!


[1]: https://coursepress.lnu.se/kurs/ria-utveckling-med-javascript/git-github/
[2]: https://coursepress.lnu.se/kurs/ria-utveckling-med-javascript/coffeescript/
[3]: https://coursepress.lnu.se/kurs/ria-utveckling-med-javascript/twitter-bootstrap/
[4]: https://coursepress.lnu.se/kurs/ria-utveckling-med-javascript/kodorganisering/