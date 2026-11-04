# Gestión de servicios en el sistema informático

Prácticas de diseño y simulación de redes con **Cisco Packet Tracer**, configuración de servicios, seguridad perimetral y monitorización de servidores Linux.

## Sobre la asignatura

En esta asignatura trabajé cómo se comunican los equipos de una red, cómo se configuran los servicios que utilizan y cómo se supervisa su funcionamiento. Combiné fundamentos de redes con simulaciones en Packet Tracer y prácticas sobre máquinas virtuales Debian.

Este repositorio está dedicado al trabajo académico de la **UD01: Gestión de la seguridad y normativas**. Los contenidos resumidos aquí corresponden a las actividades de redes, seguridad y monitorización documentadas en la memoria de prácticas.

## Contenidos trabajados

| Área | Contenidos |
| --- | --- |
| Fundamentos de redes | Modelos OSI y TCP/IP, direccionamiento IPv4, máscaras de red, direcciones públicas y privadas, puertos y puertas de enlace. |
| Simulación con Packet Tracer | Diseño de topologías con routers, switches, puntos de acceso, equipos cliente y servidores; configuración de redes cableadas e inalámbricas. |
| Servicios de red | Resolución de nombres mediante DNS y acceso a páginas web mediante HTTP. |
| Conectividad y acceso | NAT, concepto de CG-NAT y redirección de puertos para acceder a servicios de redes privadas. |
| Seguridad de red | Autenticación Wi-Fi WPA2-PSK y prácticas con el cortafuegos IPCop y una zona desmilitarizada (DMZ). |
| Monitorización | Supervisión de disponibilidad, HTTP, CPU, memoria RAM y disco mediante Nagios 4 y NCPA. |

## Prácticas destacadas

### Diseño y simulación de redes con Cisco Packet Tracer

- Creación de topologías con varias redes conectadas mediante routers.
- Configuración de direcciones IP, máscaras y puertas de enlace.
- Configuración de redes inalámbricas y autenticación WPA2-PSK.
- Acceso desde equipos cliente a un servidor web utilizando un servidor DNS.
- Uso de NAT y redirección de puertos en redes privadas.
- Análisis del intercambio de mensajes entre clientes y servidores.

### Seguridad perimetral con IPCop y DMZ

Práctica de configuración de un entorno con IPCop, una red interna y una DMZ destinada a alojar un servidor web Debian. Se trabajó la separación de zonas de red y se realizaron comprobaciones de conectividad y acceso al servicio HTTP.

### Monitorización de un servidor Debian con Nagios y NCPA

Configuración de un servidor Nagios 4 para supervisar otra máquina Debian mediante el agente NCPA. Las comprobaciones incluyeron:

- Disponibilidad del equipo.
- Funcionamiento del servicio HTTP.
- Uso de CPU, memoria RAM y disco.
- Umbrales de estado `WARNING` y `CRITICAL`.

La práctica incluyó la validación de la configuración y la resolución de incidencias relacionadas con la conectividad, el módulo CGI de Apache, la ejecución del plugin de NCPA, los permisos y las métricas consultadas.

## Herramientas y tecnologías

- **Cisco Packet Tracer:** diseño, configuración y simulación de redes.
- **Debian GNU/Linux:** administración de equipos y servicios.
- **IPCop:** cortafuegos y configuración de zonas de red.
- **Apache HTTP Server:** servicio web e interfaz de Nagios.
- **Nagios 4 y NCPA:** monitorización de equipos, servicios y recursos.
- **UTM y VirtualBox:** entornos de virtualización utilizados en las prácticas.
- **Herramientas de diagnóstico:** `ip`, `ping`, `curl`, `nc`, `ss` y `systemctl`.

## Aprendizajes

- Relacionar los conceptos de redes con su funcionamiento en un entorno práctico.
- Diseñar y comprobar topologías de red en Packet Tracer.
- Configurar servicios DNS y HTTP y verificar su accesibilidad.
- Comprender la función de NAT, los cortafuegos y las DMZ.
- Interpretar estados y métricas para detectar problemas en servidores.
- Diagnosticar incidencias y documentar las soluciones aplicadas.

---

Trabajo académico realizado en entornos de simulación y laboratorio.
