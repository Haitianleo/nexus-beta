# Componentes de terceros incluidos con NEXUS

NEXUS se instala junto con estos programas y bibliotecas. Cada uno conserva su licencia. La lista completa, con los textos de licencia, se instala en la carpeta de NEXUS (`THIRD-PARTY-NOTICES.txt` y las carpetas de `tools`).

| Componente | Para qué | Licencia | Código fuente |
|---|---|---|---|
| Sunshine | Transmisión de juegos. Programa aparte, ejecutable oficial sin modificar | GPL-3.0 | https://github.com/LizardByte/Sunshine/tree/v2026.914.233613 |
| ooz (nexus-ooz) | Descomprimir, solo para leer, la configuración interna de juegos. Programa aparte | GPL-3.0 | https://github.com/powzix/ooz (commit 05038060). El código exacto usado se instala en `tools\ooz\src` |
| Tailscale (tsnet) | Acceso remoto privado. Programa aparte | BSD-3-Clause | https://github.com/tailscale/tailscale (v1.104.1) |
| LibreHardwareMonitorLib | Lectura de sensores | MPL-2.0 | https://github.com/LibreHardwareMonitor/LibreHardwareMonitor |
| PresentMon | Medición de FPS. Ejecutable oficial sin modificar | MIT | https://github.com/GameTechDev/PresentMon |
| pythonnet, pywebview, hidapi, pywin32 y otras bibliotecas de Python | Funcionamiento interno | MIT, BSD y similares | Ver `THIRD-PARTY-NOTICES.txt` |

Los componentes con licencia GPL son programas independientes que NEXUS inicia como procesos aparte; NEXUS no incluye su código ni se enlaza con ellos. Tienes derecho a obtener el código fuente de esos componentes en los enlaces indicados.
