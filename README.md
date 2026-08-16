# Entrega Técnica 1 - Diagnóstico del entorno Node.js

##  Introducción

Este trabajo corresponde a la Entrega Técnica 1 de la materia Despliegue.

El objetivo principal fue preparar mi entorno de desarrollo, comprobar que las herramientas necesarias estuvieran instaladas y funcionando, crear un pequeño programa en Node.js para diagnosticar el entorno de ejecución y registrar el proceso utilizando Git y GitHub.

El programa que desarrollé se llama `diagnostico.js`.

Este programa realiza un diagnóstico básico del entorno y muestra:

- La versión de Node.js.
- La plataforma sobre la que se está ejecutando.
- Los argumentos recibidos desde la terminal.
- Una variable de entorno.

Además, configuré un script en `package.json` para poder ejecutar el diagnóstico mediante npm.

Finalmente utilicé Git para registrar los cambios mediante commits incrementales y GitHub para publicar el repositorio.

---

##  Objetivo del trabajo

El objetivo de este trabajo fue aprender a preparar y comprobar un entorno básico de desarrollo y realizar un primer diagnóstico utilizando Node.js.

Las tareas que fui realizando fueron:

1. Preparar las herramientas necesarias.
2. Comprobar Node.js.
3. Comprobar npm.
4. Comprobar Git.
5. Trabajar desde Visual Studio Code.
6. Crear la carpeta del proyecto.
7. Crear el proyecto Node.js.
8. Crear `diagnostico.js`.
9. Utilizar información del objeto `process`.
10. Mostrar la versión de Node.js.
11. Mostrar la plataforma.
12. Mostrar los argumentos recibidos.
13. Mostrar una variable de entorno.
14. Ejecutar el programa directamente con Node.js.
15. Configurar un script npm.
16. Ejecutar el programa mediante npm.
17. Inicializar Git.
18. Crear commits incrementales.
19. Crear el README.
20. Crear el repositorio remoto en GitHub.
21. Subir el proyecto a GitHub.
22. Comprobar el estado final.
23. Generar evidencia técnica de la ejecución.

---

##  Herramientas utilizadas

Para realizar el trabajo utilicé:

- Visual Studio Code.
- Node.js.
- npm.
- Git.
- GitHub.
- Terminal de Windows.

Las versiones que comprobé fueron:

```text
Node.js: v24.15.0
npm: 11.12.1
Git: 2.53.0.windows.3
```

La plataforma detectada por Node.js fue:

```text
win32
```

Esto corresponde a Windows.

---

## Preparación inicial del entorno

Primero preparé mi entorno de trabajo.

Para realizar el proyecto necesitaba tener instalados Node.js, npm, Git y Visual Studio Code.

Node.js y npm son necesarios para ejecutar el programa y trabajar con el proyecto.

Git es necesario para realizar el control de versiones.

Visual Studio Code lo utilicé como editor de código y también para utilizar su terminal integrada.

---

##  Comprobación de Node.js

Desde la terminal ejecuté:

```bash
node --version
```

El resultado fue:

```text
v24.15.0
```

Este comando sirve para comprobar que Node.js está instalado y disponible desde la terminal.

También permite conocer qué versión de Node.js estoy utilizando.

### Concepto: Node.js

Node.js es un entorno que permite ejecutar JavaScript fuera de un navegador.

En este trabajo utilicé Node.js para ejecutar el archivo:

```text
diagnostico.js
```

La ejecución básica del programa se realiza mediante:

```bash
node diagnostico.js prueba
```

En esta instrucción, `node` es el programa que ejecuta JavaScript y `diagnostico.js` es el archivo que quiero ejecutar.

---

##  Comprobación de npm

Después ejecuté:

```bash
npm --version
```

El resultado fue:

```text
11.12.1
```

Este comando permite comprobar que npm está instalado y funcionando.

### Concepto: npm

npm es el gestor de paquetes de Node.js.

También permite ejecutar scripts que se encuentran definidos en el archivo `package.json`.

En este proyecto utilicé npm para crear el proyecto y posteriormente para ejecutar el script de diagnóstico.

---

##  Comprobación de Git

Después comprobé Git utilizando:

```bash
git --version
```

El resultado fue:

```text
git version 2.53.0.windows.3
```

