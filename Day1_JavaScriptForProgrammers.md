# JavaScript for Software Developers
**Date:** 2018-10-09
**Location:** Berlin

## Documentation und Urls

- Doku GitHub Folder: https://github.com/whythecode/javascript-for-software-developers
- Standard Dokumentation: developer.mozilla.org
- Polyfills sind MethodExtensions in JavaScript. Man kann sie einsetzen wenn ein Browser nicht kompatibel ist. Besser aber auf Babbel oder TypeScript setzten.

## Debugging

node --inspect-brk file.js
chrome://inspect/#devices

## Tipps & Tricks

- Buchstaben klein; minus statt underscore
- Undefined ist von der Engine, null ist für den Entwickler. Niemals zuweisen. Böses Faul.
- Monate fangen bei Null an.
- mdn templatestring anschauen. (https://developer.mozilla.org/de/docs/Web/JavaScript/Reference/template_strings)
- Unterschied Truesly und falsley: Andere Datentypen wie 1, true, 'wahr', [], {} ist kein echtes true aber truesly. (https://developer.mozilla.org/de/docs/Glossary/Truthy
- == da casted Javascript im Hintergrund, deswegen immer === zum vergleichen benutzen. Wenn ich unterschiedliche Vergleiche habe dann den Wert casten.
- Arguments bei functions nicht benutzen. Kein echtes Array. Rest Operator ist viel besser. 
```javascript
function dynamicParams(a, ...other) {}
```
- https://github.com/Microsoft/TypeScript-React-Starter
- Functions Objekte wichtiges Werkzeug in JavaScript. Siehe 03-functions.js.
- () schaffen einen eigenen Scoop. Ivvy Pattern.
- Arrow Function => Lamdba Ausdruck.
- let is better then var. let is only visible in the blockscope.
- airbnb style-guide (https://github.com/airbnb/javascript)
- const in JavaScript hält die Refernz fest. Bei einem Datentyp ist es eine echte Konstante.
- immutable (https://facebook.github.io/immutable-js/) [groß] und immutablily-helper (https://github.com/kolodny/immutability-helper) [Klein und fein] für DeepCopies anschauen.
- Konstruktor Funktionen sind ganz normale Funktionen. Best Practise UpperCase.
- this ist immer der aktuelle Scope. function zertört this. Lamda verwenden. Früher wurde bind oder var self = this verwendet.
- asnyc und await gibt es auch in JavaScript. Basiert auf Promises.
- event.preventDefault(); ganz wichtig. Immer bei Event Handler machen. Gibt noch eine Steigerung. 
- swagger


## Nachforschen

- [x] Speaker benutzt cooles LivePlugIn. (Quokka)