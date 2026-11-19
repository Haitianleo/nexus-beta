# NEXUS AI Ecosystem — closed beta

**English** · [Español ↓](#español)

NEXUS is a Windows program that tunes your games' graphics **on its own, by measuring**: it tries one change, watches how your FPS actually move while you play, and keeps only what really helps on your PC.

> **This is a beta.** It has been tested on very few machines. It may fail. Everything it changes can be undone with one button.

The app is available in **English and Spanish**. It picks the language of your Windows the first time, and you can switch it at any moment from the menu.

## What it does

- **AUTO AI:** press one button on a game and NEXUS studies its files, applies what it can safely change and, after each session, checks the result and carries on by itself.
- **It measures for real:** no promised FPS. It compares what it measured before and after and tells you, also when a change did not help.
- **Three routes:** the game's own settings, the NVIDIA driver and the Windows graphics settings.
- **Restore everything:** one button puts every setting back the way it was.
- **A Windows notification** when something changes after a session.
- Also: live PC dashboard (temperatures, load, FPS), your Steam and Epic library, and power controls.

## What it does not do

- It does not modify game executables or data packages.
- It does not touch, disable or bypass anti-cheat systems.
- It does not decrypt protected files: if a game encrypts its settings, NEXUS says so and uses other routes.
- It does not make numbers up: what it cannot measure is shown as "—".

## Requirements

- Windows 11 (64-bit).
- An NVIDIA graphics card to get the most out of it. With AMD or Intel the dashboard and the game-file route work, but they are less tested.
- Games from Steam or Epic. Automatic optimisation is built for Unreal Engine games; with other engines it does less.

## Download

Go to **[Releases](../../releases)** and download `NEXUS-Setup-….exe`.

Read the **[installation guide](GUIDE.md)** first: it explains the Windows "unknown publisher" warning and how to undo everything.

## Coming soon

- **Phone app (iPhone and Android):** see your PC, launch AUTO AI and turn the PC on or off from your phone. It already works in internal testing; there is no release date yet.
- **Signed installer**, so Windows stops showing the "unknown publisher" warning.

No dates are promised: things are released when they have been tested.

## Tested so far

| Game | Result |
|---|---|
| Phantom Blade Zero | Ray tracing turned off from outside the game: from 67 to 81 FPS on average (RTX 3080, 4K), measured and confirmed by the game itself |
| SILENT HILL: Townfall | Settings applied; measurement pending |
| Halloween: The Game | Driver and Windows applied; measurement pending |

These are results from a single PC. Yours may differ: that is what the beta is for.

## Tell me how it went

Use the **Feedback & support** button inside NEXUS, or open an entry in **[Issues](../../issues)** with:

1. Your graphics card and processor.
2. The game.
3. What NEXUS showed after you played (a screenshot of the "AUTO AI · result" block is enough).
4. What you expected and what happened.

## Support the project

NEXUS is free during the beta and is made by one person. If you find it useful, you can support it on **[Ko-fi](https://ko-fi.com/12thmonth)**.

Contributions go to two specific things:

- **The phone app on the App Store.** Publishing there requires a paid Apple developer account every year. It is the app to see your PC, launch AUTO AI and play your games from your phone, also away from home.
- **Signing the Windows installer**, so the "unknown publisher" warning goes away. The certificate is also paid.

Supporting does not unlock anything different and does not buy a date: the beta is the same for everyone.

## Licence

NEXUS is proprietary software. This beta is offered for testing only: see **[LICENSE.md](LICENSE.md)**. It ships with third-party components under their own licences: **[TERCEROS.md](TERCEROS.md)**.

---

# Español

**NEXUS AI Ecosystem — beta cerrada** · [English ↑](#nexus-ai-ecosystem--closed-beta)

NEXUS es un programa para PC con Windows que ajusta los gráficos de tus juegos **solo y midiendo**: prueba un cambio, mira cómo cambian tus FPS mientras juegas y se queda únicamente con lo que de verdad ayuda en tu equipo.

> **Esto es una beta.** Está probada en pocos equipos. Puede fallar. Todo lo que cambia se puede deshacer con un botón.

La aplicación está en **español e inglés**. La primera vez usa el idioma de tu Windows, y puedes cambiarlo cuando quieras desde el menú.

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

Usa el botón **Opinar y apoyar** dentro de NEXUS, o abre un aviso en **[Issues](../../issues)** con:

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
