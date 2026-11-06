# Administración de Linux

[Volver al portafolio](../../README.md)

Las siguientes descripciones se basan en las notas originales. Las evidencias sugeridas están pendientes y no representan resultados verificados.

## Red, usuarios y permisos

Notas sobre DHCP, IP estática, usuarios, grupos, propiedad y permisos de archivos.

**Notas:** [red-usuarios-permisos.txt](red-usuarios-permisos.txt).

**Evidencia por añadir:** Configuración de interfaz, grupos del usuario y permisos de archivos de prueba.

## Scripts Bash de respaldo y red

Script de archivo tar.gz del home con fecha y otro para guardar ifconfig o ip a en un archivo.

**Notas:** [scripts-backup-red.txt](scripts-backup-red.txt).

**Evidencia por añadir:** Archivo de respaldo con fecha y archivo de información de red; una restauración no está documentada.

## Programación con cron y at

Ejemplos de actualización de paquetes, reinicio semanal y una tarea puntual de limpieza.

**Notas:** [cron-at.txt](cron-at.txt).

**Evidencia por añadir:** Entradas programadas y cola de at; aportar salida de ejecución si se realiza.

## GRUB y recuperación de acceso

Notas de edición de GRUB, arranque con init=/bin/bash y cambio de contraseña de un usuario.

**Notas:** [grub-recuperacion.txt](grub-recuperacion.txt).

**Evidencia por añadir:** Secuencia de recuperación en una VM de prueba e inicio de sesión posterior, sin mostrar /etc/shadow.

## Repositorios APT y Bashtop

Consulta y actualización de repositorios, instalación, ejecución y eliminación de Bashtop.

**Notas:** [apt-bashtop.txt](apt-bashtop.txt).

**Evidencia por añadir:** Repositorios consultados y panel de Bashtop en funcionamiento.

## Administración con Webmin

Instalación de un paquete .deb, resolución de dependencias y acceso web al puerto 10000.

**Notas:** [webmin.txt](webmin.txt).

**Evidencia por añadir:** Estado del servicio y panel de Webmin con datos personales ocultos.

Consultar también la [revisión técnica](../../docs/revision-tecnica.md).
