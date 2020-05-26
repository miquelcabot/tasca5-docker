# Tasca 5 - Desplegar una aplicació LAMP amb Docker

Nom de l'alumne = ________

## Enunciat

Desplegar mitjançant contenidors Docker una aplicació web simple, situada en aquest mateix repositori, desenvolupada amb PHP i MySQL.

Per desplegar aquesta aplicació serà necessari crear 3 contenidors:
* Un amb Apache, PHP i llibreries PHP per poder accedir a MySQL. En aquest contenidor s’hi han de copiar els fitxers HTML, PHP, etc… situats en la carpeta *www* d'aquest repositori. Es basarà en la imatge `php:7.3-apache`.
* Un amb un servidor de bases de dades MySQL. Aquest contenidor contindrà la base de dades a la que ha d’accedir l’aplicació web. Es basarà en la imatge `mysql:8.0`. S'ha d'inicialitzar amb les dades dels fitxers `*.sql` situats a la carpeta *sql* d'aquest repositori.
* Un amb l’aplicació PhpMyAdmin per poder administrar la base de dades MySQL mitjançant una interfície web. Es basarà en la imatge `phpmyadmin/phpmyadmin`.

Per tal de poder posar en marxa els tres contenidors de forma coordinada es recomana utilitzar l’eina Docker Compose (https://docs.docker.com/compose/).

Una vegada desplegats, el servidor web Apache es podrà accedir mitjançant el port 8080 de la màquina hoste, el servidor de base de dades MySQL es podrà accedir mitjançant el port 3306, i PhpMyAdmin mitjançant el port 8081.

A la següent captura de pantalla es pot veure el resultat d’accedir a l’aplicació web, una vegada desplegada i posada en funcionament:

![alt text](https://github.com/miquelcabot/tasca5-docker/blob/master/demo.png?raw=true "Demostració de l'aplicació")

Els punts que heu de lliurar per aquesta pràctica són:
1. Fitxer necessaris per configurar els contenidors Docker. Al mateix repositori hi heu d'afegir els fitxers `Dockerfile` i `docker-compose.yml` per tal de configurar els contenidors sol·licitats a l'enunciat.
2. Prerequisits de software per poder executar aquest projecte.
3. Instruccions per executar i aturar els contenidors.
4. Instruccions per accedir a la web del projecte i a phpMyAdmin. En principi, basta amb indicar les seves URLs.
5. Instruccions per accedir mitjançant terminal de comandes (bash shell) a cada un dels contenidors.
6. Instruccions per accedir al client MySQL del contenidor que té la base de dades mitjançant terminal de comandes.
7. Crear un `Project` per fer el seguiment de l'*Sprint* actual amb un diagrama [Kanban](https://es.wikipedia.org/wiki/Kanban) de tipus *Basic kanban*. Aquest *Sprint* ha de tenir almenys les següents *user stories* del *product backlog*, en forma de `Issues`, que tendran assignades a algún desenvolunpador del teu projecte:
   * L'aplicació web s'ha de desplegar a un contenidor de Docker
   * La base de dades s'ha de desplegar a un contenidor de Docker
   * Hi haurà un contenidor de Docker amb el programa phpMyAdmin per administrar la base de dades
   * L'administrador del sistema ha de poder entrar mitjançant terminal de comandes als contenidors
   * L'administrador del sistema ha de poder entrar mitjançant terminal de comandes al client MySQL

## 1. Fitxer necessaris per configurar els contenidors Docker
Mirar els fitxers `Dockerfile` i `docker-compose.yml` d'aquest repositori.

## 2. Prerequisits
(Completar)

## 3. Executar i aturar els contenidors
(Completar)

## 4. Accedir a la web i a phpMyAdmin
(Completar)

## 5. Entrar per terminal (bash shell) als contenidors 
(Completar)

## 6. Entrar al client MySQL per terminal
(Completar)

## 7. Seguiment del desenvolupament d'aquest Sprint
Mirar els menús `Issues` i `Projects` d'aquest repositori

## Format de lliurament

Has de lliurar a [Google Classroom](https://classroom.google.com) un enllaç a una release (publicació) d'aquest repositori de GitHub.

* [How to create releases](https://help.github.com/articles/creating-releases/)

## Referències

* [Exploring Docker 1 - Getting Started, Vídeo Youtube de Traversy Media](https://youtu.be/Kyx2PsuwomE)
* [Exploring Docker 2 - Docker Compose With Node & MongoDB, Vídeo Youtube de Traversy Media](https://youtu.be/hP77Rua1E0c)
* [LAMP con Docker](https://magmax.org/blog/lamp-con-docker/)
* [LAMP CON DOCKER, Vídeo Youtube](https://www.youtube.com/watch?v=lrhwWX49Uss)
* [Project management in GitHub](https://github.com/features/project-management/)
