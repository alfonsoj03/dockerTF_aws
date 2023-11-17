Para posibilitar la subida a GitHub me vi obligado a dividir el proyecto en tres comprimidos, para descomprimirlos es necesario descomprimir los tres juntos en uno sólo.

Proyecto de Despliegue de Aplicación Web con Terraform en AWS
Este proyecto utiliza Terraform para desplegar una aplicación web HTML en una instancia de Amazon Web Services (AWS). Una vez ejecutado terraform apply, la aplicación estará accesible a través del puerto 80 (HTTP) en la dirección IP asignada a la instancia.

Requisitos Previos
Antes de comenzar, asegúrate de tener los siguientes requisitos:

Terraform instalado en tu máquina local.

Credenciales de AWS configuradas en tu entorno local.

Despliegue:

Clona este repositorio a tu máquina local.

Inicializa terraform

terraform init

Ejecuta el siguiente comando para aplicar la configuración de Terraform:

terraform apply

Una vez completado, se habrá creado una instancia llamada "appDocker" en AWS.

Acceso a la Aplicación

La aplicación estará disponible en el puerto 80 de la dirección IP de la instancia EC2 en AWS. Abre tu navegador web y navega a http://<IP_de_la_Instancia>.

Nota Importante

Para garantizar el funcionamiento óptimo de la aplicación, es crucial que no haya ninguna instancia duplicada de la que este proyecto va a crear en la cuenta de AWS. Esto puede generar conflictos y afectar el comportamiento esperado de la aplicación web.
