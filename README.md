# CyberLab – Laboratorio de Ciberseguridad

Todas las pruebas fueron realizadas en un entorno virtual aislado (Host-Only Network) con fines exclusivamente educativos.
Repositorio que documenta prácticas de ciberseguridad realizadas en un entorno virtual utilizando VirtualBox y Kali Linux.  
Incluye análisis de red, escaneo de puertos, captura de tráfico y pruebas básicas en entorno controlado con herramientas como Nmap, Wireshark y Metasploit.

---

## Objetivos del laboratorio

- Implementar un entorno virtual seguro para pruebas.
- Realizar escaneo de puertos y detección de servicios.
- Analizar tráfico de red.
- Evaluar vulnerabilidades en entorno controlado y documentar hallazgos.

---

## Herramientas utilizadas

- VirtualBox
- Kali Linux
- Nmap
- Wireshark
- Metasploit

---

## Configuración del entorno

1. Instalación de VirtualBox.
2. Creación de máquina virtual con Kali Linux.
3. Configuración de red en modo NAT / Adaptador Puente.
4. Verificación de conectividad entre máquinas.

---

## Escaneo de red con Nmap

Ejemplo de comando utilizado:
```bash
nmap -sV -p 1-65535 192.168.56.101
```

Descripción:
- `-sV` → Detecta versión de servicios.
- `-p 1-65535` → Escanea todos los puertos.
- IP objetivo → Máquina dentro del entorno virtual.

Objetivo:
Identificar puertos abiertos y servicios activos para análisis posterior.

---

## Análisis de tráfico con Wireshark

- Captura de paquetes en la interfaz de red virtual.
- Filtrado por protocolos (TCP, HTTP, DNS).
- Análisis de handshakes TCP y tráfico sospechoso.

Objetivo:
Comprender cómo viajan los datos en la red y detectar posibles anomalías.

---

## Pruebas controladas con Metasploit

- Exploración de módulos disponibles.
- Ejecución de pruebas en entorno aislado.
- Análisis del comportamiento del sistema objetivo.

Objetivo:
Comprender el funcionamiento básico de herramientas de explotación en un entorno seguro.

---

## Resultados

- Identificación de puertos abiertos y servicios activos.
- Análisis de tráfico de red y comprensión de protocolos.
- Comprensión básica del proceso de enumeración y explotación.

---

## Conclusión

Este laboratorio permitió adquirir experiencia práctica en análisis de red, escaneo de vulnerabilidades y uso de herramientas fundamentales en ciberseguridad.  
El proyecto refuerza conocimientos aplicables a roles de Analista SOC Junior o posiciones Trainee en Seguridad Informática.

---

## Próximos pasos

- Automatización de escaneos básicos.
- Implementación de laboratorio con múltiples máquinas.
- Análisis de logs y simulación de incidentes.


## Evidencia – Escaneo con Nmap

### Escaneo completo

![Nmap Full Scan](evidencias/nmap_full_scan.png)

### Enumeración de servicios

![Nmap Service Enumeration](evidencias/nmap_service_focus.png)
