# Einführung in React mit TypeScript (Teil 1)

## Urls

- react-typescript-workshop.deckset.net
- bit.ly/2NyiBQx
- prettier anschauen. (https://github.com/prettier/prettier)
- TSLint (https://palantir.github.io/tslint/)

## Tipps & Tricks

- *immutables* sollten nicht mehr verändert werden.
- Destructuring anschauen.

### Destructuring

```javascript
function Welcome(props) {
  const { city } = props;
  return <h1>Hallo {city}</h1>;
}
```

```javascript
function Welcome({ city }) {
  return <h1>Hallo {city}</h1>;
}
```

- Auch hier nochmal der Hinweis. **KEINE function** immer nur noch Arrow functions.

### 🚨 Regeln 🚨

- Komponenten werden immer in UpperCamelCase benannt
- Props werden immer in lowerCamelCase benannt
- Komponenten werden niemals wie eine Funktion aufgerufen!
- ~~ ```Welcome({ city: 'Oer-Erkenschwig' })``` ~~

##

- map bei Arrays verwenden.
- React Componenten könnene mittlerweile auch Listen Elemente übergeben.

    ```javascript
    import * as React from 'react';

    const numbers = [1, 2, 3, 4, 5];

    const listItems = numbers.map(number => (
    <li key={number}>{number}</li>
    ));

    const App = () => <div>{listItems}</div>;
    ```
- Bei ```boolean``` immer ```has``` oder ```is``` davor schreiben. ```{isToggle: false}```.
- Auch in React immer mit FatArrow arbeiten. Das erledigt das bind im Konstruktor.
  
    Schlecht:
    ```javascript
    constructor(props) {
            super(props)
            // This binding is necessary to make `this` work in the callback
            this.splashOver = this.splashOver.bind(this);
        }

    handleClick() {
    this.setState(prevState => ({
        isToggleOn: !prevState.isToggleOn
    }));
    }
    ```

    Besser:
    ```javascript
    handleClick = () => {
    this.setState(prevState => ({
        isToggleOn: !prevState.isToggleOn
    }));
    };
    ```

- HOC "Higher Order Components" anschauen.
- Styled Compnents anschauen! Wichtig!!!
- Context-API

