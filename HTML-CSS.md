# Teorihandboken - HTML & CSS (HC)
Studerande: Daniel Sedell

## HC 1.1 HTML & CSS
Html står för HyperText Markup Language och är det vi som vi kan kalla grunden till alla internets webbsidor. Html utgör själva strukturen på våra sidor, där det kan vara allt från bilder till styckesindelningar. 

Hur använder vi HTML?

Inom HTML har vi olika Element som bygger upp själva strukturen inom vår hemsida. En av de vanligaste elementen inom HTML när man vill skriva något heter p eller paragraf. 

<p>Hej jag heter Daniel</p>

Man brukar likna en paragraf med en brödtext. I alla elementen så börjar man nästan alltid med en starttag och avslutar med en endtag. Så när man skriver något inom de tagarna så vet man vart man har skrivit och vad man skriver. 

Det finns såklart undantag med vissa element angående sluttagar. Som elementet img så har den ingen sluttag. 

<img 
src="https://dogtime.com/wp-content/uploads/sites/12/2011/01/GettyImages-469196054-e1691415831480.jpg"
alt="Bild på en rottweiler">

HTML är grunden på vilken all webbutveckling vilar. Alla andra webbtekniker kan vara valfria, men HTML är oumbärlig för att skapa en webbsida. Även om det finns sätt att skapa webbsidor utan att behöva lära sig HTML, är det en nödvändig komponent i webbutveckling.

CSS, som förkortas för Cascading Style Sheets, utgör en av de fundamentala komponenterna på webben. Den arbetar i samverkan med HTML och Javascript och kan betraktas som webbens ansikte utåt, eftersom den är ansvarig för att forma webbplatser visuellt. Med hjälp av CSS har du möjlighet att kontrollera diverse aspekter, inklusive typsnittsval och skapandet av elegant animation.

Hur änvänder vi då CSS?

Det finns många olika sätt att använda CSS, ett exempel kan vara när man vill ändra storlek eller form av en bild. Vi kan ta bilden från HTML exemplet ovan och lägga till lite styling som man brukar kalla det. 

img {
  border-radius: 50%;
}

Det som händer nu är att min bild kommer att utforma sig som en cirkulär bild. Genom att skriva border-radius så ändrar vi själva storleken på radien. 

Man kan även lägga in CSS direkt in i HTML dokumentet. Det gör man genom att sätta ut en tag "<style>" och en slut tag "</style>", men problemet med detta är att det kan bli lite rörigt. Det är helt enkelt enklare om man skriver sin CSS kod i ett annat dokument som man länkar till sitt HTML dokument. Allting blir bara enklare med sortering och man hittar enklare sina olika delar av koden enklare. 

Varför använder vi CSS?

Största anledningen till att vi använder CSS är för att skapa inlevelse i sin webbsida, där det gäller färg, teckensnitt, justering av text och objekt mm. Så utan CSS skulle man inte kunna skapa dessa ändringar och det är sånt som är nödvändigt för att bygga upp en bra Webbsida. 




