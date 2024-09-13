# Teorihandboken - Avancerad JavaScript (AJ)

Studerande: Daniel Sedell

## AJ 1.1 Node.js

### Vad är Node.js?

Node.js är en plattform som låter dig köra JavaScript-kod på serversidan, istället för bara i webbläsaren. Det är byggt på V8, vilket är Googles JavaScript-motor, samma som används i webbläsaren Chrome. Tack vare Node.js kan man använda JavaScript för att bygga hela webbtjänster, API:er, och till och med backend för appar.

### Varför använda Node.js?

En av de största fördelarna med Node.js är att det är väldigt snabbt och effektivt. Det hanterar många samtidiga förfrågningar utan att behöva starta en ny process för varje förfrågan. Det här är möjligt eftersom Node.js använder en så kallad "event loop", som låter den hantera flera saker samtidigt.

### När är Node.js bra att använda?

Node.js är speciellt bra när du bygger applikationer som behöver hantera många förfrågningar samtidigt, till exempel chattapplikationer eller realtids-tjänster. Det fungerar också bra för att bygga API:er som kommunicerar med andra tjänster eller databaser.

### Hur funkar det?

Med Node.js kan du använda JavaScript för att skapa och hantera servern, läsa och skriva filer, prata med databaser, och mycket mer. Eftersom JavaScript är ett av de mest använda programmeringsspråken, kan utvecklare använda sina befintliga kunskaper för att snabbt komma igång med Node.js.

### Ett enkelt exempel

Här är ett grundläggande exempel på en server skapad med Node.js:

```javascript
const http = require("http");

const server = http.createServer((req, res) => {
  res.statusCode = 200;
  res.setHeader("Content-Type", "text/plain");
  res.end("Hello World!");
});

const port = 3000;
server.listen(port, () => {
  console.log(`Servern körs på port ${port}`);
});
```

I det här exemplet skapar vi en enkel HTTP-server som svarar med texten "Hej, världen!" när någon besöker servern. Servern körs på port 3000, och du kan se ett meddelande i konsolen när servern startar.

## AJ 1.2 Express

### Vad är Express?

Express är ett populärt ramverk för att bygga webbapplikationer och API:er med Node.js. Det är känt för att vara enkelt, flexibelt och lätt att använda, vilket gör det till ett bra val för både nybörjare och erfarna utvecklare.

### Hur fungerar det?

Med Express kan du skapa "rutter" som bestämmer vad din applikation ska göra när någon besöker en viss sida eller skickar data till din server. Till exempel kan du skapa en rutt som visar en hemsida när någon går till din webbadress, och en annan rutt som tar emot användardata från ett formulär och sparar det i en databas.

### Varför använda Express?

1. **Enkelt och lätt att komma igång med:** Du kan snabbt sätta upp en server och börja bygga din applikation med bara några få rader kod.

2. **Flexibelt:** Du kan anpassa och utöka Express efter dina behov, vilket gör det användbart för allt från små till stora projekt.

3. **Stort community:** Eftersom Express är så populärt, finns det massor av exempel, handledningar och färdiga moduler som du kan använda för att spara tid och undvika att uppfinna hjulet på nytt.

### Ett enkelt exempel

Här är ett enkelt exempel på hur man kan använda Express för att skapa en webbserver som visar ett meddelande när någon besöker din sida:

```javascript
const express = require("express"); // Importera Express
const app = express(); // Skapa en Express-app

// Skapa en rutt för hemsidan
app.get("/", (req, res) => {
  res.send("Hej världen!"); // Skicka tillbaka "Hej världen!" när sidan besöks
});

// Starta servern på port 3000
app.listen(3000, () => {
  console.log("Servern körs på http://localhost:3000");
});
```

## AJ 1.3 Progressive Web Apps

### Vad är en Progressive Web App?

Progressive Web Apps är en typ av webbapplikation som kombinerar det bästa av webb och mobilappar. Du kan köra appen genom att ladda ner den eller direkt i din webbläsare. PWA kombinerar fördelarna med en webbplats med egenskaper från konventionella appar.

