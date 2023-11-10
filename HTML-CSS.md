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
Webbstandarder är riktlinjer från organisationer som World Wide Web Consortium (W3C) och andra standardiseringsgrupper. Dessa riktlinjer fastställer hur webbaserat innehåll bör skapas och tolkas. Även om begreppet webbstandarder har funnits sedan de tidiga dagarna av internetutvecklingen, har det bara nyligen blivit allmänt omfamnat av de mest populära webbläsarna.

Syftet med webbstandarder är att säkerställa att information som publiceras på internet är hållbar och samtidigt tillgänglig för så många användare som möjligt. Webbplatser som följer dessa standarder är utformade för att fungera korrekt i de senaste webbläsarna och kommer även att vara tillänglig för framtida webbläsare.

Webbstandarder har sitt ursprung i behovet att strukturera och standardisera webbsidor samt etablera etiska riktlinjer för deras skapande och användning. De tre ursprungliga webbstandarderna kan vara igenkännbara som Hypertext Markup Language (HTML), Uniform Resource Identifier (URL) och  HyperText Transfer Protocol (HTTP).

HTLM är en av den vanligaste webbstandarderna vi har idag. Det är även en webbstandar som jag använder rätt så mycket när jag skriver mina projekt. HTML är själva webbens publiceringsspråk, varje sida grundar sig från den. En av egenskaperna man kan skapa med HTML är tillgänglighet. Med de olika HTML-tilgänglihetsalternativ kan man hjälpa människor så att de kan använda din hemsida på ett så effektivt sätt som möjligt. 
 
CSS är något som jag använder mycket och det är en webbstandard som kan hjälpa till med designflexibilitet. Med CSS kan man ändra storlek på sina texter, färger och annat som kan ändra strukturen på ett positivt sätt. 

Webbstandarder erbjuder fördelar för både webbanvändare och webbutvecklare. Genom att anpassa sig till webbstandarder och följa WCAG-riktlinjerna, kan man förbättra sökmotoroptimering och tillgänglighet samtidigt som man stöder framsteg inom teknologi och designflexibilitet. Detta gynnar både dem som navigerar på webben och de som skapar webbinnehåll.

[Webflow](https://webflow.com/blog/web-standards)

[w3c](http://www.w3c.se/resources/w3c/standards/index.html)

[ChatGPT för formatering](https://chat.openai.com/)
## HC 1.5 CSS Pre-processorer (ex SASS/LESS)

CSS Pre-processorer är ett program som låter dig generera CSS från förproccernas egan unika synax. De vanligaste CSS Pre-processorerna som används är SASS eller LESS. 

Sass som är en av de mer vanligare CSS Pre-processorer har funnits ett tag. I Sass är en av de mest praktiska funktionerna möjligheten att skapa variabler. Liknande andra programmeringsspråk kan du tilldela värden till variabler för att enkelt återanvända dem senare. I Sass definieras variabler genom att använda dollartecknet ($) före variabelnamnet, som exempelvis: 

$ background-color: #2E3A23 

Det finns två större anledningar varför man vill skriva såhär. En av dem är att om du behöver använda samma färg på flera av dina sidor så behöver du helt enkelt bara komma ihåg vad för variabel du skrev. Andra anledningen är att Om du någonsin behöver ändra värdet för flera väljare är allt du behöver göra att ändra ett värde i variabeln. 

@Import

Sass utökar CSS @import-regeln för att möjliggöra import av både Sass- och SCSS-filer. Samtliga importerade filer kombineras sedan till en enda utmatad CSS-fil. Dessutom överför alla variabler eller mixins som definieras i de importerade filerna till huvudfilen, vilket innebär att du kan blanda och matcha olika filer med försäkran om att alla stilar bibehålls på global nivå.

Vid användning av @import specifieras ett filnamn att importera. Som en sista utväg kan Sass-import utföras genom att ange filnamnet för Sass- eller SCSS-filerna. Om inget filändelse anges kommer Sass att försöka hitta en fil med det namnet och antingen .scss eller .sass-förlängning och importera den.

I en typisk Sass-projektinstallation kan du observera @import-regler inom en basfil. Det möjliggör en smidig synkronisering mellan flera filer vid kompileringen, till exempel: 

@import "main.scss";

I den senaste uppgiften "u02 redesign" så använder vi @import för att kunna länka stylingen mellan olika dokument. Det gör vi för att man inte ska behöva skriva en massa onödig kod. 

När man väll har förstått och fattar hur man kan använda SASS på ett smidigt sätt så kommer man alltid att implementera det i sitt projekt.

[Lektionsmaterial](https://chasacademy.instructure.com/courses/287/files/10468?module_item_id=7006)

[Beginneer guide till SASS](https://sv.odwebdesign.net/the-beginners-guide-to-sass/)

[ChatGPT för formatering av text](https://chat.openai.com/)

## HC 1.6 Optimering och validering av HTML & CSS

HTML- och CSS-validering involverar att granska koden för en webbplats för att säkerställa att den är i linje med de senaste standarderna och fri från fel. Denna process är avgörande för att säkerställa att webbplatsen är läsbar och begriplig för både människor och sökmotorrobotar. Dessutom kan validering bidra till att förbättra laddningstiden för webbplatsen, vilket är kritiskt för SEO-optimering. Vidare har HTML- och CSS-validering potential att identifiera och åtgärda säkerhetsbrister innan de blir potentiella problem. 

Hur kan vi optimera och validera våran kod på bästa möjliga sätt?

Först och främst, ingen vill besöka en hemsida där allt innehåll laddar in långsamt, bilderna är för stora eller texten har fel font-size. En av de bättre optimeringar  man kan göra är att förminska din kod.  Att optimera din kod innebär att eliminera överflödiga tecken, mellanslag, kommentarer och formatering från dina HTML- och CSS-filer. Denna process syftar till att reducera filstorleken och därmed påskynda laddningstiden för dina webbsidor. För att uppnå detta kan du använda olika verktyg och plugins, antingen online eller lokalt, som automatiskt eller manuellt minimerar din kod.

Förutom att förbättra prestanda har förminskning av kod också en fördelaktig sidoeffekt – det blir svårare för andra att kopiera eller ändra din kod. Genom att eliminera onödiga detaljer och extratecken skapas en mer kompakt och svårtydd kod, vilket ökar säkerheten och skyddet för din webbplats.

Valedering är något som är väldigt viktigt. Anledningen varför man vill valedera är att en validator underlättar upptäckten av enkla misstag och felsteg på ett smidigt sätt, vilket sparar oss från onödiga huvudvärk. Dessutom bidrar det till att skapa en ökad konsistens på våra webbplatser över olika webbläsare. Validatorn fungerar som ett verktyg för att säkerställa att vår webbkod är korrekt och följer standarder, vilket i sin tur främjar en bättre användarupplevelse och en mer enhetlig presentation av webbplatsen.

[ChatGPT för formatering av text](https://chat.openai.com/)
[Lektionsmaterial 3-Optimering-och-validering.pdf](https://chasacademy.instructure.com/courses/287/files/10575?module_item_id=7017)
[linkedin optimering och validering](https://www.linkedin.com/advice/3/what-most-effective-html-css-optimization-86tlf#:~:text=LinkedIn%20Top%20Voice-,The%20most%20effective%20HTML%20and%20CSS%20optimization%20strategies%20for%20your,Implement%20efficient%20CSS%20selectors.)
