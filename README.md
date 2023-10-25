<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400" alt="Laravel Logo"></a></p>


<h1>Laravel 10 Vue 3 </h1>
<br><br>
<h2>Este proyecto está creado con Laravel 10, Jetstream, Inertia, Vue 3, ElementPlus</h2>
<br><br>
<p>Contiene las configuraciones iniciales para que puedas empezar tu aplicación dejando todo listo en minutos</p>
<p>Con la magía de docker no tendrás que preocuparte de versiones ni instalaciones</p>
<p>Estas instrucciones están realizadas para ser seguidas desde windows, no se ha probado desde Linux ni Mac</p>

<br>

<h2>Requisitos</h2>

<ul> 
    <li>
        Sistema operativo Windows
    </li>
    <li>
        Tener Instalado Docker Desktop
         <a href="https://youtu.be/9AZAVlknsVI">Video como instalar Docker Desktop acá</a>
    </li>
    <li>
         Tener Instalado Wsl2 
        <a href="https://youtu.be/9AZAVlknsVI">Video como instalar Wsl2 acá</a>
    </li>
    <li>
         Tener Configurado Docker Desktop 
        <a href="https://youtu.be/9AZAVlknsVI">Video como configurar Docker Desktop acá</a>
    </li>
    <li>Tener instalado Git</li>
</ul>
<br>


<br>
<h2>Paso a paso de la instalación del proyecto</h2>
<br>

<p>Abre el terminal wsl2 (Terminal linux en Windows) en la carpeta donde guardaras tu proyecto y copia los siguientes comandos</p>

<br>
<h4>Clonar proyecto con SSH</h4>


    git clone git@github.com:santiagoInostroza/laravel9-vue3-vite.git
    
    
<h4>o con HTTPS</h4>


     https://github.com/santiagoInostroza/laravel9-vue3-vite.git


<h4>ingresa a la carpeta</h4>


    cd laravel9-vue3-vite/ 
    
    
<h4>Abre vs code</h4>

    code .
    
<h4>Asegurate que docker este corriendo y de preferencia no hayan contenedores cargados.</h4>
<h4>Este comando usa un pequeño contenedor Docker que contiene PHP y Composer para instalar las dependencias de la aplicación:</h4>

    docker run --rm \
    -u "$(id -u):$(id -g)" \
    -v $(pwd):/var/www/html \
    -w /var/www/html \
    laravelsail/php81-composer:latest \
    composer install --ignore-platform-reqs
    
    

<h4>Corre Sail</h4>

    ./vendor/bin/sail up


<h4>copia archivo .env</h4>


    cp .env.example .env
    
    
<h4>crea llave de la aplicación</h4>

    ./vendor/bin/sail artisan key:generate
   
    
    
<h4>Ejecuta los siguientes comandos</h4>


    ./vendor/bin/sail npm install
   
    ./vendor/bin/sail npm run dev
    

<h4>Edita archivo hot de carpeta public:</h4>

    
    de'http://0.0.0.0:5173' a 'http://localhost:5173'


<h4>Finalmente <a href="http://localhost" >Abre localhost</a></h4>



<p align="center">
<a href="https://github.com/laravel/framework/actions"><img src="https://github.com/laravel/framework/workflows/tests/badge.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
</p>

## About Laravel

Laravel is a web application framework with expressive, elegant syntax. We believe development must be an enjoyable and creative experience to be truly fulfilling. Laravel takes the pain out of development by easing common tasks used in many web projects, such as:

- [Simple, fast routing engine](https://laravel.com/docs/routing).
- [Powerful dependency injection container](https://laravel.com/docs/container).
- Multiple back-ends for [session](https://laravel.com/docs/session) and [cache](https://laravel.com/docs/cache) storage.
- Expressive, intuitive [database ORM](https://laravel.com/docs/eloquent).
- Database agnostic [schema migrations](https://laravel.com/docs/migrations).
- [Robust background job processing](https://laravel.com/docs/queues).
- [Real-time event broadcasting](https://laravel.com/docs/broadcasting).

Laravel is accessible, powerful, and provides tools required for large, robust applications.

## Learning Laravel

Laravel has the most extensive and thorough [documentation](https://laravel.com/docs) and video tutorial library of all modern web application frameworks, making it a breeze to get started with the framework.

You may also try the [Laravel Bootcamp](https://bootcamp.laravel.com), where you will be guided through building a modern Laravel application from scratch.

If you don't feel like reading, [Laracasts](https://laracasts.com) can help. Laracasts contains over 2000 video tutorials on a range of topics including Laravel, modern PHP, unit testing, and JavaScript. Boost your skills by digging into our comprehensive video library.

## Laravel Sponsors

We would like to extend our thanks to the following sponsors for funding Laravel development. If you are interested in becoming a sponsor, please visit the Laravel [Patreon page](https://patreon.com/taylorotwell).

### Premium Partners

- **[Vehikl](https://vehikl.com/)**
- **[Tighten Co.](https://tighten.co)**
- **[Kirschbaum Development Group](https://kirschbaumdevelopment.com)**
- **[64 Robots](https://64robots.com)**
- **[Cubet Techno Labs](https://cubettech.com)**
- **[Cyber-Duck](https://cyber-duck.co.uk)**
- **[Many](https://www.many.co.uk)**
- **[Webdock, Fast VPS Hosting](https://www.webdock.io/en)**
- **[DevSquad](https://devsquad.com)**
- **[Curotec](https://www.curotec.com/services/technologies/laravel/)**
- **[OP.GG](https://op.gg)**
- **[WebReinvent](https://webreinvent.com/?utm_source=laravel&utm_medium=github&utm_campaign=patreon-sponsors)**
- **[Lendio](https://lendio.com)**

## Contributing

Thank you for considering contributing to the Laravel framework! The contribution guide can be found in the [Laravel documentation](https://laravel.com/docs/contributions).

## Code of Conduct

In order to ensure that the Laravel community is welcoming to all, please review and abide by the [Code of Conduct](https://laravel.com/docs/contributions#code-of-conduct).

## Security Vulnerabilities

If you discover a security vulnerability within Laravel, please send an e-mail to Taylor Otwell via [taylor@laravel.com](mailto:taylor@laravel.com). All security vulnerabilities will be promptly addressed.

## License

The Laravel framework is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).
