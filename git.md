###Git

Git är ett **versionshanteringssystem**, precis som Subversion som många av er har använt i tidigare kurser. Man installerar det lokalt på sin dator, och kan sedan skapa projektspecifika **repositorier**. Därefter kan man sedan backa i filhistoriken allteftersom man ställer till det för sig.

Git innehåller också funktionalitet för att **synka repositorier**. Det gör exempelvis att du kan klona en kompis projekt över nätverket, ändra lite i koden, och pusha tillbaka ändringarna till honom.

Riktigt kraftfullt blir det när vi istället arbetar mot ett repositorium i "molnet". Vilket osökt för oss till nästa rubrik:


###Github

Github är en "Git repository hosting service" på nätet. Genom att skapa ett konto där och pusha dit kod du skriver lokalt så blir du plötsligt oberoende av din arbetsstation - så länge som du sitter vid en dator med Git installerat, så kan du tanka ned din kod, arbeta med den, och pusha upp det du gjort till Github. Detta arbetssätt innebär två stora fördelar:

*    Dels blir det ett **automatiskt säkerhetskopieförfarande**. Skulle din hårddisk brinna så finns allting kvar på Github (fram till din senaste push såklart, så pusha ofta!).
*    Framför allt så blir det lätt att **kollaborera**. Hela team kan därmed enkelt samarbeta i samma kodbas, vilket vore hart när omöjligt om det bara vore löst liggande filer på ett nätverk.

Via [Githubs hemsida][5] kan man bläddra i projekt (om de inte är closed source) och snoka runt i koden.


###Cloud9

Cloud9 är en "editor in the cloud" som låter dig manipulera dina filer direkt i webbläsaren. Vi behöver inte längre en arbetsstation med Git och en editor, utan skulle kunna jobba från en sidewalk express på centralstationen! Läs mer på [resurssidan för Cloud9][4].


###Använding i kursen

I kursen är det **obligatoriskt att använda Github** som repositorium. Tidigare år har Subversion tillåtits eftersom många varit fästa vid det, men nu är den dörren stängd och låst!

Vi kommer dessutom använda **Github som publiceringsplattform** för våra projekt! Detta genom att utnyttja en funktionalitet de kallar för *Github pages*. Kortfattat går den ut på att all kod som pushas till en branch med namnet "gh-pages" (det vanliga standardnamnet är annars "master") deployas till en webserver, och blir tillgänglig på `http://<githubid>.github.com/<projektnamn>`.

Om ni sedan väljer att... 

1.    ta bort master
2.    låta master vara kvar men glömma bort den
3.    hålla både master och gh-pages uppdaterade

...är helt upp till er.


###Resurser

*    [Skolans Git-intro][8]
*    [Introduktion till Github][2], inkluderar även en Git primer
*    [Introduktion till Git][3] för den som inte blev mätt på Git-infon i Githubguiden ovan
*    [Gitintro av Jenny Donelly][1]
*    [Guide på 2010 års kursweb][7] (kräver inloggning)






 [1]: http://www.youtube.com/watch?v=QB6r9Y7mqyU&amp;feature=youtube_gdata_player
 [2]: https://help.github.com/articles/set-up-git
 [3]: http://git-scm.com/book/en/Getting-Started-Git-Basics
 [4]: https://coursepress.lnu.se/kurs/ria-utveckling-med-javascript/cloud9-editor/
 [5]: https://github.com/
 [7]: http://voyager.lnu.se/tekinet/kurser/dtt/2DV407/index.php?sida=html%2Fresurser%2Fgit
 [8]: https://coursepress.lnu.se/info/manual/kom-igang-med-github/