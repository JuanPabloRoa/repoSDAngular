Instalación
=================

Trabajo llevado a cabo en Ubuntu 16.04LTS para ramo de Sistemas Disribuidos. 
Puerto utilizado AngularJS: 9000
Puerto utilizado PHP: 3306, 6379, 2525

Requerimientos
--------------

* Node JS y NPM [descarga](https://nodejs.org/en/download/) o por [gestor de paquetes](https://nodejs.org/en/download/package-manager/)
* Gulp `$ npm install --global gulp`
* Lampp 
* PHP, apache `$ sudo apt-get install -y apache2`, `$ sudo apt-get install -y php7.0 libapache2-mod-php7.0 php7.0-cli php7.0-common php7.0-mbstring php7.0-intl php7.0-xml php7.0-mysql php7.0-mcrypt php7.0-zip` (referencia: https://cerebro-digital.com/panel/knowledgebase/57/Como-instalar-y-configurar-PHP-70-o-PHP-71-en-Linux-Ubuntu-1604.html)



Instalación
-----------
Iniciar Lampp (/opt/lampp/lampp start)

`PHP`
Una vez descomprimida la carpeta:
* ir a mysql ( con lampp acceder a http://localhost/phpmyadmin/) y crear una base de datos llamada sd.
* crear un usuario llamado img2030 y contraseña img2030.
* crear las tablas en la db abriendo una consola en la carpeta del proyecto y usando: `$ php artisan migrate`
* rellenar la base de datos con dummy data usando: `$ php artisan db:seed`
* correr el backend usando: `$ php artisan serve`

`ANGULAR JS`
Una vez descomprimida la carpeta:
* Descargar dependencias de Node: `$ npm install`
* Descargar dependencias de Bower: `$ gulp bower`
* Enlazar dependencias Bower a index.html: `$ gulp wiredep`
* Agregar nuevos archivos JS a archivo index.html: `$ gulp inject`
* Generar versión de producción: `$ gulp build`
* Iniciar servidor de desarrollo: `$ gulp serve` (se debiese abrir el navegador con la aplicacion web)


