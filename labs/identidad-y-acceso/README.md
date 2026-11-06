# Identidad y acceso remoto

[Volver al portafolio](../../README.md)

Las siguientes descripciones se basan en las notas originales. Las evidencias sugeridas están pendientes y no representan resultados verificados.

## Samba AD DC y cliente Windows

Aprovisionamiento de un dominio con Samba, configuración de DNS y Kerberos, creación de usuario y unión de Windows al dominio.

**Notas:** [samba-ad-dc.txt](samba-ad-dc.txt).

**Evidencia por añadir:** Estado de samba-ad-dc, autenticación Kerberos, pertenencia de Windows al dominio e inicio de sesión del usuario.

## SSH en máquina virtual

Instalación de OpenSSH, conexión desde PowerShell y configuración de authorized_keys para acceso mediante clave pública.

**Notas:** [ssh-en-vm.txt](ssh-en-vm.txt).

**Evidencia por añadir:** Estado del servicio SSH y conexión mediante clave pública; nunca mostrar la clave privada.

## Segundo factor para SSH con PAM

Configuración de pam_google_authenticator y opciones de SSH para solicitar un código de segundo factor.

**Notas:** [pam-ssh-2fa.txt](pam-ssh-2fa.txt).

**Evidencia por añadir:** Solicitud de contraseña y segundo factor durante una sesión de prueba, ocultando QR, semilla y códigos.

Consultar también la [revisión técnica](../../docs/revision-tecnica.md).
