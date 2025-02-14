# Proyecto E-commerce de Compra de Entradas al Cine

Este es un proyecto de e-commerce para la compra de entradas al cine, con funcionalidades de carrito de compras, historial de compras y pagos, todo implementado utilizando microservicios y contenedores Docker.

## Requisitos Previos

Antes de comenzar, asegúrate de tener instalados los siguientes programas:

- Docker - Java 11 - Maven

## Pasos para la configuración

1. Revisar la documentación (Página 72 sobre Docker)

Es importante que revises el documento del proyecto en la parte que explica sobre el uso de Docker. Ve a la página 72 para entender cómo están configurados los contenedores y cómo se ejecutan.

2. Ejecutar el script install.cmd

- Navega hasta la carpeta donde se encuentra el archivo install.cmd. - Ejecuta el siguiente comando en la terminal de Windows: bash install.cmd

Este script inicializa los contenedores de Docker y configura los servicios del proyecto.

3. Compilar los proyectos

Una vez que los contenedores estén funcionando, debes compilar cada uno de los microservicios. Para ello:

- Navega a la carpeta de cada repositorio correspondiente (por ejemplo, security, payment, cart, etc.). - Ejecuta el siguiente comando de Maven para limpiar y compilar el proyecto:
``` bash
mvn clean install
```
Esto descargará las dependencias necesarias y compilará el proyecto.

4. Ejecutar la aplicación con run.bat

Después de construir los proyectos, ejecuta el archivo run.bat que se encuentra en el directorio principal del proyecto o en el directorio del microservicio correspondiente. Este script levantará los servicios y pondrá en marcha la aplicación.

Ejecuta: 
```bash
run.bat
```
5. Acceder a la aplicación

Una vez que todo esté corriendo, puedes acceder a la aplicación web a través del navegador en la URL configurada en los contenedores de Docker (por lo general, http://localhost:3000).

## Notas Adicionales

- Problemas comunes: Si tienes algún problema al ejecutar mvn clean install o mvn clean package, asegúrate de tener todas las dependencias correctas y de estar utilizando la versión de Java adecuada (Java 11). - Contenedores Docker: Los contenedores de Docker deben estar ejecutándose correctamente. Si tienes problemas con los contenedores, revisa los logs de Docker para identificar el problema.
