# Seguridad y detección de tráfico

[Volver al portafolio](../../README.md)

Las siguientes descripciones se basan en las notas originales. Las evidencias sugeridas están pendientes y no representan resultados verificados.

## Reglas de detección con Suricata

Instalación y reglas de alerta para ICMP y tráfico TCP hacia FTP, SSH y HTTP; seguimiento de fast.log.

**Notas:** [suricata.txt](suricata.txt).

**Evidencia por añadir:** Reglas cargadas y alertas reales de fast.log vinculadas a cada prueba de tráfico.

## Filtrado con iptables y UFW

Ejemplos para bloquear y permitir tráfico TCP en los puertos 21, 22 y 80.

**Notas:** [iptables-ufw.txt](iptables-ufw.txt).

**Evidencia por añadir:** Reglas de iptables y estado de UFW, junto con pruebas de conexión antes y después.

## Cifrado simétrico con GPG

Creación de un archivo, cifrado mediante gpg2 -c y recuperación del texto con gpg --decrypt.

**Notas:** [gpg2.txt](gpg2.txt).

**Evidencia por añadir:** Archivo .gpg y contenido recuperado de un mensaje de prueba sin información sensible.

Consultar también la [revisión técnica](../../docs/revision-tecnica.md).
