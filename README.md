# palitosypelotitas

## Bultos fijos en BMW

Si querés que uno o más bultos queden siempre arriba del BMW, editá esta constante en `index.html`:

```js
const BULTOS_FIJOS_BMW = [];
```

### Ejemplos

- Ninguno fijo en BMW:
  - `const BULTOS_FIJOS_BMW = [];`
- Solo uno fijo (primer bulto):
  - `const BULTOS_FIJOS_BMW = ["b1"];`
- Varios fijos:
  - `const BULTOS_FIJOS_BMW = ["b1", "b7", "b12"];`

## Como identificar un bulto

Cada bulto tiene un ID interno con formato `bN` (`b1`, `b2`, `b3`, etc.).
El `b1` corresponde al primer texto de la lista `stringsBultos`, `b2` al segundo, y asi sucesivamente.

## Nota sobre estado guardado

La posicion de los bultos se guarda en `localStorage`.
Si cambias `BULTOS_FIJOS_BMW`, al recargar se aplica la regla y esos bultos quedan en BMW.
