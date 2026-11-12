<div align="center">

# 👋 Hola, soy Byron

**Hago apps para Android que son gratis de verdad.**
Sin cuentas · sin anuncios · sin suscripciones · sin internet

![Sin internet](https://img.shields.io/badge/permiso%20de%20internet-ninguno-2ea44f)
![Sin anuncios](https://img.shields.io/badge/anuncios-ninguno-2ea44f)
![Hecho con ayuda de Claude](https://img.shields.io/badge/hecho%20con-ayuda%20de%20Claude-8957e5)
![Estado](https://img.shields.io/badge/estado-primeras%20versiones-f0883e)

[Mis apps](#-mis-apps) · [Descargar](#%EF%B8%8F-descargar-e-instalar) · [Cómo las hago](#-cómo-las-hago-con-claude) · [Privacidad](#-privacidad) · [Fallos o ideas](#-si-algo-falla-o-tienes-una-idea)

</div>

---

## 🙋 Quién soy
Soy Byron y estoy aprendiendo a hacer apps para el móvil con ayuda de Claude. Empecé porque quería apps sencillas que funcionaran sin pedirme una cuenta, sin llenarme de anuncios y sin gastar datos. Como no las encontraba, las hago yo.

Todavía **no soy un experto**. Lo que ves aquí son mis primeras versiones: las pruebo en mi móvil y las voy mejorando poco a poco.

## 📱 Mis apps

<table>
<tr>
<td width="50%" valign="top">

### 💬 Cuéntame
Un juego de preguntas para **conocer mejor a quien tienes delante**: tu pareja, tus amigos, tu familia, tus compañeros o gente que acabas de conocer.

- Mazos listos para jugar y varios modos: por niveles, tarjetas, verdad o reto, ¿quién es más probable?, yo nunca y ¿qué prefieres?
- Puedes crear tus propios mazos, pegarlos desde una lista y compartirlos con otros móviles.
- Incluye un **prototipo de IA opcional** para crear mazos, **apagado de fábrica**. Necesita un modelo aparte y funciona dentro de tu móvil.

</td>
<td width="50%" valign="top">

### 🍽️ RecetasGain
Una app de recetas para quien quiere **comer más y mejor**: te propone comidas según los ingredientes que tienes en casa.

- Puedes crear ingredientes nuevos **leyendo la tabla nutricional de una foto**. La foto se lee en tu móvil y no se guarda.
- Integración opcional con Health Connect.
- Sin suscripciones y sin cuentas.

</td>
</tr>
</table>

> 📸 Pronto añadiré capturas de pantalla de cada app.

## ⬇️ Descargar e instalar
Las descargas estarán en la sección **[Releases](../../releases)** de este repositorio: un archivo `.apk` por app, con su código de verificación y las notas de la versión.

> 🚧 Estoy terminando las primeras versiones firmadas. Cuando estén listas, aparecerán ahí.

**Cómo instalar una APK (fuera de Google Play):**
1. Descarga la APK desde el móvil, desde la *release* de la app.
2. Ábrela. Android te pedirá **permitir instalar desde esa aplicación** (el navegador o el gestor de archivos). Acéptalo solo para esta instalación.
3. Puede salir un aviso de **Play Protect** porque la app no viene de Google Play. Si la has descargado desde aquí, puedes pulsar *Instalar de todos modos*.
4. Para actualizar, instala la versión nueva encima: se conservan tus datos.
5. Para desinstalarla, como cualquier otra app.

### ✅ Comprueba que la APK es la mía
Cada *release* trae el **SHA-256** del archivo. Compáralo con el de tu descarga:

```powershell
Get-FileHash .\archivo.apk -Algorithm SHA256   # Windows (PowerShell)
```
```bash
sha256sum archivo.apk                          # Linux o macOS
```

Si los códigos no coinciden, no la instales y vuelve a descargarla desde aquí.

Además, todas mis apps se firman con **la misma clave**. Si sabes usar `apksigner`, puedes comprobar la firma con `apksigner verify --print-certs archivo.apk` y compararla con esta huella:

**SHA-256 de mi certificado de firma:**

```
44:0B:06:39:82:7B:98:CE:62:27:2B:55:7D:E0:BA:60:45:39:AB:CE:A1:65:DF:26:1F:00:62:95:68:AC:32:D6
```

`apksigner` lo escribe en minúsculas y sin los dos puntos, así que lo verás como:

```
440b0639827b98ce62272b557de0ba604539abcea165df261f00629568ac32d6
```

## 🤖 Cómo las hago con Claude
Mis apps **están programadas con ayuda de Claude**, un asistente de Anthropic. Prefiero decirlo claro desde el principio.

| Lo que hago yo | Lo que hace Claude |
|---|---|
| Decido qué hace cada app y para quién es | Escribe el código de la app |
| Elijo cómo debe verse y sentirse | Escribe los textos de los mazos de Cuéntame y las pruebas |
| Pruebo cada versión en mi móvil y le digo lo que falla | Propone cambios y arregla los fallos que le señalo |
| Decido qué se publica y me hago responsable | Me explica lo que no entiendo |

**Qué puedes esperar:**
- Son **primeras versiones**. Puede haber fallos que aún no he visto, sobre todo en móviles distintos al mío.
- Las pruebo en un móvil concreto y en un emulador, no en cientos de dispositivos.
- No pretendo que sean perfectas: pretendo que sean sencillas, honestas y gratis.
- **El código fuente no está publicado** por ahora. Lo que publico aquí son las apps ya compiladas.

## 🔒 Privacidad
Mis apps **no piden permiso de internet**. No recogen datos, no los envían a ningún sitio y no tienen cuentas. Lo que creas se queda en tu móvil.

Las apps usan librerías de terceros (por ejemplo, la lectura de texto de fotos de RecetasGain). Sus licencias se incluyen con cada app.

## 🐛 Si algo falla o tienes una idea
Abre una **[Issue](../../issues/new)** en este repositorio y cuéntame:
- qué app y qué versión usas,
- qué móvil tienes y qué versión de Android,
- qué estabas haciendo cuando falló.

Cualquier idea o crítica amable me ayuda a mejorar.

## 🛠️ Lo que estoy haciendo ahora
- Terminar las primeras versiones firmadas de Cuéntame y RecetasGain.
- Probar la lectura de etiquetas de RecetasGain con productos reales.
- Probar, en Cuéntame, un modelo de IA pequeño que escriba mejores preguntas (sigue siendo un experimento).
- Añadir más mazos.

---

<div align="center">

Ideado y dirigido por **Byron** · Programado con ayuda de Claude (Anthropic)

</div>
