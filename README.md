<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400" alt="Laravel Logo"></a></p>


# Laravel 10 Vue 3
### Proyecto creado con Laravel 10, Jetstream, Inertia, Vue 3, Vite, ElementPlus.

## Descripción


Contiene las configuraciones iniciales para que puedas empezar tu aplicación dejando todo listo en minutos.

Con la magía de docker no tendrás que preocuparte de versiones ni instalaciones.

Estas instrucciones están realizadas para ser seguidas desde windows, no se ha probado desde Linux ni Mac.

## Requisitos

- Sistema operativo Windows
- Tener Instalado Docker Desktop <a href="https://youtu.be/9AZAVlknsVI">Video como instalar Docker Desktop acá</a>
- Tener Instalado Wsl2  <a href="https://youtu.be/9AZAVlknsVI">Video como instalar Wsl2 acá</a>
- Tener Configurado Docker Desktop  <a href="https://youtu.be/9AZAVlknsVI">Video como configurar Docker Desktop acá</a>
- Tener instalado Git

## Instrucciones en Windows

Abre el terminal wsl2 (Terminal linux en Windows) en la carpeta donde guardaras tu proyecto. Puedes clonar con `SSH` o `HTTPS`

Clonar con SSH
(Si no tienes configuradas tus llaves SSH en GitHub puedes mirar este [tutorial para configurar llaves SSH](https://platzi.com/tutoriales/1557-git-github/4067-configurar-llaves-ssh-en-git-y-github/) )


    git clone git@github.com:santiagoInostroza/Laravel10Vue3.git
    

Si no quieres configurar tus llaves SSH puedes:
Clonar con HTTPS


     https://github.com/santiagoInostroza/Laravel10Vue3.git


Ingresa a la carpeta


    cd Laravel10Vue3 
    
    
Abre vs code

    code .
    
Asegurate que docker este corriendo y de preferencia no hayan contenedores cargados e ingresa el siguiente comando: 

    docker run --rm \
    -u "$(id -u):$(id -g)" \
    -v $(pwd):/var/www/html \
    -w /var/www/html \
    laravelsail/php81-composer:latest \
    composer install --ignore-platform-reqs

Este comando usa un pequeño contenedor Docker que contiene PHP y Composer para instalar las dependencias de la aplicación

Copia archivo .env


    cp .env.example .env

Reemplaza en el .env recien creado estas variables

    DB_HOST=mysql
    DB_USERNAME=sail
    DB_PASSWORD=password

Corre Sail

    ./vendor/bin/sail up     
    
Crea llave de la aplicación

    ./vendor/bin/sail artisan key:generate


    
    
Instala Npm


    ./vendor/bin/sail npm install
   
    ./vendor/bin/sail npm run dev


Finalmente <a href="http://localhost" >Abre localhost</a>
