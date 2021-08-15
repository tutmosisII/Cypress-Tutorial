# Instalación.

# Instalación de Nodejs

Cypress corre sobre el motor de de Node, para su instalación revise las instrucciones de la página.

```bash
sudo apt update
sudo apt install snapd
sudo snap install node --classic

node -v
```
# Instalación de Cypress.

**Buena Práctica:" Se suele instalar Cypress en el directorio del proyecto.

Para esta primer prueba vamos a:
* crear un directorio de proyecto
* En ese mismo directorio inicializamos un proyecto de node.
* En el directorio vamos a instalar Cypress.

```bash
mkdir  Proyecto-Prueba
cd Proyecto-Prueba
npm init -y
```

Ahora instalamos Cypress localmente en el proyecto:

```bash
npm install cypress --save-dev
```
En este momento el directorio de proyecto debe lucir así:
```
├── Proyecto-Prueba
│   ├── node_modules
│   ├── package.json
│   └── package-lock.json
```
Cypress No ha sido ejecutado por lo que aún no tenemos el ejecutor de las pruebas en su sitio.

## Ejecutando Cypress con npx

Los ejecutables de node pueden se lanzan con el comando npx
```bash
npx cypress open
```

Luego de ejecutado cypress ahora tenemos nuestro ambiente de pruebas.

```
├── Proyecto-Prueba
│   ├── cypress              <---
│   ├── cypress.json         <---
│   ├── node_modules
│   ├── package.json
│   └── package-lock.json
```



