# Teorihandboken - Avancerad JavaScript (AJ)

Studerande: Förnamn Efternamn

## AJ 1.1 Node.js

Beskriv rubriken här

## AJ 1.2 Express

Beskriv rubriken här

## AJ 1.3 Progressive Web Apps

Beskriv rubriken här

## AJ 1.4 Typningssystem för Javascript (ex TypeScript, Flow)

Beskriv rubriken här

## AJ 1.5 Funktionell programmering i JavaScript

Beskriv rubriken här

## AJ 1.6 Avancerad funktionalitet i ES.next

<h3>Vad är ES.Next </h3>

ECMAScript Next (ES.next) refererar till den nyaste versionen av ECMAScript-standarden, grunden för JavaScript. Varje ny utgåva innehåller nya funktioner och förbättringar som underlättar för utvecklare att skapa mer effektiv och pålitlig kod. Dessa uppdateringar är resultatet av ett pågående arbete från TC39, den tekniska kommittén som ansvarar för att utveckla ECMAScript-standarden. Målet är att kontinuerligt förfina språket och introducera moderna funktioner som möter de växande behoven hos utvecklare och applikationer.

<h3>Processen när de olika förlsagen läggs till</h3>

1. Vi börjar med Idéfas (stage 0): Här läggs förlaget ut som en ide på något, ofta är det en medlem i TC39 som presenterar idén. Sedan diskuterar man om förslaget är värt att skickas vidare till nästa steg.

2. Nu går vi vidare till Förslag (Stage 1): Om idén ser lovande ut så skrivs en specifikation och idén diskuteras på en högre nivå.

3. Nu har vi kommit halvägs, till själva Utformingen (stage 2) Man har gjort en mer detaljerda specifikation, och vid det här laget förväntas det finnas ett utkast.

4. Här har vi stadiet när förslaget är Färdigställande (stage 3) Här ska förlaget vara färdigställt och utvecklare testas för att säkerställa att förslaget fungerar i praktiken.

5. Sedan har vi Godkännande (stage 4) där förslaget är redo att inkluderas i den officiella ECMAScript-standarden.

Vi kan ta ett exempel på ett förslag som är i stage 4:

<h4>ECMAScript proposal: Promise.any + AggregateError</h4>

En kort beskrivning av den innebär:

Promise.any tar emot en samling av löften (promises) och ger tillbaka ett löfte som uppfylls av det första löftet som lyckas. Om alla löften misslyckas, returnerar det istället ett fel som innehåller alla orsaker till varför de misslyckades. Om något går riktigt fel, som om det uppstår ett fel när man går igenom samlingen, ger Promise.any tillbaka ett misslyckat löfte med det felet.

Här kommer ett exempel från Promise.any

```javascript
Promise.any([
  fetch('https://v8.dev/').then(() => 'home'),
  fetch('https://v8.dev/blog').then(() => 'blog'),
  fetch('https://v8.dev/docs').then(() => 'docs')
]).then((first) => {
  // Any of the promises was fulfilled.
  console.log(first);
  // → 'home'
}).catch((error) => {
  // All of the promises were rejected.
  console.log(error);
});

källor: <https://github.com/tc39/proposals>, <https://www.proposals.es/>, https://www.proposals.es/proposals/Promise.any

## AJ 1.7 JavaScript i integrerade system

Beskriv rubriken här

## AJ 1.8 Native bundeling av JavaScript för olika operativsystem och enheter

Beskriv rubriken här
```