### Varför ska man använda den typen av app?

- PWA-tekniken som används är så kraftfull att man kan bygga en väldigt bra och responsiv app med den.
- Det är mycket billigare att skapa en app med denna teknik, och den kan ersätta appar för iOS, Android och Windows Phone.
- Man behöver inte ladda ner något, till skillnad från vanliga appar som kräver en nedladdning.

Att skapa en Progressive Web App (PWA) innebär att bygga en vanlig webbapp och sedan lägga till några specifika funktioner för att göra den "progressiv". Här är en grundläggande överblick av hur du kan skapa en enkel PWA med HTML, CSS och JavaScript.

### Steg för att skapa en enkel PWA

- Bygg en grundläggande webbapp med HTML, CSS och JavaScript.
- Skapa en manifestfil som beskriver appens metadata.
- Använd service workers för att göra appen tillgänglig offline och hantera caching.

Genom att följa dessa steg kan man skapa en grundläggande Progressive Web App (PWA) som inte bara fungerar smidigt offline, utan också kan installeras direkt på användarnas enheter. Det innebär att appen erbjuder en app-liknande upplevelse utan att behöva laddas ner via en traditionell appbutik. Nu är den fullt funktionell och redo att användas både online och offline, vilket ger användarna flexibilitet och en sömlös upplevelse, oavsett deras internetanslutning.

