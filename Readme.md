# Comandos Basicos
1. Debemos descargar una imagen, en este caso de ubuntu _*docker pull ubuntu*_. Sabemos que ha funcionado porque usamos _*docker images*_
2. Creamos un contenedor con la imagen que descargamos (usamos _*docker run ubuntu*_), para comprobar que todo haya funcionado usamos _*docker ps*_. Con el comando listamos todos los contenedores
3. Creamos un contenedor con la imagen y un nombre personalizado usamos, _*docker run -it --name dam_ubu1 ubuntu*_. Con el apartado -it entramos directamente