Esto confirmó que Git estaba instalado y disponible desde la terminal.

### Concepto: Git

Git es un sistema de control de versiones.

Permite registrar los cambios realizados en un proyecto y mantener un historial de los diferentes estados del proyecto.

---

##  Visual Studio Code y la terminal

Utilicé Visual Studio Code para crear y modificar los archivos del proyecto.

Dentro de Visual Studio Code abrí la carpeta del proyecto y utilicé la terminal integrada.

La terminal me permitió ejecutar los comandos de Node.js, npm y Git sin salir de Visual Studio Code.

---

##  Creación de la carpeta del proyecto

Creé una carpeta para trabajar con el proyecto llamada:

```text
diagnostico-entorno-primer-trabajo
```

La carpeta se encuentra dentro de:

```text
C:\Users\Pc\DESKTOP\DESPLIEGUE\
```

Dentro de esta carpeta quedaron los archivos correspondientes al proyecto.

---

##  Creación del proyecto Node.js

Dentro de la carpeta del proyecto ejecuté:

```bash
npm init -y
```

Este comando crea automáticamente un archivo llamado:

```text
package.json
```

### Concepto: package.json

`package.json` es el archivo principal de configuración de un proyecto Node.js.

Contiene información del proyecto y también permite definir scripts que luego puedo ejecutar utilizando npm.

Entre otras cosas puede contener:

- Nombre del proyecto.
- Versión.
- Descripción.
- Scripts.
- Dependencias.
- Tipo de módulo.

En este trabajo utilicé especialmente la sección:

```text
scripts
```

porque ahí agregué el comando para ejecutar el diagnóstico.

---

##  Creación de diagnostico.js

Después creé el archivo:

```text
diagnostico.js
```

Este archivo contiene el programa principal del proyecto.

El objetivo de este archivo es realizar un diagnóstico del entorno en el que se está ejecutando Node.js.

Para mostrar la información utilizo:

```javascript
console.log()
```

También utilizo diferentes propiedades del objeto:

```javascript
process
```

---

##  Concepto de diagnóstico

En este proyecto, un diagnóstico es una comprobación de información del entorno de ejecución.

El programa consulta diferentes datos para saber cómo y dónde se está ejecutando.

En mi caso el diagnóstico informa:

- Versión de Node.js.
- Plataforma.
- Argumentos.
- Variable de entorno.

Esto permite comprobar que Node.js funciona correctamente y conocer información del entorno.

---

##  Concepto de console.log()

Utilicé:

```javascript
console.log()
```

`console.log()` sirve para mostrar información en la consola o terminal.

Lo utilicé para mostrar los resultados del diagnóstico.

Por ejemplo:

```javascript
console.log("Diagnóstico del entorno")
```

permite mostrar un mensaje en la terminal.

---

##  Concepto de process

`process` es un objeto que proporciona Node.js.

Permite obtener información y acceder a diferentes características relacionadas con el proceso que está ejecutando actualmente el programa.

En este trabajo utilicé:

```javascript
process.version
```

```javascript
process.platform
```

```javascript
process.argv
```

```javascript
process.env
```

Cada propiedad me permite obtener un tipo diferente de información.

---

##  process.version

Utilicé:

```javascript
process.version
```

Esta propiedad permite conocer la versión de Node.js que está ejecutando el programa.

En mi caso el resultado fue:

```text
v24.15.0
```

Esto sirve para comprobar con qué versión de Node.js se está ejecutando el programa.

---

##  process.platform

Utilicé:

```javascript
process.platform
```

Esta propiedad permite conocer la plataforma sobre la que se está ejecutando Node.js.

En mi caso el resultado fue:

```text
win32
```

Esto significa que Node.js está ejecutándose en Windows.

---

##  process.argv

Utilicé:

```javascript
process.argv
```

Esta propiedad contiene los argumentos utilizados al ejecutar el programa desde la terminal.

Ejecuté:

```bash
node diagnostico.js prueba
```

En esta instrucción:

```text
node
```

ejecuta Node.js.

```text
diagnostico.js
```

es el archivo que quiero ejecutar.

```text
prueba
```

es un argumento que le estoy pasando al programa.

Por eso `process.argv` contiene información relacionada con la ejecución y también el argumento:

