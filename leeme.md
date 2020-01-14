¡Script para automatizar el proceso de reconocimiento y enumeración!

Objetivo
Este script automatiza todo el proceso de reconocimiento y enumeración que se ejecuta a la hora de realizar una prueba de penetración, centrando nuestra atención en los resultados finales y disminuyendo el tiempo a la hora de una auditoría.

Una vez que encuentre los puertos iniciales en aproximadamente 10 segundos, puede comenzar a buscarlos manualmente y dejar que el resto se ejecute en segundo plano sin interacción alguna de su parte.

Ventajas

La herramienta es precisa. 
Es muy rápida 
Tiene todos los escaneos básicos incluidos 
El usuario puede profundizar en los resultado del escaneo simple mientras se ejecuta el escaneo completo
Se puede usar en Hack The Box y Vulnhub para ahorrar tiempo.

Solo se necesita la “dirección IP” y el “Tipo de Escaneo” y el script buscará y analizará los puertos TCP y UDP abiertos.

Requisitos de Instalación

#apt-get update
#apt-get upgrade

El Script necesita de la instalación de Gobuster V3.0 o superior, Puesto que no es compatible con otras versiones anteriores a esta.

#apt-get install gobuster
#apt-get install gobuster --ony-upgrade

PERMISOS DE EJECUCIÓN

#chmod +x ultramat.sh

Ejemplos de uso
Utilice: 
#./ultramat.sh <Dirección IP> <Tipos de Escaneos>


#./ultramat.sh <Dirección IP> Rapido
#./ultramat.sh <Dirección IP> Basico
#./ultramat.sh <Dirección IP> Completo

Recomendado
Instalar nmap vulners "para escaneo de Vulnerabilidades CVE"
https://github.com/vulnersCom/nmap-vulners

Acceso Directo
Identificar la ruta del directorio actual
#pwd

Creación de un acceso directo:
#ln -s /RUTA_DE_CARPETA/ultramat.sh /usr/local/bin/

