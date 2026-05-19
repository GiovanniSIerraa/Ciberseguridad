# Lab 1. Practica de defensa activa

## Finalidad del Laboratorio

La finalidad de esta práctica es implementar una estrategia de Defensa en Profundidad mediante la mitigación proactiva de la superficie de exposición de un servidor. Los servidores de producción no pueden actualizarse de manera masiva y descuidada, ya que parches mal testeados podrían quebrar dependencias críticas y tumbar servicios esenciales. 

Por lo tanto, este laboratorio tiene como propósito técnico aislar y automatizar exclusivamente el canal de parches críticos de seguridad, logrando que el sistema operativo se proteja de manera autónoma ante exploits públicos.

---

## Herramientas Utilizadas
Para el desarrollo de esta simulación defensiva se emplearon los siguientes recursos tecnológicos:
* **Sistema Operativo Víctima:** Ubuntu Server (entorno desactualizado simulando un servidor corporativo en producción).
* **Sistema Operativo Atacante:** Kali Linux.
* **Unattended-Upgrades:** Paquete y servicio de Linux diseñado para automatizar la instalación de software y parches de seguridad de manera desatendida.

---

## Análisis de Vulnerabilidades (Fase de investigacion)

Se realizó una auditoría basada en las bases de datos del **NVD (National Vulnerability Database - NIST)** para comprender el impacto real de las vulnerabilidades presentes en versiones desactualizadas de OpenSSH.

1. **Vulnerabilidades Críticas Analizadas:**
   * **CVE-2023-38408 (Base Score: 9.8 CRITICAL):** Fallo en la característica PKCS#11 de `ssh-agent` que permite la ejecución remota de código (RCE) si un agente es reenviado a un sistema controlado por un atacante.
   * **CVE-2020-15778 (Base Score: 7.4 / 7.8 HIGH):** Vulnerabilidad en el comando `scp` que permite la inyección y ejecución de comandos maliciosos a través de la transferencia de archivos.
   * **CVE-2019-6110 (Base Score: 6.8 MEDIUM):** Vulnerabilidad de manipulación de salida donde un servidor malicioso (Man-in-the-Middle) puede usar códigos de control ANSI para ocultar archivos adicionales transferidos.

---

## Desarrollo del Laboratorio y Evidencias

A continuación, se detallan los pasos técnicos ejecutados en la consola del servidor Ubuntu para verificar el estado de los paquetes y configurar la automatización de las defensas.




