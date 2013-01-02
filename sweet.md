&quot;Sweeten your JavaScript!&quot;

[Sweet.js][1] är ett bibliotek som låter dig göra ändringar i JavaScripts syntax. Du introducerar ny syntax, och koden &quot;kompileras&quot; sedan till vanlig JavaScript. Bygg ditt eget CoffeeScript, helt enkelt! Det finns flera exempel på den officiella hemsidan, där ett av de enklaste är följande - genom detta makro:

[javascript]
macro fn {
	case $name:ident $params $body => {
		function $name $params $body
	}
}
[/javascript]


...så kan vi skriva `fn` istället för det fantastiskt jobbiga `function`:
<div>
[javascript]
fn usefulFunc(a){
	console.log("Whopee!");
}
[/javascript]
</div>

Vi skulle också kunna göra så att vi inte behöver använda &quot;tomma parenteser&quot; när vi inte har några argument till funktionen.

### Sweet.js i kursen

**Varför** använda ett makrobibliotek i en kurs fokuserad på kodorganisering? Därför att dess användning får dig att ställa bra frågor. När är språkets syntax i vägen för min produktivitet? När gör språkets syntax så att kodens betydelse döljs? Vilka delar av syntaxen skulle du vilja ändra om du kunde? Att testa på sweet.js är ett ypperligt sätt att komma djupare in i rätt mindset för att bli en JavaScript ninja!

**Hur** skall vi gå till väga för att nyttja makron i vårt projekt? Eftersom kursen kräver att din kod skall kunna köras utan ett kompileringssteg, så måste ni använda en [plugin till RequireJS][2] som direkt parsar makrokoden.

### Resurser

*    [Den officiella hemsidan][1]
*    [Sweet.js wiki][3]
*    [Dedikerat avsnitt av JavaScript Jabber podcast][4]
*    [Diskuterande blogpost][5]



[1]: http://sweetjs.org
[2]: https://github.com/iammerrick/require-sweet
[3]: https://github.com/mozilla/sweet.js/wiki/Example-macros
[4]: http://javascriptjabber.com/039-jsj-sweet-js-with-tim-disney/
[5]: http://jlongster.com/why-sweet.js-matters