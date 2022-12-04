# Computación Tolerante a Fallas - UDG Social

## Autores

- **Camarena Miranda Eric Omar**
- **Correa Bañuelos José Manuel**
- **Ortega Cuevas Diego Enrique**

## Descripción

Para el proyecto de tolerante a fallas decidimos por hacer una red social denominada como UDG Social el cual funciona como Instagram en donde los usuarios se pueden registrar, logear o incluso visualizar perfiles si no te encuentras logeado, a su vez tambien puedes interactuar dándole seguir a los usuarios y dando like a las publicaciones de otros usuarios.

## Tecnologías utilizadas

Para este proyecto optamos por varias tecnologías para llevarlo a cabo, a continuación se explicara mas a detalle cada una.

**Laravel:** El framework de laravel es el cerebro de nuestra aplicación debido a que con el hicimos la mayoría de las funciones, controladores y modelos que nos permiten que el usuario interactúe.

**TailwindCSS:** Debido a que nadie de nosotros era un experto en CSS puro, optamos por usar el framework TailwindCSS el cuando nos permitió darle un buen terminado a la parte de la interfaz debido a que con las clases que maneja hace que todo sea mas fácil.

**JavaScript:** JavaScript lo implementamos para poder traer dropzone a nuestro proyecto el cual es lo mas fundamental para poder subir imágenes ya que es lo que lo permite.

**Docker:** Docker lo empleamos para poder manejar el proyecto con contenedores asi no es necesario tener que instalar todos la misma versión de php debido que como todo se corre directo de una imagen ya generada esto permite que no estemos batallando por instalar la misma versión idéntica, al igual hicimos uso de los contendedores también para correr una imagen de MySQL y otras cuantas de laravel.

---

## Capturas de pantalla

                                                                      **Inicio de sesión** 

(https://github.com/JoMaCoBa/UDG-Social/blob/main/Capturas/login.png)

---

                                                               **Formulario de Registro**

(https://github.com/JoMaCoBa/UDG-Social/blob/main/Capturas/Registro.png)

---

                                                                   **Muro del Usuario**

(https://github.com/JoMaCoBa/UDG-Social/blob/main/Capturas/Muro.png)

---

                                              **Vista de home (’Desde otro usuario’)**

(https://github.com/JoMaCoBa/UDG-Social/blob/main/Capturas/Inicio1.png)

---

                                **Vista de home (’Desde un usuario que no sigue a nadie’)**

(https://github.com/JoMaCoBa/UDG-Social/blob/main/Capturas/Inicio2.png)

---

                                                        **Vista para publicar post**

(https://github.com/JoMaCoBa/UDG-Social/blob/main/Capturas/Post.png)

---

## Instalación del proyecto

Para instalar el proyecto primero haces un git clone con el enlace del repositorio:

```jsx
git clone https://github.com/JoMaCoBa/UDG-Social.git
```

Una vez hecho el git clone es necesario tener instalado docker y tenerlo abierto y despues de eso abres la terminal y rediriges a la carpeta en donde hayas guardado el proyecto para procedes en la terminal a teclear los siguientes comandos:

```jsx
wsl //Esto permite abrir la terminal de linux en windows
sail up // Sail up nos permite arrancar el proyecto y asi iniciar los contenedores en docker
```

Despues de haber usado los comandos pasados abres una nueva terminal y otra vez te redireccionas a la carpeta en donde tengas el proyecto y procedes hacer el siguiente comando el cual permite correr tailwindcss:

```jsx
npm run dev
```

Después de haber hecho te arrojara en la terminal el link de [localhost](http://localhost) el cual puedes hacer que te lo abra en el navegador pulsando ctrl+click encima del enlace.

Todavía no cantes victoria te falta tener la base de datos requerida pero gracias a las migraciones de laravel y a que estamos corriendo MySQL en una imagen de Docker solo procedes a ejecutar el siguiente comando:

**Nota:** este comando igual lo debes ejecutar en la terminal desde la carpeta del proyecto y debe ser ejecutado con la terminal de Linux “wsl” si no te marcara error y no se podrán realizar las migraciones.

```jsx
sail artisan migrate
```

Y eso seria todo para poner en marcha el proyecto y ya puedas hacer las modificaciones e implementaciones que desees.

---

## Video de Demostración

En dado caso que las instrucciones te parecieran confusas o deseas una explicación grafica a continuación dejamos un video en el cual mostramos como poner en arranque el proyecto y a su vez una demostración de lo que hace el proyecto:

[https://drive.google.com/file/d/1fhoBwHub6Db1u2qKOMdynPNy6DPpaa3f/view](https://drive.google.com/file/d/1fhoBwHub6Db1u2qKOMdynPNy6DPpaa3f/view)
