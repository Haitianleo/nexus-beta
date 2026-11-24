# Guía de la beta de NEXUS

**[English](GUIDE.md) · Español**

## 1. Instalar

1. Descarga `NEXUS-Setup-….exe` desde **Releases**.
2. Ábrelo. Windows mostrará un aviso azul de **«Windows protegió su PC»** o **«editor desconocido»**. Es normal: el instalador todavía no está firmado. Pulsa **Más información** y luego **Ejecutar de todas formas**. (Si Windows tiene activado el *Control inteligente de aplicaciones*, bloquea las aplicaciones sin firmar, también NEXUS.)
3. Acepta el permiso de administrador. Hace falta porque NEXUS instala un servicio que lee los sensores del equipo.
4. Al terminar, NEXUS se abre y queda en la bandeja, junto al reloj.

No hace falta instalar nada más. Si ya tienes la 0.39, no tienes que descargar nada: NEXUS te ofrece la versión nueva ella sola, con **Actualizar ahora**.

La primera vez que se abre, un aviso explica las estadísticas anónimas. Vienen encendidas, y puedes apagarlas ahí mismo o después en **Conexión y seguridad → Privacidad**.

## 2. Idioma

NEXUS arranca en español o en inglés según el idioma de tu Windows. Puedes cambiarlo cuando quieras desde el menú de la izquierda.

## 3. Primer uso

1. Abre NEXUS y entra en **Game Center**. Aparecen tus juegos de Steam, Epic Games, Xbox (app de Xbox, PC Game Pass y Microsoft Store), GOG, Ubisoft Connect, EA app, Amazon Games y Riot Games. Cada tarjeta dice de qué lanzador es, y puedes filtrar la lista por lanzador.
2. ¿Un juego de otro sitio (Battle.net, un emulador, un juego suelto)? Pulsa **Añadir un juego** y elige su `.exe`.
3. Entra en un juego. Con el juego **cerrado**, pulsa **AUTO AI · que lo haga NEXUS** y acepta.
4. Verás una rueda mientras trabaja y después un bloque con lo que hizo. Si no había nada que cambiar, también lo dice.
5. **Juega.** Al cerrar el juego, NEXUS espera cerca de un minuto y comprueba lo aplicado. El resultado está en la ficha del juego, y cuando un cambio sube de verdad tus FPS (medido) te avisa con una notificación de Windows.

Con el deslizador eliges hasta dónde llega: **MAX FPS** (busca más FPS), **BALANCED** (hasta los Hz de tu pantalla, sin tirones) o **ULTRA QUALITY** (no baja la calidad). En **Objetivo de FPS** también puedes escribir tu propio número para ese juego, por ejemplo 90.

Después de tu primera partida medida, NEXUS te pregunta, una sola vez, si esta versión te funciona mejor, igual o peor que la anterior. Puedes cerrarla sin responder.

## 4. Guía de ajustes

Mide lo que cuesta cada ajuste en tu PC, uno a uno, y te deja elegir.

1. En la ficha del juego, busca **Guía de ajustes** y pulsa **Empezar la guía**.
2. Juega una partida normal y cierra el juego. Esa es la referencia.
3. NEXUS baja un ajuste un nivel. Juega otra partida y cierra el juego: NEXUS lo mide, devuelve el ajuste a como estaba y pasa al siguiente. Cada resultado sale en la tabla de la guía.
4. Después de los ajustes del propio juego prueba también algunas opciones del controlador de la gráfica y de Windows (por ejemplo, las optimizaciones de Windows para juegos en ventana). No tocan los archivos del juego, así que la guía puede probarlas también en juegos con antitrampas.
5. Al terminar, marca los ajustes que te compensen y pulsa **Aplicar los marcados**. **Restaurar todo** lo deshace.

Consejos: juega en zonas parecidas en cada partida y no cambies los gráficos en el menú del juego mientras dure la guía. AUTO AI espera a que termine. **Detener guía** la para cuando quieras; lo que estaba en prueba vuelve a como estaba.

## 5. Deshacer

En la ficha del juego, **Restaurar todo** devuelve los ajustes del juego, del controlador de la gráfica y de Windows a como estaban, y detiene AUTO AI en ese juego.

