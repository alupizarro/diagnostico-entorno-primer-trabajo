# Diagnóstico del entorno Node.js

## Descripción

Este proyecto fue realizado para diagnosticar el entorno de desarrollo utilizando Node.js.

El programa `diagnostico.js` muestra información sobre la versión de Node.js, la plataforma, los argumentos recibidos y una variable de entorno.

## Requisitos

Para ejecutar el proyecto se necesita:

- Node.js
- npm
- Git
- Visual Studio Code

## Ejecución con Node.js

Para ejecutar el diagnóstico directamente con Node.js:

    node diagnostico.js prueba

## Ejecución con npm

El proyecto contiene un script llamado `diagnostico`.

Para ejecutarlo:

    npm run diagnostico -- prueba

## Información mostrada

El programa informa:

- Versión de Node.js.
- Plataforma del sistema.
- Argumentos recibidos.
- Variable de entorno `NOMBRE`.

## Control de versiones

El proyecto utiliza Git para registrar los cambios mediante commits incrementales.

## Evidencia 

Versiones
node --version
npm --version
git --version

Ejecución directa
node diagnostico.js prueba

Ejecución con npm
npm run diagnostico -- prueba

Commits
git log --oneline

Estado final
git status

“¿Qué hace diagnostico.js?”
 “Es un programa de Node.js que muestra información del entorno donde se está ejecutando.”
________________________________________
“¿Qué es process.version?”
“Es una propiedad de Node.js que permite obtener la versión de Node que está ejecutando el programa.”
En mi caso:
v24.15.0
________________________________________
“¿Qué es process.platform?”
“Indica la plataforma del sistema operativo donde se está ejecutando Node.”
En mi computadora aparece:
win32
porque estoy usando Windows.
________________________________________
“¿Qué es process.argv?”
“Es un arreglo que contiene los argumentos que recibió el programa desde la línea de comandos.”
Cuando ejecute:
node diagnostico.js prueba
el argumento que agregue es:
prueba
________________________________________
“¿Qué es process.env.NOMBRE?”
“Permite leer una variable de entorno llamada NOMBRE.”
Yo puse:
NOMBRE=Alumna Alejandra
y el programa mostró:
Variable de entorno NOMBRE: Alumna Alejandra
________________________________________
“¿Para qué sirve package.json?”
“Es el archivo de configuración del proyecto Node.js. En este caso también contiene el script que permite ejecutar el diagnóstico mediante npm.”
"diagnostico": "node diagnostico.js"
________________________________________
“¿Qué hace npm run diagnostico -- prueba?”
 “Ejecuta el script diagnostico definido en package.json. El -- indica que lo que viene después se pasa como argumento al programa.”
Por eso termina ejecutándose:
node diagnostico.js prueba
________________________________________
“¿Qué hace git add?”
“Prepara los archivos para incluirlos en el próximo commit.”
________________________________________
“¿Qué hace git commit?”
“Guarda un punto de control del proyecto en el historial de Git.”
________________________________________
“¿Qué hace git push?”
“Sube los commits del repositorio local al repositorio remoto de GitHub.”
________________________________________
“¿Qué hace git status?”
“Muestra el estado actual del repositorio y si existen cambios pendientes.”
Y:
nothing to commit, working tree clean
