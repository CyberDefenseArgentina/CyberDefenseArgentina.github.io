En octubre de 2025, se identificó una vulnerabilidad crítica en el componente Windows Server Update Services (WSUS) de Microsoft — la deserialización de datos no confiables que permite a un atacante sin privilegios ejecutar código remoto con privilegios de SYSTEM. 

Con una puntuación CVSS de 9.8, representa un riesgo significativo para entornos donde WSUS está habilitado y expuesto. 
nvd.nist.gov

El escenario de riesgo es especialmente crítico porque WSUS juega un rol central en la infraestructura de parcheo de Microsoft: un servidor comprometido puede actuar como punto de pivote — puede permitir movimiento lateral, exfiltración de datos o implantación de carga maliciosa a gran escala. 

Para mitigar este riesgo, Microsoft lanzó un parche de urgencia fuera de ciclo (out-of-band) tras primeras evidencias de explotación en el mundo real. 

Mientras tanto, se recomienda como mitigación temporal deshabilitar el rol de WSUS o bloquear los puertos TCP 8530/8531 en el firewall de host si el parche no puede aplicarse de inmediato. 

Para ejecutivos de seguridad, el mensaje clave es claro: no basta con depender del parche semanal de rutina. Una mala configuración (por ejemplo, un WSUS expuesto a Internet) combinada con una vulnerabilidad grave convierte una plataforma de parcheo en una puerta trasera para adversarios.


Visita la plataforma [OpenCVE](https://app.opencve.io/cve/CVE-2025-59287)) para conocer más.

![fallo-critico-en-servidores-Windows-WSUS](/assets/img/G4cBetYXgAEBrVf.jpg)