## 6. Juegos con antitrampas

En juegos donde NEXUS sabe que hay un antitrampas (Easy Anti-Cheat, BattlEye, Riot Vanguard, NCGuard y otros), **solo** cambia el controlador de la gráfica y Windows y no toca los archivos del juego.

Al pulsar **AUTO AI · que lo haga NEXUS** en uno de esos juegos, la ventana te lo dice y enseña **Ampliar permisos (opcional, bajo tu responsabilidad)** con dos casillas, las dos sin marcar:

1. **El archivo de ajustes del juego**: el mismo que escribe el menú de gráficos del juego.
2. **Engine.ini**: puede cambiar cosas que el menú no deja, como la niebla. En un juego online eso puede verse como trampa. Si la marcas, NEXUS enseña un aviso y vuelve a preguntar (**Entiendo el riesgo**).

**En esta beta, deja las dos sin marcar en juegos online.** Si las activas, el riesgo para tu cuenta es solo tuyo. **Quitar permisos**, en la ficha del juego, los retira y devuelve a como estaba lo que se cambió con ellos.

Si NEXUS se entera de que un juego usa antitrampas cuando ya le había cambiado algo, no deshace nada sola: te avisa y no cambia nada más en los archivos del juego sin tu permiso.

## 7. Tarjetas gráficas

- **NVIDIA:** soporte completo.
- **Intel:** temperatura, ventilador y ajustes del controlador, nuevo y sin probar todavía en gráficas Intel reales.
- **AMD:** temperatura, ventilador y consumo; los ajustes del controlador llegan en una próxima versión.

Con cualquier tarjeta NEXUS puede cambiar los ajustes del propio juego y las opciones gráficas de Windows para ese juego, y mide tus FPS igual.

**¿Tienes una gráfica AMD o Intel?** Ese soporte es nuevo y no tengo ninguna tarjeta así para probarlo. Ayúdame mandando el diagnóstico: **Conexión y seguridad → Ayuda → Exportar diagnóstico** guarda un `.zip` (sin tu nombre de usuario, sin el nombre del PC y sin rutas completas; NEXUS nunca lo envía). Adjúntalo a un aviso en [Issues](../../issues) y di qué tarjeta tienes. **Los Issues de GitHub son públicos: al adjuntar ahí el `.zip` lo estás publicando.** El archivo nombra tus juegos, así que míralo antes.

## 8. Qué esperar

- Los estados de un juego van de **DETECTADO** a **OPTIMIZADO**. «Aplicado» no es «optimizado»: NEXUS solo dice «optimizado» cuando el juego aceptó el cambio y los FPS medidos mejoraron.
- Si una partida es corta o los FPS varían mucho, NEXUS no decide: sigue midiendo en la siguiente.
- NEXUS graba FPS, uso y temperaturas mientras juegas. Esos datos se quedan en tu PC.

## 9. Desinstalar

**Configuración de Windows → Aplicaciones → NEXUS → Desinstalar.** Antes, usa **Restaurar todo** en cada juego donde pulsaste AUTO AI.

## 10. Si algo falla

| Qué pasa | Qué probar |
|---|---|
| No aparece un juego | Pulsa **Añadir un juego** en Game Center y elige el `.exe` del juego. Si es de uno de los lanzadores del apartado 3, cuéntamelo: varios son nuevos en la 0.40 y todavía no se han probado con juegos reales. |
| AUTO AI dice que no puede cambiar nada | Ese juego guarda sus ajustes de una forma que NEXUS no puede escribir. Te indica qué cambiar en el menú del juego. |
| No llega la notificación | Mira si Windows tiene «No molestar» activado (la campana junto al reloj) y si ese tipo de aviso está encendido en **Conexión y seguridad → Avisos de Windows**. |
| El juego va peor | **Restaurar todo** y cuéntamelo en el [formulario de opinión](https://forms.gle/orRMRurHcRCdbiBRA) (sin cuenta) o en Issues. |
| Algo va raro con una gráfica AMD o Intel | **Restaurar todo** deshace lo que cambió NEXUS. Después mándame **Exportar diagnóstico** (apartado 7). |
