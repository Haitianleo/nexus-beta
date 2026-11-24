# Componentes de terceros incluidos con NEXUS

NEXUS se instala junto con estos programas y bibliotecas. Cada uno conserva su licencia. La lista completa, con los textos de licencia, se instala en la carpeta de NEXUS (`THIRD-PARTY-NOTICES.txt` y las carpetas de `tools`).

| Componente | Para qué | Licencia | Código fuente |
|---|---|---|---|
| ooz (nexus-ooz) | Descomprimir, solo para leer, la configuración interna de juegos. Programa aparte | GPL-3.0 | https://github.com/powzix/ooz (commit 05038060). El código exacto usado se instala en `tools\ooz\src` |
| LibreHardwareMonitorLib | Lectura de sensores | MPL-2.0 | https://github.com/LibreHardwareMonitor/LibreHardwareMonitor |
| PresentMon | Medición de FPS. Ejecutable oficial sin modificar | MIT | https://github.com/GameTechDev/PresentMon |
| pythonnet, pywebview, hidapi, pywin32 y otras bibliotecas de Python | Funcionamiento interno | MIT, BSD y similares | Ver `THIRD-PARTY-NOTICES.txt` |

Los componentes con licencia GPL son programas independientes que NEXUS inicia como procesos aparte; NEXUS no incluye su código ni se enlaza con ellos. Tienes derecho a obtener el código fuente de esos componentes en los enlaces indicados.

## No incluidos en el instalador, pero usados

| Qué | Para qué | Licencia | Dónde está |
|---|---|---|---|
| Lista de Are We Anti-Cheat Yet? | Saber qué juegos llevan antitrampas. NEXUS la descarga como mucho una vez por semana | MIT | https://github.com/AreWeAntiCheatYet/AreWeAntiCheatYet |
| NVIDIA NVAPI | Ajustes del controlador de NVIDIA por juego. NEXUS llama a la biblioteca que instala el propio controlador; los identificadores salen de las cabeceras públicas | MIT (cabeceras) | https://github.com/NVIDIA/nvapi |
| Intel Graphics Control Library (IGCL) | Ajustes del controlador de Intel por juego. NEXUS llama a la biblioteca que instala el propio controlador, solo en equipos con gráfica Intel; las estructuras salen de la cabecera pública `igcl_api.h` | Intel Software License Agreement (su aviso completo va en `THIRD-PARTY-NOTICES.txt`) | https://github.com/intel/drivers.gpu.control-library |
| PawnIO | Leer la temperatura del procesador. Se instala aparte; NEXUS no lo instala ni lo modifica, solo lo usa si está presente | GPL-2.0 | https://github.com/namazso/PawnIO |

NVIDIA e Intel son marcas de sus dueños; NEXUS no está afiliado a ellos.

## Cambios

Desde la 0.40.0 el instalador de la beta ya no incluye Sunshine (transmisión de juegos) ni Tailscale (acceso remoto). Esas funciones siguen como «Próximamente». Al actualizar se quitan las copias que dejó una versión anterior.
