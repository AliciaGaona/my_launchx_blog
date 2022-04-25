---
title: "Mi experiencia usando Git"
date: 2022-04-24
description: 'Te cuento la experiencia que voy tieniendo respecto a Git'
---

---
## NUNCA USES LOS COMANDOS DE GIT COMO UN RECETARIO by Carlo Gilmar
---


Hay que entender bien las bases de git y el porque de cada comando, te recomiendo este curso de [Bases de Git by Carlo Gilmar](https://carlogilmar.gitbooks.io/git-course/content/chapter2.html) , 
a mi me ha ayudado mucho a entender que pasa con Git.

Primeramente algo que me sirvio muchisimo fue entender como es que funciona git con github, digamos que tienes tu proyecto en tu local(tu equipo) y tienes ese mismo remoto,
en este caso en la plataforma de Github. Por lo tanto tienes que asegurarte de tener los dos actualizados y oreganizados, para lo cual nos ayuda mucho el control de versiones, 
en cada commit puedes registrar que vas haciendo y esto dará orden y legibilidad a tu proyecto.

---

# Entendiendo lo anterior yo lo podría resumir muy muy general en:

  🚀Clonar mi repositorio de Github en mi local.
  
  Para lo cual te recomiendo crear una Clave de SSH, para puedas usar la url de SHH, y que no te este pidiendo ingresar tus credenciales cada que quieras realizar algo.
  Justo aqui encuentras la url de SHH.
  
  ![image](https://user-images.githubusercontent.com/99162884/165003651-1bd441ae-c8ec-4e5a-a00c-71f89b320006.png)
  
  ¿Que es una clave SHH?
 Son credenciales que utilizamos para que el protocolo SSH (Secure Shell) permita el acceso seguro a ordenadores a través de Internet, 
 en pocas palabras crea un puente seguro entre tu ordenador e internet(tu repositorio remoto).
 
 Te comparto lo que a mi me funciono para crearla:
 
 Asegurate de tener instalado el sofware de git.
 En git bash o la terminal de tu sistema operativo, ingresa el siguiente comando =>  ssh-keygen -t rsa -b 4096 -C “tu_email@gmail.com” , aqui ingresamos el email al que 
 se va a configurar la llave (el que tengas registrado en tu cuenta de GitHub), despues nos pide una contraseña. docle enter.
 
 Y nos aparecerá un texto "The key´s randomart image is:", lo que significa que ya nos genero nuestra clave de SHH.
 
 Nos creará dos archivos, el que necesitamos es el que tiene el .pub(significa que es tu clave pública), la clave privada no se comparte.
 En una carpeta llaamada .ssh ahi podrás encontrarlos, o simplemte poner el comando ls, y copiar el nombre que tenga el .pub, copiamos el contenido
 y lo vamos a pegar en GitHub en el siguiente lugar:
 
 1. Te vas a Settings
 
![image](https://user-images.githubusercontent.com/99162884/165004879-1d06808d-f053-460c-a178-23ef27c736b2.png)
 
 2. SSH and GPG KeyS
 
 ![image](https://user-images.githubusercontent.com/99162884/165004906-7c011b38-ddf2-40d6-8ebd-0278a133ed7e.png)

 3. Agregar nueva
 
 ![image](https://user-images.githubusercontent.com/99162884/165004976-c96d60dd-d6ca-4689-be1b-19ee37d61f72.png)

 4.Le agregas un titulo y pegas el contenido de la clave publica de SHH.
 
 ![image](https://user-images.githubusercontent.com/99162884/165005048-7cc4a71a-3af3-4d1b-98d2-a2009d268a11.png)
 
 Listo ya puedes clanar tus repositorios sin que te este pidiendo tus credenciales o más problemas que surgen.
 
 
 # Puedes probar clonando un repositorio que tengas o hacer uno nuevo, y seria algo como:
 
 git clone url(url de ssh)
 
 
 

 
 

 
 

