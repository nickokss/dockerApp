# dockerApp
Crear imagen de Docker para una aplicación. En este caso es una aplicación sencilla en Python.
## Instalar docker en LINUX (si aun no lo tenías instalado)
```sh
sudo apt-get update
```
```sh
sudo apt install docker.io -y
```
> [!TIP]
>Para que no pida contraseña cada vez que ejecutamos un comando docker
>```sh
>sudo usermod -aG docker $USER
>```
* Reiniciar PC

## Pasos para dockerizacion de la aplicación
* Instalar Docker en el Sistema Operativo en este caso se usa LINUX. En Windows puedes usar la aplicación "Windows Subsystem for Linux"
* Guardar en una ruta el código de la app (app.py). Por ejemplo: C:\apps
* En la misma ruta guardar el fichero requeriments.txt
* Tambien en la misma ruta guardar el fichero Dockerfile
* Abrimos una consola y nos situamos en la ruta donde están los 3 ficheros. Para crear crear la imagen ejecutamos el siguiente comando (El punto del final se usa para buscar el archivo en la ruta actual)
```sh
docker build -t mi_app .
```
* Usamos el siguiente comando para listar imagenes
```sh
docker images
```
* Usamos el siguiente comando para ejecutar el contenedor
```sh
docker run -p 4000:5000 mi_app
```
* Por último para ver la aplicacion vamos al navegador y ponemos la ruta que nos indique en la consola


