# Servicios de red e interoperabilidad

[Volver al portafolio](../../README.md)

Las siguientes descripciones se basan en las notas originales. Las evidencias sugeridas están pendientes y no representan resultados verificados.

## Archivos compartidos con NFS

Exportación de /OS3 y montaje desde un cliente Linux; incluye una propuesta de persistencia en fstab.

**Notas:** [nfs.txt](nfs.txt).

**Evidencia por añadir:** Exportación activa y listado de /mnt desde el cliente, también después de reiniciar.

## Servidor de archivos Samba

Recurso shared con usuario autenticado, permisos de grupo y acceso desde una unidad de red de Windows.

**Notas:** [samba-fileserver.txt](samba-fileserver.txt).

**Evidencia por añadir:** Unidad compartida en Windows, permisos de shared y contenido del archivo editado visto desde Linux.

## Servidor HTTP Apache

Instalación de Apache, edición de index.html y cambio del puerto de escucha a 8080.

**Notas:** [apache.txt](apache.txt).

**Evidencia por añadir:** Servicio activo y página personalizada accesible en el puerto 8080.

## SMTP con Postfix

Configuración de un relay Gmail con SASL y TLS, envío mediante mail y consulta de la cola.

**Notas:** [postfix.txt](postfix.txt).

**Evidencia por añadir:** Configuración sin credenciales, estado del servicio, cola y mensaje recibido con cabeceras personales ocultas.

## Impresión compartida con CUPS

Instalación de CUPS y cups-pdf, administración web y conexión de una impresora desde el host.

**Notas:** [cups.txt](cups.txt).

**Evidencia por añadir:** Impresora visible en la interfaz y hoja de prueba o PDF generado.

## Telefonía con Issabel y MicroSIP

Notas de instalación de Issabel sobre Rocky Linux 8 y configuración de extensiones y una cuenta MicroSIP.

**Notas:** [issabel-microsip.txt](issabel-microsip.txt).

**Evidencia por añadir:** Extensiones configuradas y cuenta registrada sin contraseñas; una llamada de prueba sería evidencia adicional pendiente.

Consultar también la [revisión técnica](../../docs/revision-tecnica.md).
