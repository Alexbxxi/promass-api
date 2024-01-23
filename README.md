# promass-api 🚀 

Esta aplicación contiene el backend de una app tipo Blogspot, hecho con buenas practicas y arquitectura de monolíto.

## Requisitos
Este proyecto ha sido realizado con NodeJs v20.10.0 + Express(last version) + TypeOrm(last version)

1.- Tener instalado el cliente de PostgreSQL.
<br>
2.- Tener instalado el cliente de Docker y la aplicación de escritorio (de preferencia) o alguna alternativa para gestionar contenedores.
<br>

## Pasos para la instalación

1.- Descargar o clonar el repositorio.
<br>
2.- Ejecutar el comando <code>npm install</code>
<br>
3.- Instalar el cliente de PostgreSQL localmente, crear una nueva conexión y una base datos con las características proporcionadas por mail del archivo enviroment.txt
<br>

<h3OPCIONAL</h3>
En dado caso de no tener instalado localmente el cliente de PosgreSQL y tener Docker seguir los siguientes pasos:
<br>
3.- Descarga la imagen oficial de PostgreSQL: <code>docker pull postgres</code>
<br>
4.- Verificar el estado del contenedor: <code>docker ps</code>
<br>
5.- Este comando crea la imagen, la instancia y la de la base de datos: <code>docker run -d --name mi-postgres-container -e POSTGRES_USER=postgres -e POSTGRES_PASSWORD=admin -e POSTGRES_DB=dev.PROMASS_BLOG -p 5432:5432 postgres</code> 
<br>
(En el comando donde dice "mi-postgres-container pueden poner cualquier nombre a su contenedor).


## Pasos para levantar el proyecto

1.- Ejecutar el comando <code>npm start</code> esto inicia el proyecto, hace la sincronización de la base de datos, las migraciones correspondientes y crea la carpeta dist con el transpilado a Javascript.

## Notas

(IMPORTANTE): Se tiene que crear un archivo <code>.env</code> para poder cargar las variables de entorno de la base de datos, el contenido de este archivo se manda por correo, como buena práctica de seguridad no se suben al repositorio.

Desarrollado por @Alexbxxi 🤖 para el examen de Frontend Developer para Grupo PROMASS.
