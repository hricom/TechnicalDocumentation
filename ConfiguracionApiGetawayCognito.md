## Configuración de API GETAWAY con COGNITO.

1. Se ingresa a la consola de AWS en la opción **API GETAWAY**.
2. En las opciones se selecciona la API a la que se le va a configurar **COGNITO.**
3. Se selecciona la opción de autorización 
4. Se selecciona la opción crear.
5. se Selecciona la opción de **COGNITO**
6. Se agrega un nombre, selecciona el POOL creado y en el campo Token Source se copia el siguiente texto Authorization.
7. Click en crear.
![Image](https://github.com/hricom/TechnicalDocumentation/blob/master/images/Agc.PNG)
8. Se selecciona el Resources, luego el método (el verbo del BINDING) que se va a configurar.
9. Se selecciona la opción **method Request**
![Image](https://github.com/hricom/TechnicalDocumentation/blob/master/images/Agc1.PNG)
10. En la opción que se despliega de Authorization se edita y se guarda.
![Image](https://github.com/hricom/TechnicalDocumentation/blob/master/images/Agc2.PNG)

**Nota.**
La configuración mencionada en los pasos anteriores se puede hacer en su totalidad desde codigo.