```text
prueba
```

Esto sirve para que un programa pueda recibir información desde la línea de comandos.

---

##  process.env

También utilicé:

```javascript
process.env
```

`process.env` permite acceder a las variables de entorno disponibles para el proceso de Node.js.

En este proyecto utilicé una variable llamada:

```text
NOMBRE
```

y su valor fue:

```text
Alumna Alejandra
```

El programa consulta:

```javascript
process.env.NOMBRE
```

y muestra el valor de la variable.

El resultado fue:

```text
Variable de entorno NOMBRE: Alumna Alejandra
```

---

##  Concepto de variable de entorno

Una variable de entorno es un valor que está disponible para los programas desde el entorno donde se ejecutan.

En este proyecto utilicé:

```text
NOMBRE=Alumna Alejandra
```

La finalidad fue demostrar que el programa podía acceder a un dato del entorno utilizando:

```javascript
process.env.NOMBRE
```

Las variables de entorno son útiles porque permiten proporcionar información al programa desde el entorno de ejecución.

---

##  Primera ejecución del programa

Una vez creado `diagnostico.js`, ejecuté el programa desde la terminal utilizando:

```bash
node diagnostico.js prueba
```

El programa mostró información del entorno, incluyendo:

```text
Diagnóstico del entorno
Versión de Node.js: v24.15.0
Plataforma: win32
```

También mostró los argumentos recibidos y la variable de entorno.

Esta ejecución comprobó que el programa funcionaba correctamente.

---

##  Configuración del script de npm

Después modifiqué el archivo:

```text
package.json
```

Dentro de la sección `scripts` agregué:

```json
"diagnostico": "node diagnostico.js"
```

Esto significa que creé un script llamado:

```text
diagnostico
```

Cuando ejecuto:

```bash
npm run diagnostico
```

npm busca ese script y ejecuta:

```bash
node diagnostico.js
```

Esto permite ejecutar el programa de una manera más sencilla utilizando npm.

---

##  Comprobación de los scripts de npm

Para comprobar que npm reconociera correctamente el script ejecuté:

```bash
npm run
```

El resultado mostró el script:

```text
diagnostico
```

y su comando:

```text
node diagnostico.js
```

Esto confirmó que el script estaba correctamente agregado.

---

##  Ejecución mediante npm

Después ejecuté:

```bash
npm run diagnostico -- prueba
```

El resultado fue:

```text
> diagnostico-entorno-primer-trabajo@1.0.0 diagnostico
> node diagnostico.js prueba

Diagnóstico del entorno
Versión de Node.js: v24.15.0
Plataforma: win32
```

También se mostraron los argumentos y:

```text
Variable de entorno NOMBRE: Alumna Alejandra
```

El diagnóstico volvió a ejecutarse correctamente.

---

##  Concepto del -- en npm

En el comando:

```bash
npm run diagnostico -- prueba
```

el `--` sirve para separar las opciones de npm de los argumentos que quiero enviar al programa.

Por eso la palabra:

```text
prueba
```

llega al programa y aparece dentro de:

```javascript
process.argv
```

La ejecución termina siendo equivalente a:

```bash
node diagnostico.js prueba
```

---

##  Inicialización de Git

Una vez que comprobé que el programa funcionaba, inicialicé Git.

Ejecuté:

```bash
git init
```

Esto convirtió la carpeta del proyecto en un repositorio Git.

### Concepto: repositorio Git

Un repositorio Git es el lugar donde Git guarda la información necesaria para controlar las versiones y el historial de cambios de un proyecto.

---

##  git status

Utilicé:

```bash
git status
```

Este comando permite conocer el estado actual del repositorio.

Al principio Git mostró que tenía archivos que todavía no estaban registrados.

Entre ellos estaban:

```text
diagnostico.js
package.json
```

Esto me permitió comprobar qué archivos estaban pendientes de agregar.

---

##  git add

Después utilicé:

```bash
git add .
```

El punto significa que quiero agregar los archivos del proyecto al área de preparación de Git.

Luego comprobé nuevamente:

```bash
git status
```

y Git mostró que los archivos estaban preparados para realizar el primer commit.

### Concepto: área de preparación

El área de preparación es el lugar donde se colocan los cambios que quiero incluir en el próximo commit.