Källor: [https://whitespace.se/blogg/vad-ar-pwa-eller-progressive-web-apps/](https://whitespace.se/blogg/vad-ar-pwa-eller-progressive-web-apps/)

## AJ 1.4 Typningssystem för Javascript (ex TypeScript, Flow)

# Typningssystem för JavaScript

Ett typningssystem för JavaScript används för att ge fast typkontroll och hjälpa till att hitta och undvika fel som beror på felaktiga typer i koden. JavaScript är ett dynamiskt typat språk, vilket betyder att variabler kan ändra typ medan programmet körs. För att lägga till typkontroll i JavaScript används ofta **TypeScript** eller **JSDoc-kommentarer**.

## Hur TypeScript fungerar

TypeScript fungerar genom att lägga till fast typkontroll till JavaScript. Du skriver koden i TypeScript och bestämmer vilka typer variabler, funktioner och objekt ska ha. Sedan omvandlas TypeScript-koden till vanlig JavaScript, som kan köras i alla webbläsare eller miljöer.

TypeScript använder också **duck typing**, vilket betyder att om ett objekt har de rätta egenskaperna eller funktionerna, så räknas det som rätt typ, oavsett vilken typ det ursprungligen var.

## Vanliga TypeScript-annotations

Här är några vanliga annotations som används i TypeScript:

### `number`

Används för att ange att en variabel är ett tal.

```typescript
let age: number = 30;
```

### `string`

Anger att en variabel är en textsträng.

```typescript
let name: string = "Alice";
```

# TypeScript Annotation: `boolean`

### `boolean`

Används för att ange att en variabel är en sanningsvärdesvariabel, vilket innebär att den kan ha värdet `true` eller `false`.

```typescript
let isDone: boolean = false;
```

## AJ 1.5 Funktionell programmering i JavaScript

# Funktionell programmering

Funktionell programmering är ett programmeringsparadigm som behandlar beräkning som utvärdering av matematiska funktioner. Det lägger stor vikt vid att undvika föränderligt tillstånd och muterbara data. Istället för att ändra variabler, fokuserar funktionell programmering på att använda rena funktioner som alltid ger samma utdata för samma indata.

Funktionell programmering har sina rötter i lambda-kalkyl, ett formellt system utvecklat av matematikern Alonzo Church på 1930-talet. Lambda-kalkyl var ett sätt att undersöka beräkningsbarhet och funktioner, långt innan moderna datorer existerade.  
Den första implementationen av ett funktionellt programmeringsspråk var Lisp, skapat av John McCarthy 1958. Lisp introducerade många koncept som fortfarande är centrala i funktionell programmering idag.

## Viktiga egenskaper i funktionell programmering:

- **Oföränderlighet (Immutability)**: Detta är en grundpelare. I funktionell programmering ändrar vi inte data när den väl skapats. Istället skapar vi nya datastrukturer när vi behöver göra ändringar. Detta minskar risken för oväntade sidoeffekter och gör koden mer förutsägbar.
- **Rena funktioner**: Funktioner i funktionell programmering är "rena", vilket betyder att de alltid ger samma output för samma input och inte har några sidoeffekter. Detta gör koden lättare att testa och förstå.
- **Högre ordningens funktioner**: Vi kan behandla funktioner som värden - skicka dem som argument till andra funktioner eller returnera dem från funktioner. Detta ger oss kraftfulla abstraktionsmöjligheter.

## Exempel

```javascript
// Vi har en lista med tal
const numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];

// Vi vill filtrera ut jämna tal, dubbla dem, och sedan summera resultatet

// Steg 1: Filtrera ut jämna tal
const isEven = (num) => num % 2 === 0;
const evenNumbers = numbers.filter(isEven);

// Steg 2: Dubbla varje tal
const double = (num) => num * 2;
const doubledNumbers = evenNumbers.map(double);

// Steg 3: Summera alla tal
const sum = (acc, num) => acc + num;
const total = doubledNumbers.reduce(sum, 0);

console.log("Summan av de dubblade jämna talen är:", total);
```

## AJ 1.6 Avancerad funktionalitet i ES.next

### Vad är ES.Next

ECMAScript Next (ES.next) refererar till den nyaste versionen av ECMAScript-standarden, grunden för JavaScript. Varje ny utgåva innehåller nya funktioner och förbättringar som underlättar för utvecklare att skapa mer effektiv och pålitlig kod. Dessa uppdateringar är resultatet av ett pågående arbete från TC39, den tekniska kommittén som ansvarar för att utveckla ECMAScript-standarden. Målet är att kontinuerligt förfina språket och introducera moderna funktioner som möter de växande behoven hos utvecklare och applikationer.

### Processen när de olika förslagen läggs till

1. **Idéfas (Stage 0):** Här läggs förslaget fram som en idé, ofta av en medlem i TC39. Därefter diskuteras om förslaget är värt att skickas vidare till nästa steg.

2. **Förslag (Stage 1):** Om idén ser lovande ut skrivs en specifikation och idén diskuteras på en högre nivå.

3. **Utformning (Stage 2):** En mer detaljerad specifikation skapas, och vid det här laget förväntas det finnas ett utkast.

4. **Färdigställande (Stage 3):** Förslaget ska vara färdigställt och utvecklare testar det för att säkerställa att det fungerar i praktiken.

5. **Godkännande (Stage 4):** Förslaget är nu redo att inkluderas i den officiella ECMAScript-standarden.

Vi kan ta ett exempel på ett förslag som är i Stage 4:

#### ECMAScript-förslag: Promise.any + AggregateError

En kort beskrivning av förslaget:

`Promise.any` tar emot en samling av löften (promises) och ger tillbaka ett löfte som uppfylls av det första löftet som lyckas. Om alla löften misslyckas, returnerar det istället ett fel som innehåller alla orsaker till varför de misslyckades. Om något går riktigt fel, som om det uppstår ett fel när man går igenom samlingen, ger `Promise.any` tillbaka ett misslyckat löfte med det felet.

Här kommer ett exempel från `Promise.any`:

```javascript
Promise.any([
  fetch("https://v8.dev/").then(() => "home"),
  fetch("https://v8.dev/blog").then(() => "blog"),
  fetch("https://v8.dev/docs").then(() => "docs"),
])
  .then((first) => {
    // Any of the promises was fulfilled.
    console.log(first);
    // → 'home'
  })
  .catch((error) => {
    // All of the promises were rejected.
    console.log(error);
  });
```

källor: <https://github.com/tc39/proposals>, <https://www.proposals.es/>, https://www.proposals.es/proposals/Promise.any

## AJ 1.7 JavaScript i integrerade system

Beskriv rubriken här

## AJ 1.8 Native bundeling av JavaScript för olika operativsystem och enheter

Beskriv rubriken här
