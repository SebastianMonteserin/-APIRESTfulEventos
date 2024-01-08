# -APIRESTfulEventos
Servidor con NODE.JS, de una app para organización y manejo de eventos sociales.


El proyecto consistirá en la creación de un Servidor con NODE.JS, de una app para organización y manejo de eventos sociales, como por ejemplo eventos deportivos, festivales musicales, encuentros de grupos de fans, etc. 

La API utiliza el modelo MVC, trabaja con MongoDB, posee un generador utilizando faker, validaciones con Joi y realiza Test con Chai y Supertest.

La API también se conecta con un servidor que provee datos del clima en la fecha de lso eventos, los que nos proporciona la predicción meterologica ( en un rango de 10 dias).


El proyecto se centrará en el manejo y la persistencia de dos colecciones - eventos y usuarios- mediante la implementación del patrón MVC.

En esta primera etapa, la funcionalidad de nuestra aplicación se ciruscribirá a dar respuesta a estas Historias de Usuario:

1.	-Como un usuario externo, quiero poder registrarme para poder utilizar la aplicación de eventos.

2.	-Como un profesional del ciclismo, quiero poder crear un evento que refleje una carrera de bicicletas, para que todo usuario que quiera pueda participar

3.	-Como un entusiasta del ciclismo, quiero poder suscribirme al evento de mi deporte favorito para poder participar y recibir información del evento.

4.	-Como un usuario registrado, quiero poder ver el clima que del dia de cada evento para evaluar mi participación.

5.	-Como un usuario registrado suscripto, quiero poder ver una lista de los eventos en los que estoy inscripto


Se utilizará como base de datos MongoDB.

Se implementará un sistema de login con manejo con sesiones con jwt.

Asimismo, el Servidor va a conectarse a una API externa que nos provea la predicción del clima para el día y lugar del evento indicado.

Documentación de los endpoints y casos utiles de prueba: Postman : https://documenter.getpostman.com/view/15015098/2s9YeAAuqm

Estructuras de Datos:

Evento:
- Creador
- Título 
- Categoría 
- Fecha
- Suscriptores
- Cantidad de Participantes Max

Usuario: 
- Nombre
- Contraseña
- Eventos Creados
- Eventos Asociados

# Prueba
-Priemro se debe poner en consola en la ruta del poryecto "npm isntall"
-Se debe contar con una Base de datos Mongo DB interna, a la cual se inicia desde consola con el comando  mongod --dbpath="./ nombrebase"  en la ruta donde hubicaremos el archivo.
- Corremos con npm run watch
-Podemos probar los endpoints con los ejemplos que están en el siguente enlace: https://documenter.getpostman.com/view/15015098/2s9YeAAuqm

