# Anisphere — Guía de uso

Anisphere es una app Android para descubrir noticias de anime, explorar catálogos y ver episodios desde fuentes configurables.

> Esta guía es para builds APK. No necesitas el código fuente para usar la app.

---

## Instalar el APK

1. Descarga el `.apk` desde la página de lanzamientos.
2. Ábrelo en el teléfono.
3. Si Android bloquea la instalación, permite **Instalar apps desconocidas** para el navegador / gestor de archivos.
4. Abre **Anisphere** desde el cajón de aplicaciones.

**Requisitos**

- Android **7.0** o superior (recomendado: Android 10+)
- Conexión a Internet
- Permiso de almacenamiento solo si usas descargas cuando estén disponibles  (En desarrollo)

---

## Primer uso

1. Concede el permiso de notificaciones si Android lo pide (recordatorios de estrenos).
2. Abre la pestaña **Módulos** y activa al menos una fuente.
3. Espera unos segundos mientras se comprueban los módulos.
4. Ve a **Explorar** y busca un anime.

---

## Pestañas principales

| Pestaña | Para qué sirve |
| --- | --- |
| **Noticias** | Carrusel de estrenos del día + noticias de anime. Desliza hacia abajo para actualizar. Toca un estreno para más info del calendario, o una noticia para leerla en la app. |
| **Explorar** | Busca anime en los módulos activos. Usa el botón de filtros por género / módulo. Toca una tarjeta para ver detalles. |
| **Favoritos** | Títulos guardados. Puedes buscar y filtrar igual que en Explorar. |
| **Descargas** | Zona de descargas offline (puede estar vacía en betas tempranas mientras se implementa). |
| **Módulos** | Activa o desactiva fuentes del catálogo. Usa solo las que necesites. |

---

## Calendario y notificaciones

1. Desde **Noticias**, abre el calendario / “más info” de los estrenos (o entra en **Calendario**).
2. Cambia de día con las pestañas superiores (lunes–domingo).
3. Toca un título para buscarlo en **Explorar**.
4. Toca el icono de **campana** para programar (o cancelar) una notificación local del estreno. Acepta el permiso si se solicita.

---

## Ver un anime

1. Encuentra el título en **Explorar** (o desde el calendario).
2. Abre **Detalles** para ver la ficha y la lista de episodios.
3. Elige un episodio → **Reproductor**.
4. Si hay varios servidores, cambia hasta que uno reproduzca.
5. Algunos streams usan el reproductor nativo; otros un reproductor web integrado.

Consejos:

- Si falla la reproducción, prueba otro servidor u otro módulo.
- Con mala conexión puede haber buffering o resultados vacíos: actualiza y reintenta.

---

## Favoritos

- Guarda títulos desde la pantalla de detalles (corazón / favorito).
- Abre **Favoritos** cuando quieras continuar.

---

## Solución de problemas

| Problema | Qué probar |
| --- | --- |
| No se instala | Activa orígenes desconocidos; vuelve a descargar el APK; libera espacio. |
| Búsqueda vacía | Activa módulos; comprueba Internet; quita filtros; prueba otra consulta. |
| El vídeo no reproduce | Cambia de servidor; prueba otro episodio; cambia de módulo. |
| Sin notificaciones | Permite notificaciones de Anisphere en Ajustes de Android; vuelve a tocar la campana. |
| La app se cierra | Forzar detención → abrir de nuevo; reinstala el último APK del lanzamiento. |

---

## Privacidad y notas

- Favoritos y notificaciones programadas se guardan en el dispositivo.
- El contenido depende de módulos / sitios de terceros; la disponibilidad varía.
- Las betas pueden cambiar entre versiones: usa siempre el APK más reciente.

---

## Soporte

Si algo falla en un teléfono o versión de Android concreta, indica:

- Modelo del dispositivo  
- Versión de Android  
- Versión del APK (por ejemplo `0.0.1`)  
- Qué estabas haciendo cuando falló  
