# NEXUS AI Ecosystem — beta cerrada

NEXUS es un programa para PC con Windows que ajusta los gráficos de tus juegos **solo y midiendo**: prueba un cambio, mira cómo cambian tus FPS mientras juegas y se queda únicamente con lo que de verdad ayuda en tu equipo.

> **Esto es una beta.** Está probada en pocos equipos. Puede fallar. Todo lo que cambia se puede deshacer con un botón.

## Qué hace

- **AUTO AI:** pulsas un botón en un juego y NEXUS investiga sus archivos, aplica lo que puede cambiar con seguridad y, después de cada partida, comprueba el resultado y sigue sola.
- **Mide de verdad:** no promete FPS. Compara lo que midió antes y después y te lo dice, también cuando un cambio no sirvió.
- **Tres caminos:** los ajustes del propio juego, el controlador NVIDIA y la configuración gráfica de Windows.
- **Restaurar todo:** un botón devuelve cada ajuste a como estaba.
- **Aviso de Windows** cuando cambia algo después de una partida.
- Además: panel del PC en tiempo real (temperaturas, uso, FPS), biblioteca de juegos de Steam y Epic, y control de energía.

## Qué no hace

- No modifica ejecutables ni paquetes de datos de los juegos.
- No toca, desactiva ni evita sistemas antitrampas.
- No descifra archivos protegidos: si un juego cifra sus ajustes, NEXUS lo dice y usa otros caminos.
- No inventa números: lo que no puede medir lo muestra como «—».

## Requisitos

- Windows 11 (64 bits).
- Tarjeta gráfica NVIDIA para aprovecharlo todo. Con AMD o Intel funcionan el panel y la parte de archivos del juego, pero está menos probado.
- Juegos de Steam o Epic. La optimización automática está pensada para juegos hechos con Unreal Engine; con otros motores hace menos.

## Descargar

Ve a **[Releases](../../releases)** y descarga `NEXUS-Setup-….exe`.

Lee antes la **[guía de instalación](GUIA.md)**: explica el aviso de «editor desconocido» de Windows y cómo deshacer todo.

## Próximamente

- **App para el teléfono (iPhone y Android):** ver el estado del PC, lanzar AUTO AI y apagar o encender el equipo desde el móvil. Ya funciona en pruebas internas; todavía no hay fecha para publicarla.
- **Inglés y español**, con el idioma según tu PC.
- **Instalador firmado**, para que Windows no muestre el aviso de «editor desconocido».

No hay fechas prometidas: se publicará cuando esté probado.

## Probado hasta ahora

| Juego | Resultado |
|---|---|
| Phantom Blade Zero | Trazado de rayos apagado desde fuera del juego: de 67 a 81 FPS de media (RTX 3080, 4K), medido y confirmado por el propio juego |
| SILENT HILL: Townfall | Ajustes aplicados; pendiente de medición |
| Halloween: The Game | Controlador y Windows aplicados; pendiente de medición |

Son resultados de un solo equipo. En el tuyo pueden ser distintos: para eso es la beta.

## Cuéntame cómo te fue

Abre un aviso en **[Issues](../../issues)** con:

1. Tu tarjeta gráfica y procesador.
2. El juego.
3. Qué te mostró NEXUS después de jugar (una captura del bloque «AUTO AI · resultado» sirve).
4. Qué esperabas y qué pasó.

## Apoyar el proyecto

NEXUS es gratis durante la beta y lo hace una sola persona. Si te resulta útil, puedes apoyarlo en **[Ko-fi](https://ko-fi.com/12thmonth)**.

Las aportaciones van a dos cosas concretas:

- **La app del teléfono en la App Store.** Publicar ahí exige una cuenta de desarrollador de Apple, que es de pago cada año. Es la app para ver tu PC, lanzar AUTO AI y jugar a tus juegos desde el móvil, también fuera de casa.
- **Firmar el instalador de Windows**, para que deje de salir el aviso de «editor desconocido». El certificado también es de pago.

Apoyar no da acceso a nada distinto ni compra una fecha: la beta es la misma para todos.

## Licencia

NEXUS es software propietario. Esta beta se ofrece solo para probarla: consulta **[LICENSE.md](LICENSE.md)**. Incluye componentes de terceros con sus propias licencias: **[TERCEROS.md](TERCEROS.md)**.

---

**English, in short:** NEXUS is a Windows tool that tunes your games' graphics by testing one change at a time and measuring your real FPS while you play, keeping only what helps on your PC. Closed beta, tested on few machines; everything it changes can be undone with one button. Download the installer from Releases and read GUIA.md (Spanish) first. Proprietary software, for testing only: see LICENSE.md.
