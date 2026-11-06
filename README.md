# SO3 · Portafolio técnico
**Dario Cueto · Linux, redes, automatización y seguridad**

Este repositorio reúne mis notas de prácticas de Sistemas Operativos III. Está organizado para consultar procedimientos de administración Linux, servicios de red, acceso remoto, contenedores, automatización y detección de tráfico.

## Alcance y estado de la evidencia

El material original consiste en **25 archivos de texto** con pasos, comandos y fragmentos de configuración. No contiene capturas, logs de ejecución ni archivos de infraestructura independientes. Las descripciones presentan el alcance documentado; no certifican despliegues exitosos, funcionamiento en producción ni resultados medidos. Los procedimientos no se han ejecutado como parte de esta reorganización.

## Recorrido por los laboratorios

| Área | Prácticas documentadas |
| --- | --- |
| [Automatización e infraestructura como código](labs/automatizacion/README.md) | [Ansible: Linux y Windows](labs/automatizacion/ansible.txt) · [Ansible: tareas ad hoc](labs/automatizacion/ad-hoc.txt) · [Ansible: playbooks](labs/automatizacion/playbooks.txt) · [Terraform y DigitalOcean](labs/automatizacion/terraform-digitalocean.txt) |
| [Contenedores y aplicaciones](labs/contenedores/README.md) | [Docker y Nginx](labs/contenedores/docker-nginx.txt) · [WordPress con Docker Compose](labs/contenedores/wordpress-compose.txt) · [Administración con Portainer](labs/contenedores/portainer.txt) |
| [Identidad y acceso remoto](labs/identidad-y-acceso/README.md) | [Samba AD DC y cliente Windows](labs/identidad-y-acceso/samba-ad-dc.txt) · [SSH en máquina virtual](labs/identidad-y-acceso/ssh-en-vm.txt) · [Segundo factor para SSH con PAM](labs/identidad-y-acceso/pam-ssh-2fa.txt) |
| [Servicios de red e interoperabilidad](labs/servicios-de-red/README.md) | [Archivos compartidos con NFS](labs/servicios-de-red/nfs.txt) · [Servidor de archivos Samba](labs/servicios-de-red/samba-fileserver.txt) · [Servidor HTTP Apache](labs/servicios-de-red/apache.txt) · [SMTP con Postfix](labs/servicios-de-red/postfix.txt) · [Impresión compartida con CUPS](labs/servicios-de-red/cups.txt) · [Telefonía con Issabel y MicroSIP](labs/servicios-de-red/issabel-microsip.txt) |
| [Seguridad y detección de tráfico](labs/seguridad/README.md) | [Reglas de detección con Suricata](labs/seguridad/suricata.txt) · [Filtrado con iptables y UFW](labs/seguridad/iptables-ufw.txt) · [Cifrado simétrico con GPG](labs/seguridad/gpg2.txt) |
| [Administración de Linux](labs/administracion-linux/README.md) | [Red, usuarios y permisos](labs/administracion-linux/red-usuarios-permisos.txt) · [Scripts Bash de respaldo y red](labs/administracion-linux/scripts-backup-red.txt) · [Programación con cron y at](labs/administracion-linux/cron-at.txt) · [GRUB y recuperación de acceso](labs/administracion-linux/grub-recuperacion.txt) · [Repositorios APT y Bashtop](labs/administracion-linux/apt-bashtop.txt) · [Administración con Webmin](labs/administracion-linux/webmin.txt) |

## Prácticas destacadas

| Práctica | Alcance de las notas |
| --- | --- |
| [Ansible](labs/automatizacion/README.md) | Inventario mixto Linux/Windows, SSH, WinRM, tareas ad hoc y dos playbooks. |
| [Terraform](labs/automatizacion/terraform-digitalocean.txt) | Droplet Ubuntu en DigitalOcean, clave SSH y fragmento opcional de firewall. |
| [Docker y Compose](labs/contenedores/README.md) | Nginx con directorio montado, WordPress con MySQL y administración con Portainer. |
| [Samba AD DC](labs/identidad-y-acceso/samba-ad-dc.txt) | Dominio, DNS, Kerberos y unión de un cliente Windows mediante Samba en Linux. |
| [PAM y SSH](labs/identidad-y-acceso/pam-ssh-2fa.txt) | Configuración de un segundo factor con Google Authenticator. |
| [Suricata](labs/seguridad/suricata.txt) | Reglas para alertar sobre ICMP y conexiones a FTP, SSH y HTTP. |
| [NFS y Samba](labs/servicios-de-red/README.md) | Compartición de archivos entre Linux y acceso autenticado desde Windows. |

## Estructura

| Ruta | Contenido |
| --- | --- |
| `labs/automatizacion/` | Automatización e infraestructura como código; README con descripciones y notas originales. |
| `labs/contenedores/` | Contenedores y aplicaciones; README con descripciones y notas originales. |
| `labs/identidad-y-acceso/` | Identidad y acceso remoto; README con descripciones y notas originales. |
| `labs/servicios-de-red/` | Servicios de red e interoperabilidad; README con descripciones y notas originales. |
| `labs/seguridad/` | Seguridad y detección de tráfico; README con descripciones y notas originales. |
| `labs/administracion-linux/` | Administración de Linux; README con descripciones y notas originales. |
| [docs/evidencias.md](docs/evidencias.md) | Capturas y salidas que conviene incorporar, todas pendientes. |
| [docs/revision-tecnica.md](docs/revision-tecnica.md) | Inconsistencias observadas y límites del material. |
| [docs/mapa-de-archivos.md](docs/mapa-de-archivos.md) | Correspondencia completa entre nombres anteriores y rutas organizadas. |

## Cómo consultar este portafolio

1. Abrir el área de interés y leer la descripción de la práctica.
2. Consultar el archivo de notas enlazado.
3. Revisar las observaciones técnicas antes de intentar reproducirlo.
4. Aportar las evidencias sugeridas únicamente después de obtenerlas en el laboratorio.

Las notas originales se conservan sin cambios de contenido. Algunas incluyen credenciales escritas y configuraciones permisivas de laboratorio; están señaladas en la revisión técnica. Los fragmentos son documentación histórica y requieren revisión antes de reutilizarse.
