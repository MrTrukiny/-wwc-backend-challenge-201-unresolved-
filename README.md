# ¡¡Reciban una bienvenida a la línea de Backend de los #codechallenges de #WWC 2020!!

## Este es el reto #1

    *** Lee detalladamante toda la información de este README ***

- **Nombre:** LA SÚPER PARTY
- **Dificultad:** fácil
- **Habilidades:** creación de servidor con express; uso de rutas, estatus y respuestas; almacenamiento de información en archivos; uso de middlewares; lógica básica
- **Descripción:** 
Eres el vigilante de una fiesta UNDERGROUND que se hará el próximo sábado en la Ciudad y debes registrar los asistentes.
Lo más importante es: registrar su nombre, su fecha de nacimiento y que no tengan fiebre. Si se niegan o no cumplen con los
requisitos, no pueden ingresar... ¡¡UPS!! :( 

## Instrucciones
+ Descarga este repositorio y haz `cd oop-backend` o `cd func-backend` según el tipo de backend que desees.
+ Ejecuta `npm install` y luego `npm run dev` para tener tu servidor corriendo.
+ Encontrarás un boilerplate con una arquitectura de tipo "MVC" (aunque sin la V :P). La idea es que trabajes en él para que se te haga más fácil completar el reto, pero puedes borrarlo y empezar desde cero. Lo importante es que cumplas las siguientes condiciones:
  + Crearás un endpoint que apuntará a `'/users'` con dos métodos: **GET** y **POST**.
  + El método **POST** creará un asistente nuevo en el archivo _db.json:_ que se encuentra en `./src/_data` y tendrá los siguientes datos:
  ```javascript
    nombre, requerido
    fecha de nacimiento, requerido, formato sugerido "YYYY-MM-DD",
    temperatura, requerido
    correo electrónico, opcional
    color de la prenda principal, opcional
  ```
  + Cada asistente se guardará con un `id` que será generado automáticamente por la aplicación, empezando desde **1** y será de tipo **_number_**.
  + El método **POST** retornará el nuevo asistente creado con su respectiva información y un **status 201**.
  + Si el asistente no da su nombre o su fecha de nacimiento o su temperatura no se encuentra entre **36.5 - 37.5** grados centígrados, no podrá ingresar (no se guarda en la db), y retornarás un mensaje diciendo que _paila, no puede entrar_ y un **status 400**.
  + No vamos a verificar si es mayor de edad, sólo con ingresar la fecha basta (shhh).
  + El método **GET** retornará la lista de asistentes con la información de cada uno y un **status 200**. Si la lista está vacía, retornará un mensaje diciendo que _no hay nadie partyseando aún_ y un **status 200**.
  + Crea un **middleware** que se encargue de mandar un mensaje de _página no encontrada_ para cualquier endpoint que no sea `/users` y retorne un **status 404**.
  + Los mensajes que devuelve la aplicación quedan a tu creatividad.
  + Los nombres de las propiedades de cada asistente y la estructura de la información serán decisión tuya.

### Notas:

**Encontrarás dos carpetas:**
  * _oop-backend_: Trabaja aquí si prefieres un backend "orientado a objetos" que opere a través de clases.
  * _func-backend_: Trabaja aquí si prefieres un backend que apunte a un modo de operación funcional :O.

* Puedes resolver el reto en cualquiera de ambos. Sólo se revisará una. Hacer el reto en ambos no te dará más puntaje, pero sí más experiencia.
* Esto lo hacemos para que conozcas dos paradigmas diferentes de trabajo que son posibles gracias a la "flexibilidad" de JavaScript.

## ¡¡NOS VEMOS EN EL RETO NÚMERO 2 PARA QUE VER EN QUE RESULTA ESTA FIESTA!! 
# ¡¡DIVIÉRTANSE!!
