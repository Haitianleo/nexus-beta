# Guía de la beta de NEXUS

**[English](GUIDE.md) · Español**

## 1. Instalar

1. Descarga `NEXUS-Setup-….exe` desde **Releases**.
2. Ábrelo. Windows mostrará un aviso azul de **«Windows protegió su PC»** o **«editor desconocido»**. Es normal: el instalador todavía no está firmado. Pulsa **Más información** y luego **Ejecutar de todas formas**.
3. Acepta el permiso de administrador. Hace falta porque NEXUS instala un servicio que lee los sensores del equipo.
4. Al terminar, NEXUS se abre y queda en la bandeja, junto al reloj.

No hace falta instalar nada más.

## 2. Idioma

NEXUS arranca en español o en inglés según el idioma de tu Windows. Puedes cambiarlo cuando quieras desde el menú de la izquierda.

## 3. Primer uso

1. Abre NEXUS y entra en **Game Center**. Aparecen tus juegos de Steam y Epic.
2. Entra en un juego. Con el juego **cerrado**, pulsa **AUTO AI · que lo haga NEXUS** y acepta.
3. Verás una rueda mientras trabaja y después un bloque con lo que hizo. Si no había nada que cambiar, también lo dice.
4. **Juega.** Al cerrar el juego, NEXUS espera cerca de un minuto, comprueba lo aplicado y te avisa con una notificación de Windows si cambió algo.

Con el deslizador eliges hasta dónde llega: **MAX FPS** (busca más FPS), **BALANCED** (hasta los Hz de tu pantalla, sin tirones) o **ULTRA QUALITY** (no baja la calidad). En **Objetivo de FPS** también puedes escribir tu propio número para ese juego, por ejemplo 90.

## 4. Guía de ajustes

Mide lo que cuesta cada ajuste en tu PC, uno a uno, y te deja elegir.

1. En la ficha del juego, busca **Guía de ajustes** y pulsa **Empezar la guía**.
2. Juega una partida normal y cierra el juego. Esa es la referencia.
3. NEXUS baja un ajuste un nivel. Juega otra partida y cierra el juego: NEXUS lo mide, devuelve el ajuste a como estaba y pasa al siguiente. Un aviso de Windows te dice cada resultado.
4. Al terminar, marca los ajustes que te compensen y pulsa **Aplicar los marcados**. **Restaurar todo** lo deshace.

Consejos: juega en zonas parecidas en cada partida y no cambies los gráficos en el menú del juego mientras dure la guía. AUTO AI espera a que termine. **Detener guía** la para cuando quieras; lo que estaba en prueba vuelve a como estaba.

## 5. Deshacer

En la ficha del juego, **Restaurar todo** devuelve los ajustes del juego, del controlador NVIDIA y de Windows a como estaban, y detiene AUTO AI en ese juego.

## 6. Juegos con antitrampas

En juegos donde NEXUS detecta un antitrampas (Easy Anti-Cheat, BattlEye, NCGuard y otros), **solo** cambia el controlador y Windows y no toca los archivos del juego.

En la vista completa (**Vista sencilla · ver todo** en el menú) cada uno de esos juegos tiene dos permisos separados, los dos apagados:

1. **Su archivo de ajustes**: el mismo que escribe el menú de gráficos del juego.
2. **Engine.ini**: puede cambiar cosas que el menú no deja, como la niebla. En un juego online eso puede verse como trampa. NEXUS avisa antes de que lo permitas. Al retirarlo, Engine.ini vuelve a como estaba.

**En esta beta, deja los dos apagados en juegos online.** Si los activas, el riesgo para tu cuenta es solo tuyo.

## 7. Qué esperar

- Los estados de un juego van de **DETECTADO** a **OPTIMIZADO**. «Aplicado» no es «optimizado»: NEXUS solo dice «optimizado» cuando el juego aceptó el cambio y los FPS medidos mejoraron.
- Si una partida es corta o los FPS varían mucho, NEXUS no decide: sigue midiendo en la siguiente.
- NEXUS graba FPS, uso y temperaturas mientras juegas. Esos datos se quedan en tu PC.

## 8. Desinstalar

**Configuración de Windows → Aplicaciones → NEXUS → Desinstalar.** Antes, usa **Restaurar todo** en cada juego donde pulsaste AUTO AI.

## 9. Si algo falla

| Qué pasa | Qué probar |
|---|---|
| No aparece un juego | Tiene que estar instalado por Steam o Epic. Cierra y abre NEXUS. |
| AUTO AI dice que no puede cambiar nada | Ese juego guarda sus ajustes de una forma que NEXUS no puede escribir. Te indica qué cambiar en el menú del juego. |
| No llega la notificación | Mira si Windows tiene «No molestar» activado (la campana junto al reloj). En la ficha del juego hay un botón **Probar aviso de Windows**. |
| El juego va peor | **Restaurar todo** y cuéntamelo en el [formulario de opinión](https://forms.gle/orRMRurHcRCdbiBRA) (sin cuenta) o en Issues. |
