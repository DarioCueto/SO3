# Evidencias pendientes para el portafolio

[Volver al portafolio](../README.md)

En el árbol original revisado no hay capturas, logs ni salidas de ejecución guardadas. Esta lista propone qué añadir; ninguna evidencia se ha creado o dado por obtenida.

## Prioridad de presentación

Empezar por Suricata, Samba AD DC, Ansible, Terraform y Docker/Compose permite respaldar las prácticas de detección, identidad, automatización e infraestructura descritas en las notas. Continuar con los servicios y la administración Linux.

| Laboratorio | Evidencia sugerida |
| --- | --- |
| [Ansible: Linux y Windows](../labs/automatizacion/ansible.txt) | Inventario sin credenciales y salidas reales de ping y win_ping. |
| [Ansible: tareas ad hoc](../labs/automatizacion/ad-hoc.txt) | Archivo antes y después del movimiento y salida de la tarea de reinicio. |
| [Ansible: playbooks](../labs/automatizacion/playbooks.txt) | PLAY RECAP de cada ejecución, aplicación instalada y actualización de caché. |
| [Terraform y DigitalOcean](../labs/automatizacion/terraform-digitalocean.txt) | Salida de validate y apply, Droplet en el panel y conexión SSH; ocultar tokens. |
| [Docker y Nginx](../labs/contenedores/docker-nginx.txt) | docker ps -a y página servida en el puerto 8888. |
| [WordPress con Docker Compose](../labs/contenedores/wordpress-compose.txt) | Contenedores en ejecución y pantalla de configuración de WordPress en el puerto 8081. |
| [Administración con Portainer](../labs/contenedores/portainer.txt) | Panel de contenedores y estado de Nginx antes y después de detenerlo. |
| [Samba AD DC y cliente Windows](../labs/identidad-y-acceso/samba-ad-dc.txt) | Estado de samba-ad-dc, autenticación Kerberos, pertenencia de Windows al dominio e inicio de sesión del usuario. |
| [SSH en máquina virtual](../labs/identidad-y-acceso/ssh-en-vm.txt) | Estado del servicio SSH y conexión mediante clave pública; nunca mostrar la clave privada. |
| [Segundo factor para SSH con PAM](../labs/identidad-y-acceso/pam-ssh-2fa.txt) | Solicitud de contraseña y segundo factor durante una sesión de prueba, ocultando QR, semilla y códigos. |
| [Archivos compartidos con NFS](../labs/servicios-de-red/nfs.txt) | Exportación activa y listado de /mnt desde el cliente, también después de reiniciar. |
| [Servidor de archivos Samba](../labs/servicios-de-red/samba-fileserver.txt) | Unidad compartida en Windows, permisos de shared y contenido del archivo editado visto desde Linux. |
| [Servidor HTTP Apache](../labs/servicios-de-red/apache.txt) | Servicio activo y página personalizada accesible en el puerto 8080. |
| [SMTP con Postfix](../labs/servicios-de-red/postfix.txt) | Configuración sin credenciales, estado del servicio, cola y mensaje recibido con cabeceras personales ocultas. |
| [Impresión compartida con CUPS](../labs/servicios-de-red/cups.txt) | Impresora visible en la interfaz y hoja de prueba o PDF generado. |
| [Telefonía con Issabel y MicroSIP](../labs/servicios-de-red/issabel-microsip.txt) | Extensiones configuradas y cuenta registrada sin contraseñas; una llamada de prueba sería evidencia adicional pendiente. |
| [Reglas de detección con Suricata](../labs/seguridad/suricata.txt) | Reglas cargadas y alertas reales de fast.log vinculadas a cada prueba de tráfico. |
| [Filtrado con iptables y UFW](../labs/seguridad/iptables-ufw.txt) | Reglas de iptables y estado de UFW, junto con pruebas de conexión antes y después. |
| [Cifrado simétrico con GPG](../labs/seguridad/gpg2.txt) | Archivo .gpg y contenido recuperado de un mensaje de prueba sin información sensible. |
| [Red, usuarios y permisos](../labs/administracion-linux/red-usuarios-permisos.txt) | Configuración de interfaz, grupos del usuario y permisos de archivos de prueba. |
| [Scripts Bash de respaldo y red](../labs/administracion-linux/scripts-backup-red.txt) | Archivo de respaldo con fecha y archivo de información de red; una restauración no está documentada. |
| [Programación con cron y at](../labs/administracion-linux/cron-at.txt) | Entradas programadas y cola de at; aportar salida de ejecución si se realiza. |
| [GRUB y recuperación de acceso](../labs/administracion-linux/grub-recuperacion.txt) | Secuencia de recuperación en una VM de prueba e inicio de sesión posterior, sin mostrar /etc/shadow. |
| [Repositorios APT y Bashtop](../labs/administracion-linux/apt-bashtop.txt) | Repositorios consultados y panel de Bashtop en funcionamiento. |
| [Administración con Webmin](../labs/administracion-linux/webmin.txt) | Estado del servicio y panel de Webmin con datos personales ocultos. |

## Organización propuesta para futuras evidencias

Una vez obtenidas, guardar las capturas y salidas en `labs/<categoria>/evidencias/<laboratorio>/` y enlazarlas desde el README del área. Esta ruta es una propuesta; no se crean carpetas con evidencia ficticia.

Acompañar cada evidencia con fecha, entorno utilizado, acción ejecutada y observación concreta. Una captura del servicio activo acredita ese estado puntual; para demostrar una función, incluir también la prueba del cliente o la salida correspondiente. Si falla, registrar el error y la limitación.

Ocultar contraseñas, tokens, claves privadas, semillas/QR de segundo factor y datos personales. No publicar archivos de estado de Terraform ni capturas de secretos.
