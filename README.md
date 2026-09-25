<div align="center">

# 🎧 FridaMusic Desktop

**FridaMusic para Windows, macOS y Linux — desarrollado por Frida Labs**

[![Desktop Release](https://img.shields.io/github/v/release/jagrdev-MX/FridaMusic-Desktop-Releases?style=for-the-badge&label=Desktop)](https://github.com/jagrdev-MX/FridaMusic-Desktop-Releases/releases)
[![GPL-3.0](https://img.shields.io/badge/License-GPL--3.0-blue.svg?style=for-the-badge)](#licencia-y-créditos)
[![Electron](https://img.shields.io/badge/Electron-42-47848F?style=for-the-badge&logo=electron&logoColor=white)](#tecnología)
[![FridaMusic Android](https://img.shields.io/badge/FridaMusic-Android-3DDC84?style=for-the-badge&logo=android&logoColor=white)](https://github.com/jagrdev-MX/FridaMusic_OF)

[⬇️ Descargar Desktop](https://github.com/jagrdev-MX/FridaMusic-Desktop-Releases/releases) ·
[📱 FridaMusic Android](https://github.com/jagrdev-MX/FridaMusic_OF) ·
[▶ Google Play](https://play.google.com/store/apps/details?id=com.jagr.fridamusic) ·
[🌐 Sitio oficial](https://frida-music-of.vercel.app/)

</div>

---

## Qué es FridaMusic Desktop

**FridaMusic Desktop** es la edición de escritorio del ecosistema FridaMusic. Está construida como una aplicación multiplataforma con **Electron** y una capa web moderna, adaptada a pantallas grandes, integración con el sistema operativo, reproducción continua, biblioteca, exploración, playlists, cola, letras, personalización visual y actualización desde la propia aplicación.

Desktop comparte la identidad, objetivos de producto y parte de los flujos de experiencia de **FridaMusic para Android**, pero **no es un port 1:1 del código Kotlin ni del backend móvil**. La edición de escritorio utiliza una arquitectura propia basada principalmente en **TypeScript, JavaScript, HTML, CSS, SolidJS y Electron**, reutilizando e integrando servicios y componentes compatibles donde resulta apropiado.

> Como estimación interna de alcance —no como porcentaje de líneas de código copiadas— alrededor del **80 % de los conceptos de servicio, flujos de datos e integración de la experiencia FridaMusic** pudieron reaprovecharse o adaptarse para Desktop. La capa de presentación, integración con el sistema operativo, empaquetado y actualización se implementa específicamente para escritorio.

> El repositorio de desarrollo de Desktop se mantiene separado. Este repositorio público está dedicado a **releases oficiales, instaladores, metadatos del actualizador y snapshots de código fuente correspondientes a cada versión publicada**.

## 📸 Vista rápida

<table>
  <tr>
    <td align="center" width="50%">
      <strong>Explorar y descubrir</strong><br />
      <img src="assets/screenshots/Screenshot%202026-09-23%20163006.png" alt="FridaMusic Desktop mostrando la sección Explorar" width="560" />
    </td>
    <td align="center" width="50%">
      <strong>Reproductor y cola</strong><br />
      <img src="assets/screenshots/Screenshot%202026-09-23%20162838.png" alt="FridaMusic Desktop mostrando el reproductor y la cola" width="560" />
    </td>
  </tr>
  <tr>
    <td align="center" width="50%">
      <strong>Inicio y recomendaciones</strong><br />
      <img src="assets/screenshots/Screenshot%202026-09-23%20162651.png" alt="FridaMusic Desktop mostrando recomendaciones en la pantalla principal" width="560" />
    </td>
    <td align="center" width="50%">
      <strong>Biblioteca</strong><br />
      <img src="assets/screenshots/Screenshot%202026-09-23%20162735.png" alt="FridaMusic Desktop mostrando la biblioteca musical" width="560" />
    </td>
  </tr>
  <tr>
    <td align="center" width="50%">
      <strong>Reproducción inmersiva</strong><br />
      <img src="assets/screenshots/Screenshot%202026-09-23%20162708.png" alt="FridaMusic Desktop mostrando una reproducción con tema dinámico" width="560" />
    </td>
    <td align="center" width="50%">
      <strong>Playlist y contenido relacionado</strong><br />
      <img src="assets/screenshots/Screenshot%202026-09-23%20162207.png" alt="FridaMusic Desktop mostrando una playlist y contenido relacionado" width="560" />
    </td>
  </tr>
</table>

## ✨ Qué ofrece

- 🎵 **Reproducción de escritorio** con controles persistentes, cola y navegación integrada.
- 🔎 **Exploración y búsqueda** de canciones, álbumes, artistas, playlists y contenido compatible.
- 📚 **Biblioteca y playlists** adaptadas a una interfaz de escritorio.
- 📝 **Letras mejoradas** mediante las extensiones e integraciones incluidas en el proyecto.
- 🎨 **Personalización visual** con temas, CSS y fondos dinámicos vinculados al contenido reproducido.
- 🔌 **Sistema de complementos e integraciones** heredado y adaptado de la base open source sobre la que se construye Desktop.
- 🔄 **Actualizador integrado** mediante `electron-updater`, con detección de nuevas versiones, descarga, progreso y reinicio para instalar.
- 🖥️ **Integración con el sistema operativo**, incluidos atajos, controles multimedia y soporte específico por plataforma cuando está disponible.
- 📦 **Distribución multiplataforma** para Windows, macOS y Linux.

## 🧱 Arquitectura y tecnología

La edición Desktop usa una arquitectura distinta a Android: la interfaz y gran parte de la lógica de presentación se desarrollan con tecnologías web y se empaquetan como aplicación de escritorio con Electron.

| Área | Tecnología / función |
| --- | --- |
| Runtime de escritorio | **Electron 42.5.x** |
| Lenguajes principales | **TypeScript, JavaScript, HTML y CSS** |
| UI | **SolidJS**, `solid-element`, `solid-styled-components` |
| Build | **electron-vite / Vite 8** |
| Tooling | **Node.js**, **pnpm**, TypeScript |
| Empaquetado | **electron-builder 26.x** |
| Actualizaciones | **electron-updater 6.x** |
| Pruebas | **Playwright** |
| Multimedia | Howler, FFmpeg WebAssembly y utilidades de audio |
| Servicios e integración | `youtubei.js`, WebSocket y módulos propios/terceros compatibles |
| Integración de escritorio | Discord RPC, MPRIS en Linux y utilidades específicas de Electron |
| Navegación / filtrado | Ghostery Adblocker para Electron |

La configuración de distribución genera paquetes **x64 y ARM64** cuando el formato y la plataforma lo permiten.

## 📥 Descargas oficiales

Todas las builds oficiales de escritorio se publican aquí:

➡️ **[FridaMusic Desktop Releases](https://github.com/jagrdev-MX/FridaMusic-Desktop-Releases/releases)**

### Windows
- Instalador offline **NSIS**.
- Arquitecturas **x64** y **ARM64**.
- El actualizador utiliza metadatos `latest.yml` y blockmaps publicados junto a cada release.

### macOS
- **DMG** y **ZIP**.
- **Intel x64** y **Apple Silicon ARM64**.
- La firma/notarización puede variar según la release; revisa sus notas antes de instalar.

### Linux
- **AppImage**
- **DEB**
- **RPM**
- **tar.gz**
- Builds **x64** y **ARM64** cuando corresponda.

## 🔗 Ecosistema FridaMusic

FridaMusic para Android y FridaMusic Desktop son dos ediciones del mismo ecosistema de **Frida Labs**, con ciclos de desarrollo y distribución independientes.

| Proyecto | Plataforma | Enlace |
| --- | --- | --- |
| **FridaMusic** | Android | [Repositorio público](https://github.com/jagrdev-MX/FridaMusic_OF) |
| **FridaMusic en Google Play** | Android | [Google Play](https://play.google.com/store/apps/details?id=com.jagr.fridamusic) |
| **FridaMusic Android Releases** | Android | [GitHub Releases](https://github.com/jagrdev-MX/FridaMusic_OF/releases) |
| **FridaMusic Desktop** | Windows · macOS · Linux | [Releases oficiales](https://github.com/jagrdev-MX/FridaMusic-Desktop-Releases/releases) |
| **Sitio oficial** | Web | [frida-music-of.vercel.app](https://frida-music-of.vercel.app/) |

Si llegaste aquí buscando la aplicación para teléfono, visita **[FridaMusic Android](https://github.com/jagrdev-MX/FridaMusic_OF)**.  
Si estás en el repositorio Android y buscas la edición para computadora, usa **[FridaMusic Desktop Releases](https://github.com/jagrdev-MX/FridaMusic-Desktop-Releases/releases)**.


## 🌐 Comunidad

Únete a los canales oficiales para seguir el desarrollo, compartir sugerencias o participar con la comunidad:

- 📢 **Telegram:** [https://t.me/FridaLabs](https://t.me/FridaLabs)
- 💬 **Discord:** [https://discord.gg/Gyh7nfWK9k](https://discord.gg/Gyh7nfWK9k)
- 💚 **WhatsApp:** [https://chat.whatsapp.com/CrZyvVqoLPq6QGTbJSSrAX](https://chat.whatsapp.com/CrZyvVqoLPq6QGTbJSSrAX)
- 🐛 **Issues Desktop:** [https://github.com/jagrdev-MX/FridaMusic-Desktop-Releases/issues](https://github.com/jagrdev-MX/FridaMusic-Desktop-Releases/issues)

## 🔄 Actualizaciones

FridaMusic Desktop consulta este repositorio público para buscar nuevas versiones mediante `electron-updater`. Cuando existe una actualización, la aplicación puede mostrar la versión disponible, iniciar la descarga bajo petición, enseñar el progreso y reiniciar para instalarla.

Los archivos `latest*.yml`, `.blockmap` y los ZIP auxiliares forman parte de la infraestructura del actualizador y no deben confundirse con los instaladores destinados al usuario.

## 📦 Código fuente correspondiente

FridaMusic Desktop se distribuye bajo **GPL-3.0**. Cada release binaria debe acompañarse de un archivo:

```text
FridaMusic-Desktop-Source-VERSION.tar.gz
```

Ese archivo contiene el snapshot de código correspondiente a la build distribuida, junto con los submódulos fijados y los avisos aplicables. Los archivos automáticos **“Source code”** que GitHub genera para este repositorio de distribución no sustituyen ese snapshot.

## 🪟 Seguridad en Windows

Las builds actuales pueden distribuirse sin firma digital Authenticode. Debido a ello, Microsoft Defender SmartScreen puede mostrar una advertencia de reputación para ejecutables nuevos o poco prevalentes. Una advertencia de reputación no implica por sí sola que el archivo contenga malware.

Descarga FridaMusic Desktop únicamente desde las **[releases oficiales](https://github.com/jagrdev-MX/FridaMusic-Desktop-Releases/releases)**.

## 🔐 Privacidad y soporte

FridaMusic Desktop funciona principalmente de forma local y Frida Labs no utiliza actualmente un sistema propio de telemetría o analytics para recopilar información de uso de la aplicación. Algunas funciones se comunican con servicios externos necesarios para ofrecer sus capacidades y quedan sujetas a las políticas de esos servicios.

- 📱 [FridaMusic Android](https://github.com/jagrdev-MX/FridaMusic_OF)
- 🌐 [Sitio oficial](https://frida-music-of.vercel.app/)
- 💬 Soporte: [fridalabs.soporte@gmail.com](mailto:fridalabs.soporte@gmail.com)

## ⚖️ Licencia y créditos

FridaMusic Desktop deriva de **Glassy Music** y conserva las obligaciones y atribuciones aplicables de **GPL-3.0**. Glassy Music, a su vez, se apoya en trabajo open source previo, incluido **Pear Desktop**, además de proyectos e integraciones como **Better Lyrics** y otros componentes con sus propias licencias.

Los snapshots de código fuente distribuidos con cada release conservan los archivos de licencia, avisos y créditos pertinentes.

---

<p align="center">
  <strong>FridaMusic Desktop</strong> · Frida Labs<br />
  Tu música. Tu biblioteca. Tu experiencia. Ahora también en el escritorio.
</p>