[Exsitec användes för att hitta lite mer info om HTML och CSS](https://www.exsitec.se/)
[ChatGPT användes för formatering av texten](https://chat.openai.com/)
[Genomgång av HTML och CSS från slidsen](https://chasacademy.instructure.com/courses/287/modules/items/6715)





## HC 1.2 Responsiv design
Responsiv webbdesign innebär att webbplatsen anpassar sig automatiskt efter skärmens upplösning. Oavsett om besökaren surfar från en surfplatta, smartphone eller dator, kommer webbplatsen alltid att anpassa sig till rätt format för en smidig upplevelse.

Det finns olika sätt att använda responisve desgin på. 
Den första designen man alltid brukar tillämpa i sitt HTML dokument är visningsporten eller som det heter på engleska Viewport. 
<!--<!DOCTYPE html>
<html lang="en">
  <head>
    …
    <meta name="viewport" content="width=device-width, initial-scale=1">
    …
  </head>
  …
-->
Genom att vi skriver width=device-width så matchar vi skärmens bredd i enhetsoberoende pixlar. 
initial-scale=1"> talar om hur mycket sidan ska zoomas in när den laddas in. Man kan även sätta den till ändra "initial" till "maximum" då det talar om hur mycket användaren är tillåten att zooma in. Det här är små designer som är nästan obligatoriska om man vill få en så responsive sida som möjligt. 

Flexbox är en annan bra design att implementera om man vill kontrollera sin layout i sin webbläsare. Det är ett effektivt sätt att skapa design då man har behov av att justera och disruptera saker mellan innehåll i sin container. 

<img src="https://miro.medium.com/v2/resize:fit:434/1*iigDGiNFBOUVJQ_07C1B2g.png">

Ovan så finns det en bild som visar bra exempel på hur man kan använda flexbox på många olika bra sätt. 

Ett annat sätt som liknar flexbox är Gridbox då de i helhet är rätt så lika, men det finns en sak som skiljer dem från varandra. Gridbox passar in i designer där man vill ha mer kontroll och kunna styra sitt arbete på ett bättre sätt. Det som skiljer Griv vs Flexbox är att man kan vertikalt ändra layouten på webbsidan med Grid, då man inte kan göra det om man använder Flexbox. 

<img src= "https://ishadeed.com/assets/grid-flex/grid-vs-flexbox.png">

Men varför använder vi responsive design?

kort sagt så skulle jag säga att man är väldigt framåttänkande om man använder responsive design. Det jag menar med det är att man vill alltid sträva efter ny utveckling, bättre design och alltid vara up to date som jag brukar kalla det. När jag använder mig av responsive design tänker jag alltid att det ska vara så enkelt och smidigt för användaren att använda min hemsida som jag skapar. Då det kan vara att det ska finnas alltid en mobilanpassad layout som gör det enkelt att scrolla igenon, utan att behöva scrolla eller zooma in/ut. 

[CSS grid, flexbox och responsivitet Slides från genomgång 21.9](file:///C:/Users/Danne/Downloads/3-CSS-grid-flexbox-och-responsivitet.pdf)
[ChatGPT för valedering av text](https://chat.openai.com/)
[Web.dev](https://web.dev/articles/responsive-web-design-basics)
[Bilderna](https://ishadeed.com/article/grid-layout-flexbox-components/)(https://medium.com/@lainakarosic/getting-started-with-css-flexbox-basics-58d875a574ce)





## HC 1.3 Tillgänglighet inom webb
Webbtillgänglighet, i grund och botten, handlar om att säkerställa att alla kan dra nytta av den information vi publicerar online. För oss som arbetar med webbutveckling finns några klara riktlinjer som kan göra detta arbete så smidigt som möjligt.

Det finns många olika tekniska lösningar som kan hjäpla en om man har något sorts av funktionshinder. En av dem ramverken heter WAI-ARIA. WAI-ARIA erbjuder en ram för att inkludera attribut som identifierar interaktionsfunktioner. WAI-ARIA ger riktlinjer för navigering som hjälper till att märka områden och vanliga webbstrukturer, såsom menyer, primärt innehåll, sekundärt innehåll, bannerinformation och andra webbstrukturer. Till exempel, genom att använda WAI-ARIA kan utvecklaren märka upp sidans områden och göra det smidigt för tangentbordsanvändare att navigera mellan dem utan att behöva upprepa tangenttryckningar.

Den mest vanliga fuktionen som används av många olika individer och organisationer runt om i världen, Web Content Accessibility Guidelines eller som förkortning WCAG. WCAG är en samling för olika riktlinjer där man ökar tillgängligheten på internet för användrare med olika funktionsvariationer. Kort sagt så vill man förenkla olika element för att kunna gör det så enkelt så möjligt för användaren att använda webbsidan, utan några större problem. Ett exempel kan vara att erbjuda undertexter eller transkriptioner för videoinnehåll samt att använda textbaserade alternativ för ljudinnehåll hjälper personer med hörselnedsättning att delta fullt ut.

När jag fokuserar på webbtillgänglighet tvingas jag tänka på olika sätt att presentera och interagera med webbinnehåll. Det kan leda till kreativa lösningar och innovationer som gör min webbplats eller app bättre för alla användare. 

Ett annat argument att använda webbtillgänglighet är att man får en ökad användarbas. Genom att sätta webbtillgänglighet i fokus, öppnar du dörrar till en bredare användarbas. Det handlar inte enbart om att underlätta för personer med funktionsvariationer, utan även att inkludera äldre användare och de som surfar med äldre webbläsare eller enheter som har begränsad funktionalitet. Detta kan i sin tur stärka din webbplats eller applikations popularitet och tillgänglighet.

[w3.org](https://www.w3.org/WAI/standards-guidelines/wcag/)
[Onsdag 27.9 - Tillgänglighet.pdf](https://chasacademy.instructure.com/courses/287/files/10557?module_item_id=7013)
[ChatGPT användes för formulering][https://chat.openai.com/]






























## HC 1.4 Aktuella webbstandarder (gällande och kommande standarder)


## HC 1.5 CSS Pre-processorer (ex SASS/LESS)
Beskriv rubriken nedan här

## HC 1.6 Optimering och validering av HTML & CSS
Beskriv rubriken nedan här
