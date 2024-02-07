# dockerApp
Crear imagen de Docker para una aplicación. En este caso es una aplicación sencilla en Python.

## Pasos para dockerizacion de la aplicación
* Instalar Docker en el Sistema Operativo en este caso se usa LINUX en Windows puedes usar la aplicación "Windows Subsystem for Linux"
* Guardar en una ruta el código de la app. Por ejemplo: C:\nickokss\app.py
* En la misma ruta guardar el fichero requeriments.txt
* Tambien en la misma ruta guardar un fichero Dockerfile
* Para crear crear la imagen ejecutamos el comando donde definimos el tag (El punto del final se usa para buscar el archivo en la ruta actual)
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
* Por último para ver la aplicacion vamos al navegador y ponemos la ruta "localhost:4000"
