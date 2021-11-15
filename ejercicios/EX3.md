# Ejecutando Pruebas en una aplicación.

En el [ejercicio 2](Ex2.md) nos familiarizamos con la línea de comandos.

Correr pruebas en la línea de comandos, es mucho más efectivo que hacer uso del navegador. Esto se debe a bajo consumo de recursos al correr la prueba, pue no se levanta una interfaz gráfica (headless).

Por defecto Cypres usa el navegador Electron y corre las pruebas especificadas en los archivos **.spec.js** en la carpeta de integración del proyecto.

## Configuración de Cypress.

Cypress puede configruarse por medio de:

| Configuracion | Bandera | Descripcción |
|---|---|---|
| Variables de Ambiente | --env o -e | Pasa variables definidas en la terminal a la ejecución de Cypress|
| Configuracion temporal | --config o -c | Se peuden cambiar las configuraciones definidas en **Cypress.json** al sobre escribirlas por medio de estas banderas.|
| Configuracion por archivo | --config-file o -C | Se especifíca un archivo a usar los valores declarados sobre escribe las ya definidas en **Cypress.json** |
| Correr un Navegador | --headed | Abre un navegador para correr las pruebas|
| Correr sin navegador | --headless | Corre pruebas sin UI |
| Correr una especificación | --spec o -s | corre solo las pruebas de dicha especificación |

## Trabajando en una aplicación real **[RWA](https://github.com/cypress-io/cypress-realworld-app)**

Youtube:  [Cypress Patterns and Prectices](https://www.youtube.com/watch?v=V-o8WzlwKmM)
