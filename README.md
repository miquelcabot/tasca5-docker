# Tasca 5 - Desplegar una aplicació LAMP amb Docker

Nom de l'alumne = ________

## Enunciat

Desplegar mitjançant contenidors Docker una aplicació web simple, situada en aquest mateix repositori, desenvolupada amb PHP i MySQL.

Per desplegar aquesta aplicació serà necessari crear 3 contenidors:
* Un amb Apache, PHP i llibreries PHP per poder accedir a MySQL. En aquest contenidor s’hi han de copiar els fitxers HTML, PHP, etc… situats en la carpeta *www* d'aquest repositori. Es basarà en la imatge “php:7.3-apache”.
* Un amb un servidor de bases de dades MySQL. Aquest contenidor contindrà la base de dades a la que ha d’accedir l’aplicació web. Es basarà en la imatge “mysql:8.0”. S'ha d'inicialitzar amb les dades dels fitxers `*.sql` situats a la carpeta *sql* d'aquest repositori.
* Un amb l’aplicació PhpMyAdmin per poder administrar la base de dades MySQL mitjançant una interfície web. Es basarà en la imatge “phpmyadmin/phpmyadmin”.

Per tal de poder posar en marxa els tres contenidors de forma coordinada es recomana utilitzar l’eina Docker Compose (https://docs.docker.com/compose/).
Una vegada desplegats, el servidor web Apache es podrà accedir mitjançant el port 8080 de la màquina hoste, el servidor de base de dades MySQL es podrà accedir mitjançant el port 3306, i PhpMyAdmin mitjançant el port 8081.

A la següent captura de pantalla es pot veure el resultat d’accedir a l’aplicació web, una vegada desplegada i posada en funcionament:
![alt text](https://github.com/miquelcabot/tasca5-docker/blob/master/demo.png?raw=true "Demostració de l'aplicació")

## Format de lliurament

Has de lliurar a [Google Classroom](https://classroom.google.com) un enllaç a una release (publicació) d'aquest repositori de GitHub.

* [How to create releases](https://help.github.com/articles/creating-releases/)

## Referències

* [Exploring Docker 1 - Getting Started, Vídeo Youtube de Traversy Media](https://youtu.be/Kyx2PsuwomE)
* [Exploring Docker 2 - Docker Compose With Node & MongoDB, Vídeo Youtube de Traversy Media](https://youtu.be/hP77Rua1E0c)
* [LAMP con Docker](https://magmax.org/blog/lamp-con-docker/)
* [LAMP CON DOCKER, Vídeo Youtube](https://www.youtube.com/watch?v=lrhwWX49Uss)
