# STAGE 0
Hacemos una lista de los paquetes que tenemos instalados junto con la version de cada uno, lo ponemos en el *requirements.txt*

<img width="437" height="102" alt="image" src="https://github.com/user-attachments/assets/1cd659a4-d383-4d7a-95ba-92324ed2a3de" />

Luego hacemos un compose aplicanco ciertos parametros por ejemplo command que hace de cmd y el restart para que el contenedor se reinicie solo si se cae
<img width="746" height="190" alt="image" src="https://github.com/user-attachments/assets/e9e5fb9a-fbcc-482e-a3a1-a815db8894ec" />

Ponemos el docker con los valores que queremos
<img width="577" height="169" alt="image" src="https://github.com/user-attachments/assets/2208f76e-ab36-4e5a-81e6-3b816a9c3410" />

# STAGE 1

Añadimos gunicorn, para que funcione todo bien quitamos todos los django_browser_reload de urls.py y settings.py que tenemos. Tambien del wsgi.py si esta

<img width="414" height="127" alt="image" src="https://github.com/user-attachments/assets/a3a4260e-6ef2-49b2-9f35-ab82645d7fbe" />

Añadimos requirements.txt el gunicorn

# STAGE 2

Creamos un default.conf en la carpeta nginx/conf.d/

<img width="817" height="510" alt="image" src="https://github.com/user-attachments/assets/95201b54-eb46-4432-a54c-fe083e30e222" />

Creamos tambien el compose

<img width="848" height="652" alt="image" src="https://github.com/user-attachments/assets/9b2bd59e-5302-48bf-a5a4-58ec62bd4613" />
