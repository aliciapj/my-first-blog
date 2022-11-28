# Bienvenida a tu primer blog con django

Cómo ejecutar el proyecto:
1. Haz un fork del proyecto en tu propio repositorio
2. Descarga el proyecto del repo con git
3. Crea un entorno virtual
4. Activa el entorno virtual
5. Instala las librerías del `requirements.txt`
6. Genera las migraciones del proyecto con `python manage.py makemigrations`
7. Ejecuta las migraciones en la base de datos con `python manage.py migrate`
8. Carga los datos iniciales del fichero `db.json` con `python manage.py loaddata db.json`
9. Ejecuta el servidor de django para probar la aplicación

Puntos extra:
* Crea tu propio usuario superuser para poder entrar en el admin de django.
   Para ello, crea como variables de entorno los siguientes parámetros:
   - `export DJANGO_SUPERUSER_PASSWORD='my-password-here'`
   - `export DJANGO_SUPERUSER_USERNAME='my-username-here'`
   - `export DJANGO_SUPERUSER_EMAIL='my-email-here'`
   A continuación, llama al comando para crear un super-usuario con la opción `noinput` así:
   - `python manage.py createsuperuser --noinput`