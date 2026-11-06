# Contenedores y aplicaciones

[Volver al portafolio](../../README.md)

Las siguientes descripciones se basan en las notas originales. Las evidencias sugeridas están pendientes y no representan resultados verificados.

## Docker y Nginx

Instalación de Docker y contenedor Nginx con puerto 8888 del host y un directorio de contenido HTML montado.

**Notas:** [docker-nginx.txt](docker-nginx.txt).

**Evidencia por añadir:** docker ps -a y página servida en el puerto 8888.

## WordPress con Docker Compose

Ejemplo de dos servicios: WordPress en el puerto 8081 y MySQL 5.7, con variables de entorno y depends_on.

**Notas:** [wordpress-compose.txt](wordpress-compose.txt).

**Evidencia por añadir:** Contenedores en ejecución y pantalla de configuración de WordPress en el puerto 8081.

## Administración con Portainer

Despliegue de Portainer con acceso al socket Docker y volumen de datos; describe detener Nginx desde la interfaz.

**Notas:** [portainer.txt](portainer.txt).

**Evidencia por añadir:** Panel de contenedores y estado de Nginx antes y después de detenerlo.

Consultar también la [revisión técnica](../../docs/revision-tecnica.md).