---

##  Primer commit

Después realicé:

```bash
git commit -m "Crear proyecto inicial"
```

El primer commit quedó identificado como:

```text
49485bd Crear proyecto inicial
```

Este commit registró el estado inicial del proyecto.

### Concepto: commit

Un commit es un registro de un estado del proyecto.

Permite guardar un punto determinado del historial y saber qué cambios se realizaron.

En este trabajo utilicé commits incrementales para que el proceso fuera visible.

---

##  Creación del README

Después creé el archivo:

```text
README.md
```

El README es el archivo de documentación principal del proyecto.

En él explico:

- El objetivo del trabajo.
- Las herramientas utilizadas.
- Los comandos realizados.
- El funcionamiento del diagnóstico.
- Los conceptos utilizados.
- El proceso con Git.
- La evidencia técnica.
- La forma de ejecutar el proyecto.

---

##  Segundo commit

Después de crear el README ejecuté:

```bash
git add README.md
```

Esto preparó el README para ser registrado.

Después ejecuté:

```bash
git commit -m "Agregar README"
```

El segundo commit quedó:

```text
c9d2840 Agregar README
```

---

##  Historial de commits

Para comprobar los commits ejecuté:

```bash
git log --oneline
```

El resultado fue:

```text
c9d2840 (HEAD -> master) Agregar README
49485bd Crear proyecto inicial
```

Esto demuestra que tengo dos commits y que el proceso quedó registrado de manera incremental.

### Concepto: git log

`git log` permite consultar el historial de commits del proyecto.

Utilicé:

```bash
git log --oneline
```

La opción `--oneline` permite mostrar los commits de forma resumida.

---

##  Comprobación del estado del proyecto

Utilicé:

```bash
git status
```

para comprobar el estado del proyecto.

El resultado final fue:

```text
On branch master
nothing to commit, working tree clean
```

Esto significa que no había cambios pendientes de registrar.

### Concepto: working tree clean

Cuando Git muestra `working tree clean`, significa que no hay cambios pendientes respecto del último commit.

---

##  Creación del repositorio en GitHub

Después publiqué el proyecto en GitHub.

El repositorio se llama:

```text
diagnostico-entorno-primer-trabajo
```

La descripción utilizada fue:

```text
Diagnóstico del entorno de desarrollo realizado con Node.js para informar versiones, plataforma, argumentos y variables de entorno.
```

Repositorio:

https://github.com/alupizarro/diagnostico-entorno-primer-trabajo

---

##  Concepto de repositorio remoto

Un repositorio remoto es una copia del repositorio que se encuentra en otro lugar, en este caso en GitHub.

Mi repositorio local está en mi computadora.

El repositorio remoto está en GitHub.

Git permite conectar ambos y enviar los cambios del repositorio local al remoto.

---

##  Comprobación del repositorio remoto

Para comprobar la conexión con GitHub ejecuté:

```bash
git remote -v
```

El resultado fue:

```text
origin  https://github.com/alupizarro/diagnostico-entorno-primer-trabajo.git (fetch)
origin  https://github.com/alupizarro/diagnostico-entorno-primer-trabajo.git (push)
```

`origin` es el nombre que Git utiliza para identificar el repositorio remoto principal.

### Concepto: origin

`origin` es un nombre utilizado habitualmente por Git para identificar el repositorio remoto principal del proyecto.

---

##  Error de remote origin

En un momento intenté agregar nuevamente el repositorio remoto utilizando:

```bash
git remote add origin https://github.com/alupizarro/diagnostico-entorno-primer-trabajo.git
```

Git respondió:

```text
error: remote origin already exists.
```

Esto no significaba que el proyecto estuviera mal.

Significaba que el repositorio remoto llamado `origin` ya estaba configurado.

Lo comprobé nuevamente con:

```bash
git remote -v
```

y confirmé que la dirección era correcta.

Por lo tanto no fue necesario agregar nuevamente el remoto.

---

##  Subida del proyecto a GitHub

Para subir los commits a GitHub ejecuté:

```bash
git push -u origin master
```

La operación se realizó correctamente.

Git mostró:

```text
[new branch] master -> master
branch 'master' set up to track 'origin/master'.
```

Esto significa que la rama `master` local quedó vinculada con la rama `master` del repositorio remoto.

