# Guía de la beta de NEXUS

## 1. Instalar

1. Descarga `NEXUS-Setup-….exe` desde **Releases**.
2. Ábrelo. Windows mostrará un aviso azul de **«Windows protegió su PC»** o **«editor desconocido»**. Es normal: el instalador todavía no está firmado. Pulsa **Más información** y luego **Ejecutar de todas formas**.
3. Acepta el permiso de administrador. Hace falta porque NEXUS instala un servicio que lee los sensores del equipo.
4. Al terminar, NEXUS se abre y queda en la bandeja, junto al reloj.

No hace falta instalar nada más.

## 2. Primer uso

1. Abre NEXUS y entra en **Game Center**. Aparecen tus juegos de Steam y Epic.
2. Entra en un juego. Con el juego **cerrado**, pulsa **AUTO AI · que lo haga NEXUS** y acepta.
3. Verás una rueda mientras trabaja y después un bloque con lo que hizo. Si no había nada que cambiar, también lo dice.
4. **Juega.** Al cerrar el juego, NEXUS espera cerca de un minuto, comprueba lo aplicado y te avisa con una notificación de Windows si cambió algo.

Con el deslizador eliges hasta dónde llega: **MAX FPS** (busca más FPS), **BALANCED** (hasta los Hz de tu pantalla, sin tirones) o **ULTRA QUALITY** (no baja la calidad).

## 3. Deshacer

En la ficha del juego, **Restaurar todo** devuelve los ajustes del juego, del controlador NVIDIA y de Windows a como estaban, y detiene AUTO AI en ese juego.

## 4. Juegos con antitrampas

En juegos con antitrampas (por ejemplo Easy Anti-Cheat), NEXUS **solo** cambia el controlador y Windows y no toca los archivos del juego. Existe un permiso para que también cambie el archivo de ajustes de ese juego.

**En esta beta, no actives ese permiso.** No está probado lo suficiente, y la decisión de tocar un juego con antitrampas tiene riesgos para tu cuenta que son solo tuyos.

## 5. Qué esperar

- Los estados de un juego van de **DETECTADO** a **OPTIMIZADO**. «Aplicado» no es «optimizado»: NEXUS solo dice «optimizado» cuando el juego aceptó el cambio y los FPS medidos mejoraron.
- Si una partida es corta o los FPS varían mucho, NEXUS no decide: sigue midiendo en la siguiente.
- NEXUS graba FPS, uso y temperaturas mientras juegas. Esos datos se quedan en tu PC.

## 6. Desinstalar

**Configuración de Windows → Aplicaciones → NEXUS → Desinstalar.** Antes, usa **Restaurar todo** en cada juego donde pulsaste AUTO AI.

## 7. Si algo falla

| Qué pasa | Qué probar |
|---|---|
| No aparece un juego | Tiene que estar instalado por Steam o Epic. Cierra y abre NEXUS. |
| AUTO AI dice que no puede cambiar nada | Ese juego guarda sus ajustes de una forma que NEXUS no puede escribir. Te indica qué cambiar en el menú del juego. |
| No llega la notificación | Mira si Windows tiene «No molestar» activado (la campana junto al reloj). En la ficha del juego hay un botón **Probar aviso de Windows**. |
| El juego va peor | **Restaurar todo** y cuéntalo en Issues. |
