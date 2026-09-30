# 🎨 ColorFilter — Android Retro Screen Filter & Eye Care

[![Release](https://img.shields.io/github/v/release/LuisRZJ/android-color-filter-app?color=FFB300&style=for-the-badge&logo=android)](https://github.com/LuisRZJ/android-color-filter-app/releases/latest)
[![Platform](https://img.shields.io/badge/Platform-Android%208.0%2B-3DDC84?style=for-the-badge&logo=android)](https://www.android.com/)
[![License](https://img.shields.io/badge/License-GPL%20v3-blue.svg?style=for-the-badge)](LICENSE)
[![No Ads](https://img.shields.io/badge/Ads-100%25%20Free-brightgreen?style=for-the-badge)](#privacidad-y-seguridad)

Filtro de pantalla avanzado para Android con **efectos analógicos retro CRT**, perfiles de descanso visual, **widget flotante arrastrable**, filtrado selectivo por aplicación (**lista negra y blanca**) y automatización programada.

[📥 Descargar APK (Última Versión)](https://github.com/LuisRZJ/android-color-filter-app/releases/latest)

---

## ✨ Características Destacadas

### 📺 1. Modos Retro CRT y Distorsión Analógica en Vivo
Renderizado gráfico procedimental acelerado por hardware para convertir tu pantalla en un monitor de época:
* **Scanlines (Líneas de barrido):** Texturizado nítido repetido en bucle sin sobrecargar la CPU.
* **Curvatura y Viñeta de Tubo:** Efecto esférico radial que replica las pantallas de rayos catódicos de los 80s y 90s.
* **Barrido V-Hold animado:** Desplazamiento dinámico en tiempo real que simula el refresco electromagnético analógico de 50/60 Hz.
* **Presets Históricos:**
  * 🖥️ *Monitor CRT Clásico (VGA 90s)*
  * 🟢 *Fósforo Verde (IBM 5151 / Matrix monocromático)*
  * 🟠 *Terminal Ámbar (DEC VT220 de alto descanso ocular)*
  * 📼 *TV Tubo / VHS (Barras de desincronización y ruido de estática)*
  * ⚡ *Cyberpunk Glitch (Interferencia electromagnética viva)*

### 🛡️ 2. Disponibilidad por Aplicación (Listas Negra y Blanca)
* **Todas las Apps (Global):** El filtro funciona de forma uniforme en todo el sistema.
* **Lista Negra:** El filtro se apaga automáticamente en apps sensibles a la fidelidad de color (como la Cámara, Galería o Videojuegos).
* **Lista Blanca:** El filtro se enciende **únicamente** cuando abres apps designadas (lectores de libros, navegador, procesadores de texto).

### 🎈 3. Widget Flotante Rápido
* Burbuja circular arrastrable que permanece sobre otras aplicaciones.
* **Física magnética (*Snap to Edge*):** Se adhiere suavemente a los bordes de la pantalla al soltarla.
* Panel desplegable con chips rápidos para alternar perfiles al instante.
* **Cierre en 1 clic (✕):** Botón directo para retirarlo sin abrir la aplicación.

### ⏰ 4. Horarios y Estadísticas de Salud Visual
* Programa encendido y apagado automático según la hora del día.
* Contador en tiempo real del tiempo de exposición y desglose por perfiles.

### 📸 5. Captura Limpia (Screenshots sin filtro)
* Botón *"Pausa 15s"* directo en la barra de notificaciones para tomar capturas de pantalla con los colores originales del sistema.

---

## 📲 Instalación

1. Descarga el archivo [`app-release.apk`](https://github.com/LuisRZJ/android-color-filter-app/releases/latest) de la sección de **Releases**.
2. Abre el archivo en tu dispositivo Android.
3. Si el sistema lo requiere, activa la opción **"Permitir desde esta fuente"**.
4. Si aparece el aviso preventivo de Google Play Protect, toca en **"Más detalles"** y luego en **"Instalar de todas formas"**.
5. Abre la aplicación y concede los permisos solicitados:
   * **Mostrar sobre otras aplicaciones:** Indispensable para proyectar el filtro de luz y el widget flotante.
   * **Acceso de uso:** *(Opcional)* Requerido únicamente para detectar qué app está abierta y aplicar la Lista Negra / Blanca.

---

## 🔒 Privacidad y Seguridad

* **Sin anuncios ni rastreadores:** 100% libre de publicidad y código espía.
* **Protección Anti-Tapjacking:** La opacidad de la ventana está estrictamente calibrada por debajo del límite de seguridad de Android para garantizar que ningún botón ni gesto del sistema quede bloqueado.
* **Respaldo en la Nube Transparente:** La sincronización de ajustes se realiza contra tus propios repositorios mediante la API oficial de GitHub; ningún tercero tiene acceso a tus datos.

---

## 🛠️ Stack Tecnológico

* **Lenguaje:** Kotlin
* **Interfaz de Usuario:** Jetpack Compose & Material 3
* **Motor Gráfico:** `Canvas`, `BitmapShader` y `LinearGradient`/`RadialGradient` acelerados por hardware
* **Servicio:** Android Foreground Service con canales de notificación dedicados
* **Arquitectura:** Módulos desacoplados de persistencia (`SharedPreferences`), alarmas (`AlarmManager`) y detección de primer plano (`UsageStatsManager`).

---

## 📄 Licencia

Este proyecto está bajo la Licencia **GNU General Public License v3.0 (GPLv3)**. Consulta el archivo [LICENSE](LICENSE) para más detalles.
