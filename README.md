# Tarea 2.4 Despliegue de un Sistema LMS Moodle con GitHub/Docker en una Mac Pro 2019-Equipo 2.

Este es una documentación para el despliegue de la aplicación de ***Moodle*** con una infraestructura basada en contenedores de ***Docker***:

Si deseas realizar este despliegue, puedes obtenerlo clonando el repositorio:

~~~
git clone <URL>
~~~

***Nota:*** Esto clonará el repositorio actual con sus archivos.

---

A continuación, ingresa al ***directorio clonado***.

---
## Paso 1. Entrar al directorio de moodle.

~~~
cd moodle
~~~

Entrar al directorio del ***moodle***.

---
## Paso 2. Compilar el docker-compose.yml.

~~~
docker-compose up -d
~~~

Compilación de archivo `docker-compose.yml`.

***Nota:*** Si desea detener la ejecución puede en algún momento más adelante, puede ejecutar el comando:

~~~
docker-compose stop
~~~

Y para iniciarlo nuevamente:

~~~
docker-compose start
~~~

---
## Paso 3. Ingresar al Moodle.

Ingrese a su ***browser favorito*** y coloque la `URL`:

~~~
localhost:80
~~~

Esto debería desplegar un panel de ***Moodle***.

***Nota:*** Podrá iniciar sesión de haciendo ***click*** en ***login***.

	El usuario es: user.
	La contraseña es: bitnami.

---
## Paso 4. Creación de cursos.

Una vez dentro del ***moodle*** podemos crear cursos, para ello, debemos navegar por los apartados:

	- Courses/category 1/manage courses and categories/Add new course

Lo que permitirá ingresar los datos para la creación de un ***nuevo curso***:

![Descripción de la imagen](./imgs/new-course.png)

Ingrese los datos:

![Descripción de la imagen](./imgs/new-course-2.png)

Haga ***click*** en el botón crear para crear el curso:

![Descripción de la imagen](./imgs/new-course-3.png)

De esta manera habrá creado un n***uevo curso***.

---
## Paso 5. Creación de usuarios.

Para la creación de usuarios: deberá navegar por los apartados:

	- Users/Add a new user

![Descripción de la imagen](./imgs/new-users.png)
![Descripción de la imagen](./imgs/new-users-2.png)

Aquí podrá crear sus usuarios como desee:

![Descripción de la imagen](./imgs/new-users-3.png)

---
## Paso 6. Asignación de usuarios a cursos y roles.

Para agregar usuarios creados a un curso, debemos ingresar al apartado de:

	courses/

E ingresar al curso que desea ingresar a sus participantes, dentro seleccionar el apartado:

	Participants/Add new user

![Descripción de la imagen](./imgs/add-user-courses.png)

Donde podrá ingresar sus usuarios ya creados y asignar sus roles.

---

