# TechnicalDocumentation
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

![Image](https://lh3.googleusercontent.com/NCmgHhv5ZMu_8JWRfMM4WH7KentSHDmONfsBH5dBDTm1XBAcvrAZn6o59_33W9KRa2MtWFTprhz8DtrmnbiT_sxF7TtHd2ZNJmXNtxvomniuslz73WNbqJVrXRrQnCcHo9F_x-a_j0IUP9P-YZcLF3YytV90cgRHxA8nGvM4jJYL5K-PWnqkZFLyNnVxRnhNLeSGgnh_SHy6v9uK3Vd-QHqVMqT7BdPouCjPC89JXo2IeM3ZUeToJVF4qFBE2-eJa-J478IXVa79jqe_S60pPxZS5dg1WiSrIR7-CWO1y0zcD4yMA94Bl1wKJ-CnZs-HPmB0loo3lkfE-6YrK1XCjIZ7VY2GQAKmvCnWXDZtzzP1iBa8OKCWOxKTkFCjZyoxGiU4nVfK0e8fhQKg1jSBkDGpMYFTTG_qTJBHWa8vuRB15EAOG123UIQZbY6t9Os0Nv2Fm8hLvMnlPePdYhlZ8get77HDlRXpoAAbX2qqzuxyKZVc7TDqehbm6dzUwPUzfpul-1wBE7sf2L5pLrItcxGy0wePwEhby4n7sm5WgjhLXV0143CPB3OgJobUoJzl6TYRBkTCdqaxmjKVWkmgN-oYUcrhR10AmohjZgileQz4AECtk_XBxYVKcWrsuKkFGJNHetqn1AL_cW9MIvmFtXEFMEWLbkE=w1920-h628-no)

Vamos a las opciones de FUNCTION CODE y seguimos los pasos de la imagen.

Para el punto tres de la imagen el texto que se pone lo encontramos en el archivo aws-lambda-tools-defaults.json de la solución de la lambda.

En el punto cuatro de la imagen se sube el .zip generado en el segundo paso.  
