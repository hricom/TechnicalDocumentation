# Technical Documentation
Technical Manuals

## LAMBDA  en .netcore
Despliegue manual.
* ***Requisitos.***
* Se debe tener instaladas las siguientes herramientas:

AWS Toolkit for Visual Studio

AWS CLI

Amazon.Lambda.Tools (Este se instala desde el CMD con el siguiente comando dotnet tool update -g Amazon.Lambda.Tools).

* ***Pasos.***
1. Teniendo la implementación, pararnos en la raíz del proyecto perteneciente al presentación, para esto debemos estar en el CMD.
* Ejemplo.

  cd "proyecto/src/solución"
  
2. Ahora se ejecuta el siguiente comando 

  dotnet lambda deploy-function

Esto genera un compilado en .ZIP en la raíz de la presentación dentro de la carpeta BIN.
* Ejemplo.

\bin\Release\netcoreapp2.1

3. Se ingresa a la consola de AWS, vamos a lambda y creamos una lambda básica con el nombre que va a quedar la lambda que se va a desplegar, esta será el contenedor de la lambda que se va desplegar.

Ingresamos a la lambda que creamos

![Image](https://github.com/hricom/TechnicalDocumentation/blob/master/images/Lambda.png)

Vamos a las opciones de FUNCTION CODE y seguimos los pasos de la imagen.

Para el punto tres de la imagen el texto que se pone lo encontramos en el archivo aws-lambda-tools-defaults.json de la solución de la lambda.

En el punto cuatro de la imagen se sube el .zip generado en el segundo paso.  
