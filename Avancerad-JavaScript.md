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
