# Comandos Basicos
1. Debemos descargar una imagen, en este caso de ubuntu _*docker pull ubuntu*_. Sabemos que ha funcionado porque usamos _*docker images*_
2. Creamos un contenedor con la imagen que descargamos (usamos _*docker run ubuntu*_), para comprobar que todo haya funcionado usamos _*docker ps*_. Con el comando listamos todos los contenedores
3. Creamos un contenedor con la imagen y un nombre personalizado usamos, _*docker run -it --name dam_ubu1 ubuntu*_. Con el apartado -it entramos directamente
4. Una vez dentro, para ver la ip tenemos que actualizarlo _*apt update*_. Despues tenemos que instalar net-tools _*apt isntall net-tools*_ (es donde esta el comando para ver la ip), una vez terminado usamos _*ifconfig*_. Si queremos hacer ping a google tenemos que instalar nslookup _*apt isntall nslookup*_ y _*nslookup google.com*_ . Para poder hacer el ping instalamos el _*apt isntall iputils-ping*_
5. Como cambiamos de contenedor habra que volver isntalar el net-tools, primero lo creamos y abrimos _*docker run -it --name dam_ubu2 ubuntu*_, ahora ya podriamos hacer ping entre ellos
6. Salimos usando exit, con _*docker ps -a*_ nos muestra como esta el conendor
7. Con _*docker stats -a*_ nos muestra lo que consume cada contenedor
8. Con _*docker stats -a*_ nos muestra las estadisticas