
# <p align="center">Introducción a Git</p>
## Objetivo
<p style="text-align: justify;">
El objetivo de la práctica es introducirnos en el uso de Git, que es un sistema de control de versiones distribuido, y en GitHub, que es un proveedor donde se alojan los repositorios. Familiarizarnos con las acciones que se pueden realizar tanto en Git como en GitHub, así como los comandos que se utilizan y las situaciones en las que se deben usar.

Para ello se utilizó la creación de una carpeta; dentro de ella se creó un pequeño programa en lenguaje Python que imprime en pantalla un mensaje, el cual fue modificado para visualizar el control de versiones que nos brinda Git.
</p>

## Como ejecutar el programa

<p style="text-align: justify;">
Para ejecutar el programa que se encuentra en el repositorio, tenemos que hacer una copia de ese repositorio  en nuestra computadora. Para ello, realizamos lo siguiente: 

Usar el comando `git clone URL-del-repositorio "nombre de la carpeta donde se guardará la copia"`.

Una vez con la copia en nuestra computadora, abrimos la terminal. Dentro de la terminal, nos posicionamos en la carpeta donde está nuestro programa con el comando `cd` seguido de la ruta de la carpeta. Posteriormente, escribimos `python "nombre de nuestro programa"` y debemos observar en pantalla el mensaje que tiene nuestro programa.
</p>

## Comandos utilizados

### Inicialización del cliente

- `git config --global user.name "Nombre Usuario"`: asignar nombre de usuario
- `git config --global user.email miEmail@mail.com`: asignar correo de usuario

### Inicializar repositorio local

- ` git init  `: inicializar repositorio
- ` git remote add ALIAS URL-GIT-REPOSITORIO-REMOTO `: asociar repositorio remoto
- ` touch .gitignore `: ignorar archivos que no son importantes
  
### Enviar cambios al repositorio remoto

- ` git add -A`: Enviar archivos al área de preparación 
- ` git commit -m "mensaje del commit"`: enviar archivos al repositorio local
- ` git push ALIAS NOMBRE-RAMA `: enviar cambios del repositorio local al repositorio remoto

### Estos comandos no se utilizaron, pero son importantes 

- ` git status`: estatus de los archivos 
- ` git clone URL-REPOSITORIO`: copiar repositorio remoto en repositorio local 
- ` git pull ALIAS NOMBRE-RAMA`:  actualizar cambios de repositorio remoto en repositorio local

## Notas sobre el archivo .gitignore

<p style="text-align: justify;">
El archivo `.gitignore` se crea para evitar que archivos se compartan en el repositorio remoto, ya que no se necesitan. Estos archivos pueden ser archivos de compilación, archivos temporales o archivos de depuración, como el que nosotros ignoramos.

Al ejecutar el programa desde otra computadora, se creará el archivo ignorado si es necesario; de lo contrario, se ejecutará de manera adecuada.

Para verificar que el archivo no se subió, revisamos que en el repositorio remoto no se encuentre dicho archivo.
</p>





