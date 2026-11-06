# Automatización e infraestructura como código

[Volver al portafolio](../../README.md)

Las siguientes descripciones se basan en las notas originales. Las evidencias sugeridas están pendientes y no representan resultados verificados.

## Ansible: Linux y Windows

Configuración de inventario, acceso SSH a Linux y WinRM a Windows; incluye pruebas con ping y win_ping.

**Notas:** [ansible.txt](ansible.txt).

**Evidencia por añadir:** Inventario sin credenciales y salidas reales de ping y win_ping.

## Ansible: tareas ad hoc

Movimiento de un archivo en Windows mediante win_shell y reinicio de un host Linux con become.

**Notas:** [ad-hoc.txt](ad-hoc.txt).

**Evidencia por añadir:** Archivo antes y después del movimiento y salida de la tarea de reinicio.

## Ansible: playbooks

Ejemplos YAML para descargar e instalar Notepad++ en Windows y actualizar la caché APT en Linux.

**Notas:** [playbooks.txt](playbooks.txt).

**Evidencia por añadir:** PLAY RECAP de cada ejecución, aplicación instalada y actualización de caché.

## Terraform y DigitalOcean

Configuración de un Droplet Ubuntu 22.04 en nyc1, clave SSH, salida de IP y un fragmento opcional de firewall.

**Notas:** [terraform-digitalocean.txt](terraform-digitalocean.txt).

**Evidencia por añadir:** Salida de validate y apply, Droplet en el panel y conexión SSH; ocultar tokens.

Consultar también la [revisión técnica](../../docs/revision-tecnica.md).
