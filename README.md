# RegEx Validering i JavaScript

Detta övningsrepo täcker grundläggande användning av reguljära uttryck (RegEx) för att validera användarinmatning i formulär. Du kommer att implementera olika typer av validering, såsom e-post, telefonnummer, lösenord, URL, postnummer och ålder. Vi kommer att använda JavaScript för att testa dessa regEx.

Övning 1-6 gör du i script.js samt med console.log, och för övning 7 ska du skapa ett formulär med HTML + JavaScript Formulär med RegEx Validering.
Förslag på format är:
```
const nameRegex = /^[A-Za-z]+ [A-Za-z]+$/;

const name = "John Doe";
const isValidName = nameRegex.test(name);
console.log(isValidName);  // true eller false
```
test:
```
const name1 = "John Doe";
const name2 = "John";
const name3 = "John 123";
const name4 = "john doe";

console.log(nameRegex.test(name1));  // true
console.log(nameRegex.test(name2));  // false (saknar efternamn)
console.log(nameRegex.test(name3));  // false (nummer är inte tillåtna)
console.log(nameRegex.test(name4));  // true (förnamn och efternamn fungerar också med små bokstäver)

```

## Uppgifter

 1. **Validera E-postadress**<br>
 Testa regEx för olika e-postadresser och implementera ett formulärfält där användaren kan skriva in sin e-postadress.

 2. **Validera Telefonummer**<br>
 Testa regEx för olika telefonnummerformat och implementera validering för telefonnummer i ett formulär.

 3. **Validera Lösenord (minst 8 tecken, en bokstav, en siffra, och ett specialtecken)**<br>
 Skapa ett lösenordsfält i ett formulär och ge användaren feedback om lösenordet är giltigt.

 4. **Validera URL**<br>
 Skapa ett URL-fält i ett formulär och validera att användaren skriver en korrekt URL.

 5. **Validera Postnummer (svenskt format)**<br>
 Skapa ett postnummerfält i ett formulär och validera postnumret.

 6. **Validera Ålder (mellan 18 och 100 år)**<br>
 Skapa ett åldersfält i ett formulär och validera att användaren är mellan 18 och 100 år gammal.

 7. **Skapa ett formulär med HTML + JavaScript Formulär med RegEx Validering.**<br>
Vi kommer att skapa ett formulär där användaren måste fylla i följande fält:
    - E-postadress
    - Telefonnummer
    - Lösenord
    - URL
    - Postnummer
    - Ålder

Om användaren försöker skicka in formuläret utan att fylla i rätt information, kommer felmeddelande att visas vid input-fältet det hör till.

### Länkar för mer information om RegEx:

- [RegExr](https://regexr.com/) – Ett bra verktyg för att skapa och testa reguljära uttryck.
- [MDN Web Docs - Regular Expressions](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions) – Dokumentation om RegEx i JavaScript.


Lycka till!
