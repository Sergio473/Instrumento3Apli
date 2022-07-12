# Instrumento3Apli
Comandos Django

1. Primero que nada entramos a el directorio donde crearemos nuestro entorno
![image](https://user-images.githubusercontent.com/90642664/178550652-8d48403e-daa7-4fae-b3e5-cfaa02f1864a.png)

2. Creamos una carpeta dnetro de este y luego accedemos a ella 
![image](https://user-images.githubusercontent.com/90642664/178551940-8d04ad12-4932-4a29-9eae-5b464233d2ef.png)

3. Después crearemos el entorno venv con el comando python -m venv (nombre de carpeta)
![image](https://user-images.githubusercontent.com/90642664/178567813-552a5f15-8495-4d4d-a076-ef4c595e4be5.png)

4. Una vez creado el venv accederemos a el mediante el nombre_del_entorno\Scripts\activate y luego instalaremos django dentro de este
![image](https://user-images.githubusercontent.com/90642664/178562945-d8bfe66a-c09e-482c-b283-fde5b24aa9e2.png)

5. Luego de haberse instalado, lo siguiente sera crear el esqueleto con el comando django-admin startproject ProyectoFinal
![image](https://user-images.githubusercontent.com/90642664/178565385-267e504f-5f6f-48e6-8cf1-8879dad9ec7e.png)

6. Luego migraremos los datos, utilizaremos primero acceder a la carpeta antes creada y luego ejecutaremos el siguiente comando python manage.py migrate
![image](https://user-images.githubusercontent.com/90642664/178566178-5160e29a-84b8-41e4-ad4e-004762197db8.png)

7. Por último corremos el proyecto y comprobamos.
![image](https://user-images.githubusercontent.com/90642664/178566427-f039ad48-f53a-4bc8-be37-08b05670c9c5.png)

Luego crearemos una aplicación llamada student, para esto ejecutamos el siguiente comando python3 manage.py startapp catstudent. Como observan yo ya lo tengo creado.
![image](https://user-images.githubusercontent.com/90642664/178576070-157874ed-3a78-40e7-8b50-b2f2c78a8998.png)

Luego modificaremos las view.py para crear una vista unica de página de inicio
![image](https://user-images.githubusercontent.com/90642664/178576559-eaf28a9c-65aa-4984-b5ea-112879f3a7d1.png)

Después modificaremos urls.py para enrutar diferentes urls a sus vistas apropiadas
![image](https://user-images.githubusercontent.com/90642664/178576742-f65c3986-c269-482d-b2c3-ea6838b69e49.png)

También modificaremos nuestra urls.py de nuestro esqueleto que es donde realmente se maneja el enrutamiento
![image](https://user-images.githubusercontent.com/90642664/178577064-dc5ea731-1c7a-4a18-8ee4-b9281f1c01cb.png)

Registrar Aplicación

Para el registro nos iremos hasta settings.py y ahi os iremos hasta donde esta installed_apps y añadiremos la siguiente linea 'catstudent.apps.CatstudentConfig' para la configuración de la aplicación
![image](https://user-images.githubusercontent.com/90642664/178578500-966d6f34-4d2a-4500-a5b6-861b8a28079e.png)

Especificación de a base de datos

Nos dirijimos hasta Databases en la misma pestaña de settings.py y pondremos la siguiente linea 'NAME': os.path.join(BASE_DIR, 'db.sqlite3') que especifíca que usaremos sqlite3

![image](https://user-images.githubusercontent.com/90642664/178579886-b62f7fa4-37a1-4969-8d5d-5004cc738837.png)

Igual modificaremos el TIME_ZONE para que le idiquemos la zona en la que nos encontramos ubicados y tome esa hora

![image](https://user-images.githubusercontent.com/90642664/178579932-a4427d69-986d-461c-b549-5e9b88c5d99f.png)

Base de Datos







