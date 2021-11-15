# Comando de Cyspress.

Hay dos maneras de instalar Cypress, de forma local o global. En este repositorio hemos venido trabajando con la instalación local.

## Instalación local

```bash
npm install cypress
```
Esta forma de instalación es recomendada por el equipo de dearrollo de Cypress.

## Instalación Global

```bash
npm install cypress --global
```

La **importancia de la línea de comandos** vs la ejecucíón en un navegador con cabecera radica en el el poder de la automatización y la reducción de las dependencias manuales.

## Comando básicos de Cypress.

```bash
cypress run
cypress open 
cypress info
cypress version
```

### cypress run

Esta es la orden para ejecutar las pruebas en el proyecto sin cabeceras ([headless](diccionario.md)) por defecto se usará el navegador de [Electron](https://www.electronjs.org/)

Este comando corre las instrucciones de las pruebas de isntegración especificadas en el archivo **.spec.js**

Las configuraciones más comunes son

| Bandera | Descripción |
|--|--|
|--env ó -e | Permite definir [varibales de ambiente](https://www.freecodecamp.org/news/what-are-environment-variables-and-how-can-i-use-them-with-gatsby-and-netlify/) por medio de la línea de comandos|
|--browser ó -b|Define el navegador a usar para las pruebas|
|--config ó -c| Sobre escribe configruaciónes del archivo cypress.json en la línea de comandos de forma dinámica|
|--config-file ó -C|Sobre escribe configruaciónes del archivo cypress.json abriendo un nuevo archivo de configuración.|
|--headed| Corre las pruebas luego de abrir un browser|
|--headless| Corre las pruebas sin un navegador con ambiente gŕafico, ideal para ejecuciones en pipelines o automatizadas|
|-spec ó -s| Indica que archivo spec se va a ejecutar.|

## cypress run --env <varibale-de-ambiente>

Las variables de ambiente controlan la manera como **Cypress** es ejecutado.

Si se requeire ejecutar pruebas en diferentes ambientes el uso de variables de ambiente recobra mucha importancia.
Son últiles tambien cuando los ambietes cambian rápidamente.

Se pueden definir como cadenas de caractéres ó objetos de JSON.