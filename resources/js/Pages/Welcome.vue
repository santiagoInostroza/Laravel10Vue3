<script setup>
import { Head, Link } from '@inertiajs/vue3';

defineProps({
    canLogin: Boolean,
    canRegister: Boolean,
    laravelVersion: String,
    phpVersion: String,
});
</script>

<template>
    <Head title="Bienvenido" />
    <div class="p-8 md:p-16 lg:p-24 text-gray-400 bg-gradient-to-r via-gray-200 from-indigo-300 to-indigo-200">
        <h1 class="text-5xl text-gray-700 font-bold text-gray-500 text-center my-8">
            Hola Bienvenido
        </h1>
        <div class="my-16 text-2xl md:text-3xl text-gray-700">
            Este proyecto está pensado como una base para que puedas comenzar rapidamente a crear tu propio proyecto.
        </div>
        <div class="my-16 text-2xl md:text-3xl text-gray-700">
            Tiene instalada las siguientes librerias:
        </div>
        <ul class="grid grid-cols-1 md:grid-cols-2 gap-6 lg:gap-8">
            <!-- Laravel 10 -->
            <li class="border rounded p-4 shadow bg-white">
                <h2 class="mb-4 text-3xl md:text-2xl text-gray-600 font-bold">
                    <a href="https://laravel.com/docs/10.x/sail" target="_blank" rel="noopener noreferrer">
                        <div class="flex gap-8">
                            <svg xmlns="http://www.w3.org/2000/svg" width="50" height="52" viewBox="0 0 50 52"><title>Logomark</title><path d="M49.626 11.564a.809.809 0 0 1 .028.209v10.972a.8.8 0 0 1-.402.694l-9.209 5.302V39.25c0 .286-.152.55-.4.694L20.42 51.01c-.044.025-.092.041-.14.058-.018.006-.035.017-.054.022a.805.805 0 0 1-.41 0c-.022-.006-.042-.018-.063-.026-.044-.016-.09-.03-.132-.054L.402 39.944A.801.801 0 0 1 0 39.25V6.334c0-.072.01-.142.028-.21.006-.023.02-.044.028-.067.015-.042.029-.085.051-.124.015-.026.037-.047.055-.071.023-.032.044-.065.071-.093.023-.023.053-.04.079-.06.029-.024.055-.05.088-.069h.001l9.61-5.533a.802.802 0 0 1 .8 0l9.61 5.533h.002c.032.02.059.045.088.068.026.02.055.038.078.06.028.029.048.062.072.094.017.024.04.045.054.071.023.04.036.082.052.124.008.023.022.044.028.068a.809.809 0 0 1 .028.209v20.559l8.008-4.611v-10.51c0-.07.01-.141.028-.208.007-.024.02-.045.028-.068.016-.042.03-.085.052-.124.015-.026.037-.047.054-.071.024-.032.044-.065.072-.093.023-.023.052-.04.078-.06.03-.024.056-.05.088-.069h.001l9.611-5.533a.801.801 0 0 1 .8 0l9.61 5.533c.034.02.06.045.09.068.025.02.054.038.077.06.028.029.048.062.072.094.018.024.04.045.054.071.023.039.036.082.052.124.009.023.022.044.028.068zm-1.574 10.718v-9.124l-3.363 1.936-4.646 2.675v9.124l8.01-4.611zm-9.61 16.505v-9.13l-4.57 2.61-13.05 7.448v9.216l17.62-10.144zM1.602 7.719v31.068L19.22 48.93v-9.214l-9.204-5.209-.003-.002-.004-.002c-.031-.018-.057-.044-.086-.066-.025-.02-.054-.036-.076-.058l-.002-.003c-.026-.025-.044-.056-.066-.084-.02-.027-.044-.05-.06-.078l-.001-.003c-.018-.03-.029-.066-.042-.1-.013-.03-.03-.058-.038-.09v-.001c-.01-.038-.012-.078-.016-.117-.004-.03-.012-.06-.012-.09v-.002-21.481L4.965 9.654 1.602 7.72zm8.81-5.994L2.405 6.334l8.005 4.609 8.006-4.61-8.006-4.608zm4.164 28.764l4.645-2.674V7.719l-3.363 1.936-4.646 2.675v20.096l3.364-1.937zM39.243 7.164l-8.006 4.609 8.006 4.609 8.005-4.61-8.005-4.608zm-.801 10.605l-4.646-2.675-3.363-1.936v9.124l4.645 2.674 3.364 1.937v-9.124zM20.02 38.33l11.743-6.704 5.87-3.35-8-4.606-9.211 5.303-8.395 4.833 7.993 4.524z" fill="#FF2D20" fill-rule="evenodd"/></svg>
                            Laravel 10
                        </div>
                    </a>
                </h2>
                <p>
                    Laravel es un marco de aplicación web con una sintaxis elegante y expresiva. Ya hemos sentado las bases: liberándote para crear sin preocuparte por las cosas pequeñas.
                </p>
            </li>
            <!-- Vue 3 -->
            <li class="border rounded p-4 shadow bg-white">
                <h2 class="mb-4 text-xl md:text-2xl flex gap-4">
                    <svg class="logo" viewBox="0 0 128 128" width="24" height="24" data-v-608f1a0f=""><path fill="#42b883" d="M78.8,10L64,35.4L49.2,10H0l64,110l64-110C128,10,78.8,10,78.8,10z" data-v-608f1a0f=""></path><path fill="#35495e" d="M78.8,10L64,35.4L49.2,10H25.6L64,76l38.4-66H78.8z" data-v-608f1a0f=""></path></svg>
                    <a href="https://v3.vuejs.org" target="_blank" rel="noopener noreferrer">Vue 3</a>
                </h2>
                <p>
                    Un marco accesible, eficaz y versátil para crear interfaces de usuario web.
                </p>
            </li>
            <!-- sail -->
            <li class="border rounded p-4 shadow bg-white">
                <h2 class="mb-4 text-3xl md:text-2xl text-gray-600 font-bold">
                    <a href="https://laravel.com/docs/10.x/sail" target="_blank" rel="noopener noreferrer">Laravel Sail</a>
                </h2>
                <p>
                    Laravel Sail es una interfaz de línea de comandos liviana para interactuar con el entorno de desarrollo Docker predeterminado de Laravel. Sail proporciona un excelente punto de partida para crear una aplicación Laravel utilizando PHP, MySQL y Redis sin necesidad de experiencia previa en Docker.
                </p>
                <h3 class="my-8">Ejemplos</h3>
                <p>
                    sail up : comando para levantar el servidor
                </p>
            </li>
            <!-- Jetstream -->
            <li class="border rounded p-4 shadow bg-white">
                <h2 class="mb-4 text-xl md:text-2xl">
                    <a href="https://jetstream.laravel.com" target="_blank" rel="noopener noreferrer">
                        <svg xmlns="http://www.w3.org/2000/svg" width="317" height="48" fill="none">
                            <path d="M74.09 30.04V13h-4.14v21H82.1v-3.96h-8.01zM95.379 19v1.77c-1.08-1.35-2.7-2.19-4.89-2.19-3.99 0-7.29 3.45-7.29 7.92s3.3 7.92 7.29 7.92c2.19 0 3.81-.84 4.89-2.19V34h3.87V19h-3.87zm-4.17 11.73c-2.37 0-4.14-1.71-4.14-4.23 0-2.52 1.77-4.23 4.14-4.23 2.4 0 4.17 1.71 4.17 4.23 0 2.52-1.77 4.23-4.17 4.23zM106.628 21.58V19h-3.87v15h3.87v-7.17c0-3.15 2.55-4.05 4.56-3.81V18.7c-1.89 0-3.78.84-4.56 2.88zM124.295 19v1.77c-1.08-1.35-2.7-2.19-4.89-2.19-3.99 0-7.29 3.45-7.29 7.92s3.3 7.92 7.29 7.92c2.19 0 3.81-.84 4.89-2.19V34h3.87V19h-3.87zm-4.17 11.73c-2.37 0-4.14-1.71-4.14-4.23 0-2.52 1.77-4.23 4.14-4.23 2.4 0 4.17 1.71 4.17 4.23 0 2.52-1.77 4.23-4.17 4.23zM141.544 19l-3.66 10.5-3.63-10.5h-4.26l5.7 15h4.41l5.7-15h-4.26zM150.354 28.09h11.31c.09-.51.15-1.02.15-1.59 0-4.41-3.15-7.92-7.59-7.92-4.71 0-7.92 3.45-7.92 7.92s3.18 7.92 8.22 7.92c2.88 0 5.13-1.17 6.54-3.21l-3.12-1.8c-.66.87-1.86 1.5-3.36 1.5-2.04 0-3.69-.84-4.23-2.82zm-.06-3c.45-1.92 1.86-3.03 3.93-3.03 1.62 0 3.24.87 3.72 3.03h-7.65zM164.516 34h3.87V12.1h-3.87V34zM185.248 34.36c3.69 0 6.9-2.01 6.9-6.3V13h-2.1v15.06c0 3.03-2.07 4.26-4.8 4.26-2.19 0-3.93-.78-4.62-2.61l-1.77 1.05c1.05 2.43 3.57 3.6 6.39 3.6zM203.124 18.64c-4.65 0-7.83 3.45-7.83 7.86 0 4.53 3.24 7.86 7.98 7.86 3.03 0 5.34-1.41 6.6-3.45l-1.74-1.02c-.81 1.44-2.46 2.55-4.83 2.55-3.18 0-5.55-1.89-5.97-4.95h13.17c.03-.3.06-.63.06-.93 0-4.11-2.85-7.92-7.44-7.92zm0 1.92c2.58 0 4.98 1.71 5.4 5.01h-11.19c.39-2.94 2.64-5.01 5.79-5.01zM221.224 20.92V19h-4.32v-4.2l-1.98.6V19h-3.15v1.92h3.15v9.09c0 3.6 2.25 4.59 6.3 3.99v-1.74c-2.91.12-4.32.33-4.32-2.25v-9.09h4.32zM225.176 22.93c0-1.62 1.59-2.37 3.15-2.37 1.44 0 2.97.57 3.6 2.1l1.65-.96c-.87-1.86-2.79-3.06-5.25-3.06-3 0-5.13 1.89-5.13 4.29 0 5.52 8.76 3.39 8.76 7.11 0 1.77-1.68 2.4-3.45 2.4-2.01 0-3.57-.99-4.11-2.52l-1.68.99c.75 1.92 2.79 3.45 5.79 3.45 3.21 0 5.43-1.77 5.43-4.32 0-5.52-8.76-3.39-8.76-7.11zM244.603 20.92V19h-4.32v-4.2l-1.98.6V19h-3.15v1.92h3.15v9.09c0 3.6 2.25 4.59 6.3 3.99v-1.74c-2.91.12-4.32.33-4.32-2.25v-9.09h4.32zM249.883 21.49V19h-1.98v15h1.98v-8.34c0-3.72 2.34-4.98 4.74-4.98v-1.92c-1.92 0-3.69.63-4.74 2.73zM263.358 18.64c-4.65 0-7.83 3.45-7.83 7.86 0 4.53 3.24 7.86 7.98 7.86 3.03 0 5.34-1.41 6.6-3.45l-1.74-1.02c-.81 1.44-2.46 2.55-4.83 2.55-3.18 0-5.55-1.89-5.97-4.95h13.17c.03-.3.06-.63.06-.93 0-4.11-2.85-7.92-7.44-7.92zm0 1.92c2.58 0 4.98 1.71 5.4 5.01h-11.19c.39-2.94 2.64-5.01 5.79-5.01zM286.848 19v2.94c-1.26-2.01-3.39-3.3-6.06-3.3-4.23 0-7.74 3.42-7.74 7.86s3.51 7.86 7.74 7.86c2.67 0 4.8-1.29 6.06-3.3V34h1.98V19h-1.98zm-5.91 13.44c-3.33 0-5.91-2.61-5.91-5.94 0-3.33 2.58-5.94 5.91-5.94s5.91 2.61 5.91 5.94c0 3.33-2.58 5.94-5.91 5.94zM309.01 18.64c-1.92 0-3.75.87-4.86 2.73-.84-1.74-2.46-2.73-4.56-2.73-1.8 0-3.42.72-4.59 2.55V19h-1.98v15H295v-8.31c0-3.72 2.16-5.13 4.32-5.13 2.13 0 3.51 1.41 3.51 4.08V34h1.98v-8.31c0-3.72 1.86-5.13 4.17-5.13 2.13 0 3.66 1.41 3.66 4.08V34h1.98v-9.36c0-3.75-2.31-6-5.61-6z" fill="#000"/>
                            <path d="M11.395 44.428C4.557 40.198 0 32.632 0 24 0 10.745 10.745 0 24 0a23.891 23.891 0 0113.997 4.502c-.2 17.907-11.097 33.245-26.602 39.926z" fill="#6875F5"/>
                            <path d="M14.134 45.885A23.914 23.914 0 0024 48c13.255 0 24-10.745 24-24 0-3.516-.756-6.856-2.115-9.866-4.659 15.143-16.608 27.092-31.75 31.751z" fill="#6875F5"/>
                        </svg>
                    </a>
                </h2>
                <p>
                    Laravel Jetstream es un kit de inicio de aplicaciones bellamente diseñado para Laravel y proporciona el punto de partida perfecto para su próxima aplicación Laravel. Jetstream proporciona la implementación para el inicio de sesión, el registro, la verificación de correo electrónico, la autenticación de dos factores, la administración de sesiones, la API a través de Laravel Sanctum y funciones opcionales de administración de equipos de su aplicación.
                </p>
                <h3 class="my-8">Ejemplos:</h3>
                <p>
                    <div v-if="canLogin">
                        <Link v-if="$page.props.auth.user" :href="route('dashboard')" class="font-semibold hover:text-gray-900 dark:text-gray-400 dark:hover:text-white focus:outline focus:outline-2 focus:rounded-sm focus:outline-red-500">Dashboard</Link>

                        <template v-else>
                            <div class="my-8">
                                <Link :href="route('login')" class="font-semibold  hover:text-gray-900 dark:text-gray-400 dark:hover:text-white focus:outline focus:outline-2 focus:rounded-sm focus:outline-red-500">Ingresar</Link>
                                
                                <Link v-if="canRegister" :href="route('register')" class="ml-4 font-semibold  hover:text-gray-900 dark:text-gray-400 dark:hover:text-white focus:outline focus:outline-2 focus:rounded-sm focus:outline-red-500">Registrarse</Link>
                            </div>
                        </template>
                    </div>
                </p>
            </li>
            <!-- Inertia -->
            <li class="border rounded p-4 shadow bg-white">
                <h2 class="mb-4 text-xl md:text-2xl flex gap-4">
                    <a href="https://inertiajs.com" target="_blank" rel="noopener noreferrer">
                        <svg class="block fill-current text-purple-600" viewBox="0 0 275.3 50.5" style="height: 25px;"><path d="M231.2 16.1h-17.8l17.2 17.2-17.2 17.2h17.8l17.2-17.2z"></path><path d="M258.1 16.1h-17.8l17.2 17.2-17.2 17.2h17.8l17.2-17.2z"></path><path d="M6 15.3h10.3l-6 34.2H0l6-34.2zm.6-9.1C7.2 2.9 10.3 0 13.7 0s5.7 2.8 5.2 6.2c-.5 3.4-3.7 6.2-7.2 6.2s-5.6-3-5.1-6.2zM54.3 28.5l-3.7 21H40.4L43.8 30c.8-4.4-1.6-6.2-4.9-6.2-3.4 0-6.5 2-7.5 6.6L28 49.5H17.8l6-34.2h10.3l-.5 3.2c2.3-2.6 6.2-4.2 10.1-4.2 6.9.1 12.2 5.1 10.6 14.2zM94.5 32.4c-.1.8-.5 2.7-1.1 4.1H68.9c.6 3.8 3.8 4.8 7 4.8 2.9 0 5.2-.8 7.2-2.7l7.2 5.9c-4 4-8.7 6-15 6-11.8 0-18-8.5-16.3-18.7a20.7 20.7 0 0 1 20.5-17.4c9.8 0 16.9 7.6 15 18zm-9.7-3.7c-.3-3.8-3-5.3-6.2-5.3a8.9 8.9 0 0 0-8.3 5.3h14.5zM123.9 14.6l-2 11.6c-4-.6-10.5.8-11.7 7.8l.1-.4-2.8 15.9H97.3l6-34.2h10.3l-1.1 6.2c2.1-4.7 6.6-6.9 11.4-6.9zM137.8 37.3c-.5 3.1 2 3.3 6.6 2.9l-1.6 9.3c-12.3 1.4-16.9-2.7-15.2-12.2l2.1-12.1h-5.5l1.8-9.9h5.4l1.2-6.5 10.8-3.1-1.7 9.6h7.1l-1.8 9.9h-7l-2.2 12.1zM155.3 15.3h10.3l-6 34.2h-10.3l6-34.2zm.6-9.1c.5-3.3 3.7-6.2 7.1-6.2s5.7 2.8 5.2 6.2c-.5 3.4-3.7 6.2-7.2 6.2s-5.7-3-5.1-6.2zM208.1 15.3l-6 34.2h-10.3l.4-2.3a15.5 15.5 0 0 1-10.3 3.3c-11.1 0-15.3-9.6-13.5-18.9 1.6-8.8 8.6-17.2 19.2-17.2 4.5 0 7.7 1.8 9.6 4.6l.6-3.6h10.3zm-13.2 17.2c.9-5.2-1.9-8.4-6.6-8.4a9.5 9.5 0 0 0-9.5 8.3c-.9 5.1 1.8 8.3 6.6 8.3 4.6.1 8.6-3.1 9.5-8.2z"></path></svg>
                    </a>
                </h2>
                <p>
                    Inertia es un nuevo enfoque para crear aplicaciones web clásicas basadas en servidor. Lo llamamos el monolito moderno.

                    Inertia le permite crear aplicaciones de una sola página renderizadas completamente en el lado del cliente, sin la complejidad que viene con los SPA modernos. Para ello, aprovecha los patrones existentes del lado del servidor que ya te encantan.

                    Inertia no tiene enrutamiento del lado del cliente ni requiere una API. ¡Simplemente cree controladores y vistas de páginas como siempre lo ha hecho! Inertia funciona muy bien con cualquier marco de backend, pero está optimizado para Laravel .
                </p>
            </li>
            <!-- Tailwind Css -->
            <li class="border rounded p-4 shadow bg-white">
                <h2 class="mb-4 text-xl md:text-2xl flex gap-4">
                    <a href="https://tailwindcss.com" target="_blank" rel="noopener noreferrer">
                        <svg viewBox="0 0 248 31" class="text-slate-900 dark:text-white w-auto h-5"><path fill-rule="evenodd" clip-rule="evenodd" d="M25.517 0C18.712 0 14.46 3.382 12.758 10.146c2.552-3.382 5.529-4.65 8.931-3.805 1.941.482 3.329 1.882 4.864 3.432 2.502 2.524 5.398 5.445 11.722 5.445 6.804 0 11.057-3.382 12.758-10.145-2.551 3.382-5.528 4.65-8.93 3.804-1.942-.482-3.33-1.882-4.865-3.431C34.736 2.92 31.841 0 25.517 0zM12.758 15.218C5.954 15.218 1.701 18.6 0 25.364c2.552-3.382 5.529-4.65 8.93-3.805 1.942.482 3.33 1.882 4.865 3.432 2.502 2.524 5.397 5.445 11.722 5.445 6.804 0 11.057-3.381 12.758-10.145-2.552 3.382-5.529 4.65-8.931 3.805-1.941-.483-3.329-1.883-4.864-3.432-2.502-2.524-5.398-5.446-11.722-5.446z" fill="#38bdf8"></path><path fill-rule="evenodd" clip-rule="evenodd" d="M76.546 12.825h-4.453v8.567c0 2.285 1.508 2.249 4.453 2.106v3.463c-5.962.714-8.332-.928-8.332-5.569v-8.567H64.91V9.112h3.304V4.318l3.879-1.143v5.937h4.453v3.713zM93.52 9.112h3.878v17.849h-3.878v-2.57c-1.365 1.891-3.484 3.034-6.285 3.034-4.884 0-8.942-4.105-8.942-9.389 0-5.318 4.058-9.388 8.942-9.388 2.801 0 4.92 1.142 6.285 2.999V9.112zm-5.674 14.636c3.232 0 5.674-2.392 5.674-5.712s-2.442-5.711-5.674-5.711-5.674 2.392-5.674 5.711c0 3.32 2.442 5.712 5.674 5.712zm16.016-17.313c-1.364 0-2.477-1.142-2.477-2.463a2.475 2.475 0 012.477-2.463 2.475 2.475 0 012.478 2.463c0 1.32-1.113 2.463-2.478 2.463zm-1.939 20.526V9.112h3.879v17.849h-3.879zm8.368 0V.9h3.878v26.06h-3.878zm29.053-17.849h4.094l-5.638 17.849h-3.807l-3.735-12.03-3.771 12.03h-3.806l-5.639-17.849h4.094l3.484 12.315 3.771-12.315h3.699l3.734 12.315 3.52-12.315zm8.906-2.677c-1.365 0-2.478-1.142-2.478-2.463a2.475 2.475 0 012.478-2.463 2.475 2.475 0 012.478 2.463c0 1.32-1.113 2.463-2.478 2.463zm-1.939 20.526V9.112h3.878v17.849h-3.878zm17.812-18.313c4.022 0 6.895 2.713 6.895 7.354V26.96h-3.878V16.394c0-2.713-1.58-4.14-4.022-4.14-2.55 0-4.561 1.499-4.561 5.14v9.567h-3.879V9.112h3.879v2.285c1.185-1.856 3.124-2.749 5.566-2.749zm25.282-6.675h3.879V26.96h-3.879v-2.57c-1.364 1.892-3.483 3.034-6.284 3.034-4.884 0-8.942-4.105-8.942-9.389 0-5.318 4.058-9.388 8.942-9.388 2.801 0 4.92 1.142 6.284 2.999V1.973zm-5.674 21.775c3.232 0 5.674-2.392 5.674-5.712s-2.442-5.711-5.674-5.711-5.674 2.392-5.674 5.711c0 3.32 2.442 5.712 5.674 5.712zm22.553 3.677c-5.423 0-9.481-4.105-9.481-9.389 0-5.318 4.058-9.388 9.481-9.388 3.519 0 6.572 1.82 8.008 4.605l-3.34 1.928c-.79-1.678-2.549-2.749-4.704-2.749-3.16 0-5.566 2.392-5.566 5.604 0 3.213 2.406 5.605 5.566 5.605 2.155 0 3.914-1.107 4.776-2.749l3.34 1.892c-1.508 2.82-4.561 4.64-8.08 4.64zm14.472-13.387c0 3.249 9.661 1.285 9.661 7.89 0 3.57-3.125 5.497-7.003 5.497-3.591 0-6.177-1.607-7.326-4.177l3.34-1.927c.574 1.606 2.011 2.57 3.986 2.57 1.724 0 3.052-.571 3.052-2 0-3.176-9.66-1.391-9.66-7.781 0-3.356 2.909-5.462 6.572-5.462 2.945 0 5.387 1.357 6.644 3.713l-3.268 1.82c-.647-1.392-1.904-2.035-3.376-2.035-1.401 0-2.622.607-2.622 1.892zm16.556 0c0 3.249 9.66 1.285 9.66 7.89 0 3.57-3.124 5.497-7.003 5.497-3.591 0-6.176-1.607-7.326-4.177l3.34-1.927c.575 1.606 2.011 2.57 3.986 2.57 1.724 0 3.053-.571 3.053-2 0-3.176-9.66-1.391-9.66-7.781 0-3.356 2.908-5.462 6.572-5.462 2.944 0 5.386 1.357 6.643 3.713l-3.268 1.82c-.646-1.392-1.903-2.035-3.375-2.035-1.401 0-2.622.607-2.622 1.892z" fill="currentColor"></path></svg>
                    </a>
                </h2>
                <p>
                    Un marco CSS de utilidad repleto de clases como , y que se pueden componer para crear cualquier diseño, directamente en su marcado .
                </p>
                <h3 class="my-8">Ejemplos:</h3>
                <p>-Toda esta pantalla está realizada con diseños de Tailwind</p>
                <p class="animate-pulse my-4">-Este ejemplo tiene la clase: animate-pulse</p>
            </li>
            <!-- Vite -->
            <li class="border rounded p-4 shadow bg-white">
                <h2 class="mb-4 text-xl md:text-2xl flex gap-4 items-center">
                    <svg xmlns="http://www.w3.org/2000/svg" width="40" height="30" viewBox="0 0 410 404" fill="none">
                        <path d="M399.641 59.5246L215.643 388.545C211.844 395.338 202.084 395.378 198.228 388.618L10.5817 59.5563C6.38087 52.1896 12.6802 43.2665 21.0281 44.7586L205.223 77.6824C206.398 77.8924 207.601 77.8904 208.776 77.6763L389.119 44.8058C397.439 43.2894 403.768 52.1434 399.641 59.5246Z" fill="url(#paint0_linear)"/>
                        <path d="M292.965 1.5744L156.801 28.2552C154.563 28.6937 152.906 30.5903 152.771 32.8664L144.395 174.33C144.198 177.662 147.258 180.248 150.51 179.498L188.42 170.749C191.967 169.931 195.172 173.055 194.443 176.622L183.18 231.775C182.422 235.487 185.907 238.661 189.532 237.56L212.947 230.446C216.577 229.344 220.065 232.527 219.297 236.242L201.398 322.875C200.278 328.294 207.486 331.249 210.492 326.603L212.5 323.5L323.454 102.072C325.312 98.3645 322.108 94.137 318.036 94.9228L279.014 102.454C275.347 103.161 272.227 99.746 273.262 96.1583L298.731 7.86689C299.767 4.27314 296.636 0.855181 292.965 1.5744Z" fill="url(#paint1_linear)"/>
                        <defs>
                        <linearGradient id="paint0_linear" x1="6.00017" y1="32.9999" x2="235" y2="344" gradientUnits="userSpaceOnUse">
                        <stop stop-color="#41D1FF"/>
                        <stop offset="1" stop-color="#BD34FE"/>
                        </linearGradient>
                        <linearGradient id="paint1_linear" x1="194.651" y1="8.81818" x2="236.076" y2="292.989" gradientUnits="userSpaceOnUse">
                        <stop stop-color="#FFEA83"/>
                        <stop offset="0.0833333" stop-color="#FFDD35"/>
                        <stop offset="1" stop-color="#FFA800"/>
                        </linearGradient>
                        </defs>
                    </svg>
                    <a href="https://vitejs.dev/" target="_blank" rel="noopener noreferrer">
                        Vite
                    </a>
                </h2>
                <p>
                    Prepárese para un entorno de desarrollo que finalmente podrá alcanzarlo.
                </p>
                <h3 class="my-8">Ejemplos:</h3>
                <p>-Inicio instantáneo del servidor</p>
                <p>-HMR ultrarrápido</p>
                <p>-Funciones ricas</p>
                <p>-Construcción optimizada</p>
                <p>-Complementos universales</p>
                <p>-API completamente tipificadas</p>
            </li>
            <!-- Element Plus -->
            <li class="border rounded p-4 shadow bg-white">
                <h2 class="mb-4 text-xl md:text-2xl flex gap-4 items-center">
                    <a href="https://element-plus.org/es-ES/" target="_blank">
                        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 153.71 38"  width="100" height="30" >
                            <g id="图层_2" data-name="图层 2">
                                <g id="图层_1-2" data-name="图层 1">
                                    <path id="Shape-Copy" class="cls-1" d="M142,26.16s.28,0,.82,0a.72.72,0,0,1,.69.41s1.08,2,1.37,2.48,0,.42-.12.41h0s-.31,0-3.45,0a4.93,4.93,0,0,1-4.54-4.54v-7H134.3V15.28c0-.36.41-.41.41-.41h2.07V12.25a.6.6,0,0,1,.41-.55l2.3-.66c.34-.1.59,0,.59.35V15h3.58c.34,0,.41.41.41.41V18h-4v6.06c0,1.76,1.93,2.07,1.93,2.07Zm-10.6,3h-2.2c-.43,0-.41-.55-.41-.55V18.45c0-.62-.83-.83-.83-.83h-4.54c-.68,0-.69.83-.69.83V28.77a.41.41,0,0,1-.41.42h-2.2c-.48,0-.41-.55-.41-.55V15.83c0-1,1.24-1.24,1.24-1.24h9.63c1,0,1.23,1.24,1.23,1.24V28.5c0,.72-.41.69-.41.69ZM115.73,23.4H107.2v2.07c0,.74,1,1,1,1H115a1.16,1.16,0,0,1,.82.42s.61,1.25.83,1.79-.41.55-.41.55H106c-1.24,0-1.51-1.52-1.51-1.52V16c0-.67,1-1,1-1h10.32c1,0,1.24,1.23,1.24,1.23v5.93c0,1-1.24,1.23-1.24,1.23Zm-1.52-4.95s-.08-.69-.68-.69h-5.65s-.68.18-.68.69V20a.69.69,0,0,0,.68.69h5.65a.9.9,0,0,0,.68-.83V18.45ZM101.28,29.19h-2.2c-.29,0-.41-.42-.41-.42V18.45c0-.64-.83-.83-.83-.83H95.78c-.58,0-.69.83-.69.83V28.77c0,.35-.41.42-.41.42h-2.2c-.31,0-.42-.42-.42-.42V18.45c0-.66-.82-.83-.82-.83H89.17c-.63,0-.68.83-.68.83V28.77a.39.39,0,0,1-.42.42h-2.2a.41.41,0,0,1-.41-.42V15.69c0-.75,1.1-1.1,1.1-1.1h13.76c1.1,0,1.37,1.38,1.37,1.38v12.8c0,.48-.41.42-.41.42Zm-20-5.79H72.8v2.07c0,.74,1,1,1,1h6.88a1.19,1.19,0,0,1,.83.42s.6,1.25.82,1.79-.41.55-.41.55H71.56c-1.24,0-1.51-1.52-1.51-1.52V16c0-.67,1-1,1-1H81.33c1,0,1.24,1.23,1.24,1.23v5.93c0,1-1.24,1.23-1.24,1.23Zm-1.51-4.95s-.09-.69-.69-.69H73.49s-.69.18-.69.69V20a.69.69,0,0,0,.69.69h5.64a.91.91,0,0,0,.69-.83V18.45ZM68,29.19H62.76a4.35,4.35,0,0,1-4.13-4c0-3.91,0-16.1,0-16.1h2.48a.79.79,0,0,1,.82.82V24.37A2.58,2.58,0,0,0,63.86,26h2.2s.72-.23,1.24.69l1.1,1.93s.08.55-.41.55Zm-26.56-.83V10.19a1,1,0,0,1,.69-1H55.05c.73,0,.42.83.42.83s-.41,1.12-.69,1.65a1,1,0,0,1-.83.55H45.56a.77.77,0,0,0-.83.69v4.54h9.5c.55,0,.27.69.27.69s-.71,1.52-1,1.93a1.05,1.05,0,0,1-.83.41h-8v4.82a.91.91,0,0,0,.69.83h8.81a.85.85,0,0,1,.82.41l1.24,1.93c.37.56-.14.69-.14.69H42.26C41.68,29.19,41.43,28.36,41.43,28.36Zm-8.14-1.14c0,1.57-.83,1.93-.83,1.93S18.32,37.31,17.4,37.83a1.68,1.68,0,0,1-1.52,0S1.09,29.25.55,28.87a1.29,1.29,0,0,1-.55-1s0-17,0-17.78S1,8.76,1,8.76L15.75.21a2,2,0,0,1,1.79,0S30.6,7.8,32,8.62a2.08,2.08,0,0,1,1.25,2.06s0,15.07,0,16.54Zm-5.9-17c-3-1.74-10.16-5.87-10.16-5.87a1.58,1.58,0,0,0-1.41,0L4.22,11s-.77.46-.76,1.08S3.46,26,3.46,26a1,1,0,0,0,.43.75c.43.3,12,7,12,7a1.3,1.3,0,0,0,1.19,0c.72-.4,11.82-6.79,11.82-6.79s.65-.28.65-1.51c0-.36,0-1.74,0-3.47L16.53,29.88v-3a3,3,0,0,1,1-2.07l11.56-7a2.49,2.49,0,0,0,.55-1.46c0-1.27,0-2.37,0-3.07L16.53,21.2V18a2.17,2.17,0,0,1,.83-1.79Z"/>
                                    <path class="cls-1" d="M150.32,11.21h-2.24v-5c0-.11.12-.21.29-.24l1.44-.26c.26,0,.51.07.51.24Z"/>
                                    <path class="cls-1" d="M148.08,9h2.24v5.11c0,.11-.11.21-.28.25l-1.45.26c-.26.05-.51-.07-.51-.24Z"/>
                                    <path class="cls-2" d="M145.09,9h8.22a.4.4,0,0,1,.4.4v1.85a0,0,0,0,1,0,0h-9a0,0,0,0,1,0,0V9.36A.4.4,0,0,1,145.09,9Z"/>
                                </g>
                            </g>
                        </svg>
                    </a>
                </h2>
                <p>
                    una biblioteca de componentes basada en Vue 3 para diseñadores y desarrolladores
                </p>
                <h3 class="my-8">Ejemplos:</h3>
                <p class="grid gap-4 grid-cols-2">
                    <el-button>Default</el-button>
                    <el-button type="primary">Primary</el-button>
                    <el-button type="success">Success</el-button>
                    <el-button type="info">Info</el-button>
                    <el-button type="warning">Warning</el-button>
                    <el-button type="danger">Danger</el-button>
                </p>
            </li>
        </ul>
    </div>
</template>

<style>
.bg-dots-darker {
    background-image: url("data:image/svg+xml,%3Csvg width='30' height='30' viewBox='0 0 30 30' fill='none' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M1.22676 0C1.91374 0 2.45351 0.539773 2.45351 1.22676C2.45351 1.91374 1.91374 2.45351 1.22676 2.45351C0.539773 2.45351 0 1.91374 0 1.22676C0 0.539773 0.539773 0 1.22676 0Z' fill='rgba(0,0,0,0.07)'/%3E%3C/svg%3E");
}
@media (prefers-color-scheme: dark) {
    .dark\:bg-dots-lighter {
        background-image: url("data:image/svg+xml,%3Csvg width='30' height='30' viewBox='0 0 30 30' fill='none' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M1.22676 0C1.91374 0 2.45351 0.539773 2.45351 1.22676C2.45351 1.91374 1.91374 2.45351 1.22676 2.45351C0.539773 2.45351 0 1.91374 0 1.22676C0 0.539773 0.539773 0 1.22676 0Z' fill='rgba(255,255,255,0.07)'/%3E%3C/svg%3E");
    }
}
</style>