### Concepto: git push

`git push` sirve para enviar los commits del repositorio local al repositorio remoto.

En este caso los envió a GitHub.

---

##  Concepto de rama

Una rama es una línea de trabajo dentro de un repositorio Git.

En este trabajo utilicé la rama:

```text
master
```

Cuando ejecuté:

```bash
git push -u origin master
```

vinculé mi rama local `master` con la rama remota `master`.

---

##  Comprobación de la subida

Después ejecuté nuevamente:

```bash
git push -u origin master
```

y Git mostró:

```text
Everything up-to-date
```

Esto significa que todos los cambios ya estaban subidos al repositorio remoto.

---

##  Comprobación final

Finalmente comprobé:

```bash
git status
```

y obtuve:

```text
On branch master
Your branch is up to date with 'origin/master'.
nothing to commit, working tree clean
```

Esto confirmó que:

- Estoy trabajando en la rama `master`.
- La rama local está actualizada.
- La rama está conectada con `origin/master`.
- No tengo cambios pendientes.
- El repositorio está limpio.

También ejecuté:

```bash
git log --oneline
```

y obtuve:

```text
c9d2840 (HEAD -> master, origin/master) Agregar README
49485bd Crear proyecto inicial
```

Esto demuestra que los commits están sincronizados con GitHub.

---

##  Código ejecutable

El proyecto puede ejecutarse directamente mediante Node.js utilizando:

```bash
node diagnostico.js prueba
```

También puede ejecutarse mediante npm utilizando:

```bash
npm run diagnostico -- prueba
```

Las dos formas ejecutan el diagnóstico.

---

##  Resultado de la ejecución

El resultado obtenido fue:

```text
Diagnóstico del entorno
Versión de Node.js: v24.15.0
Plataforma: win32
Argumentos: [
  'C:\Program Files\nodejs\node.exe',
  'C:\Users\Pc\DESKTOP\DESPLIEGUE\diagnostico-entorno-primer-trabajo\diagnostico.js',
  'prueba'
]
Variable de entorno NOMBRE: Alumna Alejandra
```

Con esta salida pude comprobar que todos los datos solicitados aparecen correctamente.

---

##  Evidencia técnica

Como evidencia técnica del trabajo realicé las siguientes comprobaciones.

### Versiones

Ejecuté:

```bash
node --version
npm --version
git --version
```

Resultados:

```text
v24.15.0
11.12.1
git version 2.53.0.windows.3
```

### Ejecución directa

Ejecuté:

```bash
node diagnostico.js prueba
```

El programa mostró correctamente:

```text
Versión de Node.js: v24.15.0
Plataforma: win32
Argumentos: ...
Variable de entorno NOMBRE: Alumna Alejandra
```

### Ejecución mediante npm

Ejecuté:

```bash
npm run diagnostico -- prueba
```

El diagnóstico volvió a ejecutarse correctamente.

### Historial

Ejecuté:

```bash
git log --oneline
```

Resultado:

```text
c9d2840 Agregar README
49485bd Crear proyecto inicial
```

### Estado final

Ejecuté:

```bash
git status
```

Resultado:

```text
nothing to commit, working tree clean
```

### Repositorio remoto

Ejecuté:

```bash
git remote -v
```

y comprobé que estaba conectado con GitHub.

---

##  Evidencias que acompañan la entrega

Para demostrar técnicamente el trabajo puedo presentar capturas de:

1. `node --version`.
2. `npm --version`.
3. `git --version`.
4. `node diagnostico.js prueba`.
5. `npm run diagnostico -- prueba`.
6. `git status`.
7. `git log --oneline`.
8. `git remote -v`.
9. El repositorio en GitHub.

Estas capturas permiten demostrar que las herramientas están instaladas, que el programa funciona, que npm ejecuta el script, que Git registra los cambios y que el proyecto fue publicado en GitHub.

---

##  Conceptos principales que aprendí

### Node.js

Es un entorno que permite ejecutar JavaScript fuera del navegador.

Lo utilicé para ejecutar `diagnostico.js`.

### npm

Es el gestor de paquetes de Node.js.

También permite ejecutar scripts definidos en `package.json`.

### package.json

Es el archivo de configuración del proyecto.

