# Scripts de npm

Correr comandos desde al terminal es una característica que se peude lograr usando la propiedad **script** de **pakage.json**

Adiciona la línea de apertura en el objeto de scripts de [pakage.json](Proyecto-Prueba/package.json)
```bash
"scripts": {

  "open": "npx cypress open"

}
```

Ahora es posible correr el proyecto desde la terminal con el siguiente comando:

```bash
npm run open
```