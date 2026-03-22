# 🐱 Xata Jr. — Portfolio

> ### 🌐 [Ver Portafolio en Vivo](https://addictive-gamer.github.io/xata-jr-portfolio/) &nbsp;·&nbsp; 📁 [Ver Repositorio](https://github.com/addictive-gamer/xata-jr-portfolio)

![version](https://img.shields.io/badge/version-10.10-blueviolet?style=for-the-badge)
![host](https://img.shields.io/badge/Hosted_by-GitHub_Pages-black?style=for-the-badge&logo=github)
![lang](https://img.shields.io/badge/Bilingüe-ES%20%7C%20EN-9146ff?style=for-the-badge)
![theme](https://img.shields.io/badge/Tema-Oscuro%20%2F%20Claro-c77dff?style=for-the-badge)
![worker](https://img.shields.io/badge/Backend-Cloudflare_Worker_v5.0-orange?style=for-the-badge&logo=cloudflare)
![mobile](https://img.shields.io/badge/Mobile-Optimizado-39ff14?style=for-the-badge)

Portafolio personal bilingüe (ES/EN) de **Xata Jr.** (también conocido como **Addictive Gamer**) —
ilustrador, adaptador musical y traductor. HTML/CSS/JS vanilla puro, sin frameworks.

**Versión actual:** `v10.10` · **Última actualización:** 21 de marzo de 2026
**Mantenido por:** José Luis Aquino Rivera (Xata Jr. / Addictive Gamer)
**Contacto:** pepin.aquino.rivera@gmail.com

---

## 📑 Tabla de Contenidos

1. [Sobre Xata Jr.](#sobre-xata-jr)
2. [Redes Sociales](#redes-sociales)
3. [Herramientas y Setup](#herramientas-y-setup)
4. [Colegas y Proyectos](#colegas-y-proyectos)
5. [Features completas](#features-completas)
6. [Arquitectura técnica](#arquitectura-técnica-para-ia-y-desarrolladores)
7. [Formulario de Contacto → Cloudflare Worker](#formulario-de-contacto--cloudflare-worker)
8. [Historial de Versiones](#historial-de-versiones)
9. [Cómo publicar](#cómo-publicar--desplegar)
10. [Créditos](#créditos)

---

## 🎨 Sobre Xata Jr.

**Xata Jr.** es el alias de **José Luis Aquino Rivera** (también **Addictive Gamer**). Ilustrador digital, adaptador musical (translyrics) y traductor (ES/EN) con base en México.

| Campo | Detalle |
|---|---|
| **Alias principal** | Xata Jr. |
| **Alias alternativo** | Addictive Gamer |
| **Disciplinas** | Ilustración · Pixel Art · Música / Translyrics · Traducción |
| **Idiomas** | Español · Inglés |
| **Correo** | pepin.aquino.rivera@gmail.com · nekoaddictive@gmail.com |

El nombre "Xata Jr." nació en un concurso de versiones alternas de la mascota del servidor **Xata Family**. La mascota original (Xata) era un gato morado femenino — Xata Jr. es la versión masculina con sombrero de copa y corbata. El autor no tiene gatos; cuida dos tortugas 🐢🐢

---

## 🔗 Redes Sociales

| Plataforma | Usuario | URL |
|---|---|---|
| 𝕏 Twitter | @XataJr | https://x.com/XataJr |
| Instagram (principal) | @addictiive.gamer | https://www.instagram.com/addictiive.gamer/ |
| Instagram (arte) | @xata.jr | https://www.instagram.com/xata.jr/ |
| VGen (comisiones) | XataJr | https://vgen.co/XataJr |
| YouTube | @XATAJr | https://www.youtube.com/@XATAJr |
| Twitch | xatajr | https://www.twitch.tv/xatajr |
| Kick | addictivegamer | https://kick.com/addictivegamer |
| GameJolt | @Addictiive | https://gamejolt.com/@Addictiive |
| Ko-fi | xatajr | https://ko-fi.com/xatajr |

---

## 🛠️ Herramientas y Setup

**🎨 Arte:** Clip Studio Paint · Photoshop · Affinity Suite · Photopea · Aseprite · Ibis Paint X · Blockbench · Blender · Tableta Veikk

**🎵 Música:** BandLab · LMMS · Cakewalk · Synthesizer V · Vocaloid 4 · OpenUtau · Audacity · OBS

**💻 PC:** Mini PC Machenike · AMD Ryzen 7 · AMD Radeon 7600 · 16 GB RAM · Windows 11

---

## 🤝 Colegas y Proyectos

| Proyecto | Rol | URL |
|---|---|---|
| **RabGamesStudio** — Talk to the Hand | Ilustrador & Sprite Artist | https://gamejolt.com/@RabGamesStudio |
| **Nightmare Labs** | Traductor ES Latino | https://gamejolt.com/@NightmareLabs |

---

## ✨ Features Completas

### 🌐 Internacionalización (ES/EN)
- `[data-lang]` en `<body>` + clases `.es`/`.en` en cada texto
- Pop-up de selección al cargar · toggle en esquina superior derecha
- Todo traducido: FAQ (22 preguntas), formulario, secciones, easter egg

### 🎨 Diseño
- **Tipografía:** Syne (headings) + DM Sans (cuerpo)
- **Modo claro/oscuro** con toggle ☀️/🌙, persistido en `localStorage`
- Noise texture overlay · grilla de fondo en hero con mask radial

### 🦸 Hero
- Full-screen con animaciones escalonadas `@keyframes fadeUp`
- Partículas flotantes en `<canvas>` — se adaptan al modo claro/oscuro

### 🖱️ Cursor Personalizado
- Punto (`#cursor-dot`) + anillo (`#cursor-ring`) con lerp 12%
- **Desactivado completamente en touch** con `@media (hover: none)` + detección JS

### 📱 Responsive / Mobile
- Breakpoints: `768px` · `480px`
- `@media (hover: none)`: cursor desactivado, `cursor: auto` restaurado
- `font-size: 1rem` en inputs/textareas — **previene autozoom en iOS**
- `.char-counter` a `0.72rem` en ≤480px
- `.sensitive-field` con padding reducido y `min-height: 80px` en ≤480px
- `.field-counter-wrap { overflow: visible }` en ≤768px

### 🖼️ Galería
- Grid responsivo · overlay al hover · visor modal con zoom lens
- Carga lazy · imágenes desde Instagram CDN + Twitter CDN

### ❓ FAQ Acordeón
- 22 preguntas en 5 categorías · apertura/cierre con `max-height`

### 📬 Formulario con contador de caracteres
Ver sección dedicada.

### 🥚 Easter Egg
- **Trigger 1:** Konami `↑ ↑ ↓ ↓ ← → ← → B A`
- **Trigger 2:** 5 clicks rápidos en "Jr." (compatible móvil)

---

## 🤖 Arquitectura Técnica (para IA y Desarrolladores)

### Estructura del archivo

```
index.html  — único archivo, HTML + CSS inline + JS inline
├── <head>
│   ├── Meta SEO · OG · Twitter Card · theme-color #c77dff
│   ├── Font Awesome 6.5.1 CDN
│   ├── Google Fonts CDN (Syne + DM Sans)
│   └── <style>  ~750 líneas
│       ├── :root dark · body.light-mode
│       ├── @media (hover: none) — cursor desactivado en touch
│       ├── .char-counter · .field-counter-wrap · .field-over
│       ├── .sensitive-field · .sensitive-disclaimer
│       ├── Mobile fixes: 768px · 480px
│       └── Hero · Galería · FAQ · Formulario · Footer
├── <body data-lang="">
│   ├── #lang-popup · #controls · #cursor-dot · #cursor-ring
│   ├── <header> — Hero + canvas#particles
│   ├── <main> — todas las secciones
│   ├── <footer>
│   ├── #image-viewer (zoom lens) · #easter-egg
│   └── <script>  ~600 líneas
│       ├── updateCharCounter(el, max)
│       ├── submit handler con validación de chars
│       └── ...resto
```

### Sin dependencias externas instaladas
Sin npm · sin bundler · sin framework · sin build step. Solo CDNs: Font Awesome + Google Fonts.

### Sistema de Idiomas
```css
[data-lang="es"] .en { display: none !important; }
[data-lang="en"] .es { display: none !important; }
```

---

## 📬 Formulario de Contacto → Cloudflare Worker

### Flujo

```
Usuario llena formulario
    ↓
FormData → Cloudflare Worker (POST)  [source="xata" — formData.append explícito]
    ↓
Worker envía en paralelo:
  ├── 📧 Email HTML (Resend) → 3 destinatarios
  │     adjuntos + info sensible incluidos
  └── 💬 Discord DM (bot) → IDs configurados
        mensaje texto markdown con # / ## / > / ` / || ||
        adjuntos como SPOILER_ (blur hasta click)
```

### Campos del formulario

| ID | `name` | Tipo | **Límite** | Notas |
|---|---|---|---|---|
| `#cf-name` | `name` | text | **80** | Requerido |
| `#cf-email` | `email` | email | **254** | Requerido · RFC 5321 |
| `#cf-social` | `social` | text | **60** | Opcional |
| `#cf-social-platform` | `socialPlatform` | select | — | Requerido si social ≠ "" |
| `#cf-reason` | `reason` | select | — | Motivo de contacto |
| `#cf-message` | `message` | textarea | **1000** | Requerido · overhead Discord |
| `#cf-file` | `attachment` | file | PNG/JPG/GIF/WEBP · 5 MB · ×5 | Opcional |
| `#cf-sensitive` | `sensitiveInfo` | textarea | **500** | Opcional · spoiler Discord |
| *(hidden)* | `source` | — | — | `"xata"` en `formData.append` |

### Indicador de caracteres

| Estado | Color | Condición | Animación |
|---|---|---|---|
| Normal | Gris | > 50 restantes | — |
| Advertencia | 🟡 `#e8c000` | ≤ 50 | `c-pulse` |
| Peligro | 🟠 `#ff9500` | ≤ 20 | `c-pulse` |
| Límite | 🔴 `#ff4466` | ≤ 0 | `c-shake` + borde rojo |

### Campo de información sensible
Borde amarillo tenue, ícono 🔐, disclaimer bilingüe. Discord: `||spoiler||`. Email: sección amarilla.

### Mensajes Discord (Worker v4.0)

```
# 🐱 NUEVO MENSAJE — XATA JR. PORTFOLIO

## ── 👤 ──────────────────────────
> 👤 ***Nombre del remitente***
> 📧 **Correo:** `correo@ejemplo.com`
> [red social si se proporcionó]
> [motivo si se proporcionó]

## ── 💬 ──────────────────────────
> 💬 **Mensaje:**
> Contenido del mensaje...

## ── 🔐 ──────────────────────────   ← solo si hay info sensible
> 🔐 ***INFORMACIÓN SENSIBLE***
> -# Maneja con discreción
|| contenido oculto ||

## ── 🕒 ──────────────────────────
-# 🐱 Xata Jr. Portfolio · <t:UNIX:f> · <t:UNIX:R>
```

### Configuración del Worker (Cloudflare Secrets)

| Secret | Valor |
|---|---|
| `DISCORD_BOT_TOKEN` | Token del bot de Discord |
| `RESEND_API_KEY_XATA` | API key de Resend para Xata Jr. |
| `XATA_DISCORD_ID_1` | `920017830605361232` (Addictive Gamer) |
| `XATA_DISCORD_ID_2` | `536493452549160970` (Colega Xata) |
| `XATA_DISCORD_ID_3` | vacío o `blank` |

> **Compatibilidad:** Xata Jr. y RabGamesStudio comparten el mismo Worker (`worker-unified.js`). Los campos enviados por ambas páginas son idénticos — el Worker los distingue por `source="xata"` / `source="rab"`. Verificado: ✅ 100% compatible.

---

## 📦 Historial de Versiones

### v10.10 — Optimización móvil (21 mar 2026)

**➕ Añadido**
- `.char-counter` a `0.72rem` en ≤480px
- `.sensitive-field` con padding reducido y `min-height: 80px` en ≤480px
- `.field-counter-wrap { overflow: visible }` en ≤768px — el contador no se corta

> Nota: `@media (hover: none)` y `font-size: 1rem` anti-iOS-zoom ya estaban implementados desde versiones anteriores ✓

---

### v10.9 — Límite mensaje corregido (21 mar 2026)

- Límite campo mensaje: **2000 → 1000** (overhead Discord · Worker trunca dinámicamente)

---

### v10.8 — Contador de caracteres (21 mar 2026)

- Contador `restantes / máximo` con 4 estados de color + animaciones
- `maxlength` HTML + validación JS · reset al enviar

---

### v10.7 — Campo información sensible (21 mar 2026)

- Campo `Información sensible` con diseño amarillo + 🔐
- Discord: `||spoiler||` · Email: sección amarilla

---

### v10.6 — Worker v2.0 · source fix · Discohook (21 mar 2026)

**🐛 Bug fix crítico:** `source='xata'` ahora se añade explícitamente en `formData.append` — antes se omitía del FormData manual y el Worker no identificaba correctamente el origen.

---

### v10.5 — Red social opcional + plataforma (21 mar 2026)

- `#cf-social` con selector dinámico `#cf-social-platform`

---

### v10.4 → v9.0

Ver historial completo en el repositorio.

---

## 🚀 Cómo publicar / desplegar

1. `index.html` + `favicon.png` en la raíz del repositorio
2. **Settings → Pages → Deploy from branch → main / root**
3. URL: `https://addictive-gamer.github.io/xata-jr-portfolio/`

**Conectar el Worker** (compartido con RabGamesStudio):
1. [workers.cloudflare.com](https://workers.cloudflare.com) → pegar `worker-unified.js`
2. **Settings → Variables and Secrets** → todos los secrets
3. `WORKER_URL` ya apunta a `https://xata-portfolio-bot.addictivegamer.workers.dev`

---

## ✨ Créditos

| Rol | Persona / Herramienta |
|---|---|
| 💡 Idea original | **Nepo Edits** |
| 🎨 Arte, contenido e identidad | **José Luis Aquino Rivera** (Xata Jr.) |
| 🤖 Desarrollo v7 — base | **Gemini AI** (Google) |
| ✨ Rediseño v8–v10.10 | **Claude** (Anthropic) |
| 🧪 Beta Testing | **Alex GD** |
| 🌐 Hosting | **GitHub Pages** |
| 📧 Emails | **Resend** |
| ⚙️ Backend | **Cloudflare Workers v5.0** |
| 🔤 Tipografías | **Google Fonts** (Syne · DM Sans) |
| 🎨 Iconos | **Font Awesome 6.5.1** |

---

*Este proyecto es prueba de lo que la creatividad humana y la IA pueden construir juntas. · 2026*

> "Construido bajo mi comando, pero sin Gemini no tendría la página, y si no fuera por Claude no estaría tan estilizada nwn" — Xata Jr.
