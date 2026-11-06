# Revisión del material original

[Volver al portafolio](../README.md)

Revisión de lectura del contenido original del commit `59281dce44601bbcc97f0640b288fe120016285a`. No se ejecutaron los comandos ni se consultaron otras fuentes para ampliar los laboratorios. Las siguientes observaciones identifican aspectos que deben comprobarse al reproducir las notas; no se presentan como correcciones ya probadas.

| Archivo organizado | Observación del contenido |
| --- | --- |
| [Ansible](../labs/automatizacion/ansible.txt) | Contiene contraseñas literales, WinRM Basic con tráfico sin cifrar y una indicación de desactivar el firewall. Algunas variables aparecen juntas en una línea. Revisar credenciales, formato y transporte antes de reutilizarlo. |
| [Terraform](../labs/automatizacion/terraform-digitalocean.txt) | El Droplet se llama `OS3vm`, pero el firewall referencia `digitalocean_droplet.ubuntu_server.id`. El ejemplo permite SSH desde cualquier origen. No hay salida de validate o apply que confirme su ejecución. |
| [Suricata](../labs/seguridad/suricata.txt) | El nombre original menciona Snort, pero no incluye pasos de Snort. La ruta del comando de ejecución difiere de la ruta del YAML editado; la explicación final asigna FTP al puerto 22 aunque su regla usa 21. Son alertas de tráfico, sin pruebas almacenadas de detección de ataques ni modo IPS. |
| [Samba AD DC](../labs/identidad-y-acceso/samba-ad-dc.txt) | Documenta un controlador Samba en Linux con cliente Windows. La línea para crear un usuario incluye una sintaxis de contraseña que requiere revisión. No incluye GPO ni evidencias de administración con Windows Server. |
| [NFS](../labs/servicios-de-red/nfs.txt) | El origen del comando mount usa `servidor:/OS3`, mientras que la entrada propuesta en fstab omite los dos puntos. Revisar antes de probar la persistencia. |
| [Samba fileserver](../labs/servicios-de-red/samba-fileserver.txt) | Las notas incluyen `user add`, una ruta `/user/sbin/nologin` y un bucle con sudo cuya sintaxis debe revisarse. También ofrecen una alternativa de creación de archivos. |
| [PAM/SSH](../labs/identidad-y-acceso/pam-ssh-2fa.txt) | La línea destinada a reiniciar el servicio no incluye una acción de systemctl. No hay salida de una sesión que demuestre el segundo factor. |
| [SSH](../labs/identidad-y-acceso/ssh-en-vm.txt) | La secuencia entre host y VM y los permisos indicados para authorized_keys necesitan revisión. No hay captura de autenticación por clave. |
| [Apache](../labs/servicios-de-red/apache.txt) | Describe cambiar ports.conf a 8080, sin documentar una revisión del VirtualHost. Falta comprobar la escucha y la respuesta efectiva. |
| [Postfix](../labs/servicios-de-red/postfix.txt) | Hay líneas de servicio y parámetros con posibles errores de escritura, además de un ejemplo de credenciales. Las notas interpretan una cola vacía como éxito, pero no aportan el mensaje recibido que respalde la entrega. |
| [Docker/Compose](../labs/contenedores/wordpress-compose.txt) | Define WordPress y MySQL 5.7 con contraseñas de ejemplo; no define volúmenes persistentes para esos servicios. No atribuir persistencia de la base de datos a este ejemplo. |
| [Portainer](../labs/contenedores/portainer.txt) | La imagen usada en pull difiere de la usada en run. El montaje del socket Docker y la administración de Nginx aparecen en las notas, sin captura del resultado. |
| [Cron y at](../labs/administracion-linux/cron-at.txt) | update y upgrade se programan al mismo minuto sin documentar coordinación. La tarea de limpieza elimina contenido de /tmp. No hay registro de ejecución. |
| [Bash y backup](../labs/administracion-linux/scripts-backup-red.txt) | Se documenta crear un tar.gz y guardar información de red. No se documenta restaurar el respaldo ni comprobar su integridad. |
| [GRUB](../labs/administracion-linux/grub-recuperacion.txt) | Incluye edición directa de /etc/shadow durante la recuperación. No hay prueba guardada de recuperación; no publicar ese archivo como evidencia. |
| [CUPS](../labs/servicios-de-red/cups.txt) e [Issabel](../labs/servicios-de-red/issabel-microsip.txt) | CUPS propone acceso amplio y administración remota. Issabel incluye detener fail2ban, contraseñas literales y números de extensión que no coinciden entre pasos. Revisar antes de reutilizar; no se documenta una llamada completada. |

## Qué conserva esta reorganización

Los archivos de notas mantienen íntegro su contenido, incluidos sus errores y ejemplos originales, para separar la organización editorial de una futura revisión técnica. Los nuevos documentos no afirman que las configuraciones hayan sido corregidas o validadas. Las credenciales que aparecen en las notas no se reproducen en los resúmenes; si alguna sigue en uso, debe sustituirse y revisarse su exposición previa.
