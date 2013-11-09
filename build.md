Med build step, eller **byggsteg**, menas en automatiserad procedur där applikationen löpande konkateneras, minifieras och packas till en distributionsversion. Det kan också innebära kompilering av exempelvis CoffeeScript och SASS/SCSS eller liknande.

Eftersom vi redan använder Require så ligger det nära till hands att använda **r.js**, som ingår där som beståndsdel. Om du är nyfiken, läs på om hur den funkar och integrera den i ditt löpande arbete med appen!

Samma resultat kan också uppnås med exempelvis [GruntJS](http://gruntjs.com/) eller liknande, som i sin tur exekverar node-moduler eller dylikt. 

Om du använder ett byggsteg, se till att både distributionsversionen OCH den orörda källkoden ligger uppe på Github Pages! 
