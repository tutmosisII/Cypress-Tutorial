# Solución Ejecicio 2.

## 1. Correr Cypress con Chrome

En el objeto de scripts adiciona lo siguiente:

```javascript
"scripts": {

"test:chrome": "npx cypress run --browser chrome"

}
```


## 2. Correr Cypress con firefox

En el objeto de scripts adiciona lo siguiente:

```javascript
"scripts": {

"test:firefox": "npx cypress run --browser firefox"

}
```

Con las respectivas líneas en su lugar, solo queda pendiente ejecutar las pruebas.

```bash
npm run test:chrome
npm run test:firefox
```
