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
