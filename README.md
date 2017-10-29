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
`PHP`









`ANGULAR JS`
Una vez descomprimida la carpeta:
* Descargar dependencias de Node: `$ npm install`
* Descargar dependencias de Bower: `$ gulp bower`
* Enlazar dependencias Bower a index.html: `$ gulp wiredep`
* Agregar nuevos archivos JS a archivo index.html: `$ gulp inject`
* Generar versión de producción: `$ gulp build`
* Iniciar servidor de desarrollo: `$ gulp serve` (se debiese abrir el navegador con la aplicacion web)


