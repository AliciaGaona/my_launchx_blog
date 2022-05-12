---
title: "Pasos para inicializar un proyecto en nodeJS"
date: 2022-05-11
description: 'Inicializar proyecto de nodeJS'
---

## BASES QUE CUALQUIER PROYECTO NECESITA

Conjunto de folders y archivos para organizar nuestro código
Versionamiento con git.
Puede incluir dependencias.
Todo proyecto lleva PRUEBAS DE UNIDAD. (No negociable)


__Cuida del orden para que el orden cuide de ti by @Carlo Gilmar__

## Intalar la ultima versión de nodeJS.
## Escoger tu editor de texto favorito.

En mi caso uso Visual Code.

## Usar y conocer tu SO en su línea de comandos.

En mi caso windows 10.


1. Crear un proyecto nuevo.

2. Inicializar el proyecto agregando package.json ▶️  npm init (Recuerda siempre VERSIONAR tus apps)

![image](https://user-images.githubusercontent.com/99162884/167997193-ec6236ab-c911-4ac4-9006-27229decbd22.png)

![image](https://user-images.githubusercontent.com/99162884/167997259-02c061f9-e73a-42f6-8b8b-b90410dbdcf2.png)

![image](https://user-images.githubusercontent.com/99162884/167997314-a8879a24-b6c4-459c-ac34-7fe9972e8b2b.png)

3. Una vez inicializado nuestro proyecto, ya podemos comenzar a instalar las dependencias que usaremos.

- npm install --save-dev jest

Verifica que depués de esto se haya creado un directorio llamado __node_modules__ este contiene todos los scripts de js de las dependencias.

__RECUERDA NUNCA VERSIONARLO__ : para evitar que se versione creamos en la RAÍZ del proyecto un archivo llamado .gitignore con el nombre de lo que no quieras versionar, en este caso: **/node_modules , con esto vamos a decirle a git que excluya este directorio de los commits que realicemos.

Mira todos estos cambios pendientes antes de crear el archivo .gitignore

![image](https://user-images.githubusercontent.com/99162884/167998798-61b1703d-9ab7-4253-8775-0f324a765639.png)

Creando .gitignore

![image](https://user-images.githubusercontent.com/99162884/167999055-822399c0-10c5-453f-8081-427f81b042d1.png)

Fijate como después de instalar Jest, el corazón de nuestra app lo registra.

![image](https://user-images.githubusercontent.com/99162884/167999333-e96c8a50-179d-4247-9c10-7b6ae503214d.png)


4. Crea la estructura de tu proyecto, las carpetas donde iran tus archivos y tus pruebas unitarias etcetc.

Por ejemplo en LauchX usamos dos directorios principales(app y test), en app van todas nuestras clases y se duplica todo en test para que cada fucnionalidad tenga su prueba unitaria.

Regla de oro: Por cada funcionalidad primero se hace una prueba unitaria.

5. Creación de prueba unitaria, la idea es hacerla fallar y pensar en todos los escenarios, y despues hacer que pase.

Partiendo de ahi, crear la funcionalidad.

6. Crea un archivo en la raíz de tu proyecto que se llame index.js. Este será el archivo principal de este proyecto e inicializalo en tu package.json

![image](https://user-images.githubusercontent.com/99162884/168000977-c89780a8-1af4-4e95-be1c-f0004073ef9f.png)

7. Ve a tu archivo package.json, y modifica la línea que inicia con "test" por:

node ./node_modules/jest/bin/jest.js" (puede variar dependiendo del sistema operativo)

Con esto , podremos activar el comando npm test y correr las pruebas

__El script del package.json se usa para declarar la palabra con la que vamos a inicializar alguna dependencia instalada__




## DEPENDENCIAS

- Jest - es una librería abierta para pruebas en JavaScript desarrollada por Facebook. Su eslogan es "Pruebas de JavaScript deliciosas".

[Documentación Jest](https://jestjs.io/docs/api)



## PRUEBAS DE UNIDAD


## GLOSARIO

- NPM (Node Package Manager) es un gestor de paquetes de js que nos permite obtener cualquier librería, nos permitirá agregar y usar dependencias de forma simple.

- npm init - activará la inicialización de tu proyecto, se generará un archivo package.json y se guardará en el directorio actual.

- archivo package.json - el corazón de tu proyecto ❤️,  maneja todas tus dependencias y referencias.

- VERSIONAR tus apps - usar git como un diario de commits de loq ue vas haciendo, te recomiendo este contenido que lo explica muy cool

[Curso Git by Carlo Gilmar](https://carlogilmar.gitbooks.io/git-course/content/)

- Depencia JS - bibliotecas de js que nos facilitan la vida 

- __node_modules__ este contiene todos los scripts de js de las dependencias, __RECUERDA NUNCA VERSIONARLO