En este trabajo lo utilicé para definir el script:

```json
"diagnostico": "node diagnostico.js"
```

### diagnostico.js

Es el programa principal del proyecto.

Su función es mostrar información del entorno.

### console.log()

Sirve para mostrar información en la terminal.

### process

Es un objeto proporcionado por Node.js que permite acceder a información del proceso actual.

### process.version

Muestra la versión de Node.js.

### process.platform

Muestra la plataforma donde se está ejecutando Node.js.

### process.argv

Contiene los argumentos enviados desde la línea de comandos.

### process.env

Permite acceder a las variables de entorno.

### Variable de entorno

Es un valor proporcionado por el entorno de ejecución que puede ser leído por el programa.

### Git

Es un sistema de control de versiones.

### git init

Inicializa un repositorio Git.

### git status

Muestra el estado actual del repositorio.

### git add

Prepara archivos para un commit.

### git commit

Registra un estado del proyecto.

### git log

Muestra el historial de commits.

### git remote

Permite consultar o configurar repositorios remotos.

### git push

Envía los cambios del repositorio local al repositorio remoto.

### GitHub

Es el servicio donde publiqué el repositorio remoto.

---

##  Comprensión del código

El objetivo del trabajo no fue solamente conseguir que el programa funcionara.

También tuve que comprender qué hace cada parte.

Puedo explicar que:

- `diagnostico.js` es el programa que realiza el diagnóstico.
- `console.log()` muestra la información.
- `process.version` obtiene la versión de Node.js.
- `process.platform` obtiene la plataforma.
- `process.argv` obtiene los argumentos.
- `process.env.NOMBRE` obtiene la variable de entorno.
- `package.json` contiene la configuración del proyecto.
- El script `diagnostico` permite ejecutar el programa mediante npm.

---

##  Comprensión de los comandos de Git

También comprendí el objetivo de los principales comandos utilizados.

```bash
git init
```

Sirve para inicializar el repositorio.

```bash
git status
```

Sirve para comprobar el estado del repositorio.

```bash
git add .
```

Sirve para preparar los archivos para un commit.

```bash
git commit -m "mensaje"
```

Sirve para registrar un estado del proyecto.

```bash
git log --oneline
```

Sirve para consultar el historial.

```bash
git remote -v
```

Sirve para comprobar los repositorios remotos.

```bash
git push -u origin master
```

Sirve para subir los commits al repositorio remoto.

---

##  Estructura final del proyecto

La estructura principal del proyecto es:

```text
diagnostico-entorno-primer-trabajo/
|
├── diagnostico.js
├── package.json
├── README.md
└── .git/
```

El archivo `diagnostico.js` contiene el programa.

El archivo `package.json` contiene la configuración del proyecto y el script de npm.

El archivo `README.md` contiene la documentación.

La carpeta `.git` contiene la información del repositorio y su historial.

---

##  Cumplimiento de los criterios de entrega

### Código ejecutable

El proyecto puede ejecutarse utilizando:

```bash
node diagnostico.js prueba
```

o:

```bash
npm run diagnostico -- prueba
```

El programa funciona correctamente y muestra los datos solicitados.

### Proceso visible

El proceso quedó registrado mediante commits incrementales.

Los commits realizados fueron:

```text
49485bd Crear proyecto inicial
c9d2840 Agregar README
```

El historial puede comprobarse utilizando:

```bash
git log --oneline
```

### Evidencia técnica

La entrega cuenta con evidencia de:

- Versiones de Node.js, npm y Git.
- Ejecución directa del programa.
- Ejecución mediante npm.
- Historial de Git.
- Estado final del repositorio.
- Repositorio remoto.
- Proyecto publicado en GitHub.

---

## Resultado final

Al finalizar el trabajo obtuve un proyecto Node.js ejecutable que realiza un diagnóstico básico del entorno.

El programa informa:

```text
Versión de Node.js
Plataforma
Argumentos
Variable de entorno
```

Además, el proyecto cuenta con:

- `diagnostico.js`
- `package.json`
- `README.md`
- Git
- Commits incrementales
- Evidencia técnica
- Repositorio remoto
- Publicación en GitHub

Repositorio:

https://github.com/alupizarro/diagnostico-entorno-primer-trabajo

---

