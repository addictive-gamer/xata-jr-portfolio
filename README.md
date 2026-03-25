# 🐱 Xata Jr. — Portfolio

> ### 🌐 [Ver Portafolio en Vivo](https://addictive-gamer.github.io/xata-jr-portfolio/) &nbsp;·&nbsp; 📁 [Ver Repositorio](https://github.com/addictive-gamer/xata-jr-portfolio)

![version](https://img.shields.io/badge/version-10.12-blueviolet?style=for-the-badge)
![host](https://img.shields.io/badge/Hosted_by-GitHub_Pages-black?style=for-the-badge&logo=github)
![lang](https://img.shields.io/badge/Bilingüe-ES%20%7C%20EN-9146ff?style=for-the-badge)
![theme](https://img.shields.io/badge/Tema-Oscuro%20%2F%20Claro-c77dff?style=for-the-badge)
![worker](https://img.shields.io/badge/Backend-Cloudflare_Worker_v5.2-orange?style=for-the-badge&logo=cloudflare)
![mobile](https://img.shields.io/badge/Mobile-Optimizado-39ff14?style=for-the-badge)

Portafolio personal bilingüe (ES/EN) de **Xata Jr.** (también conocido como **Addictive Gamer**) —
ilustrador, adaptador musical y traductor. HTML/CSS/JS vanilla puro, sin frameworks.

**Versión actual:** `v10.12` · **Última actualización:** 24 de marzo de 2026  
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
8. [Correcciones pendientes conocidas](#-correcciones-pendientes-conocidas)
9. [Historial de Versiones](#historial-de-versiones)
10. [Cómo publicar](#cómo-publicar--desplegar)
11. [Créditos](#créditos)

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
- Desactivado completamente en touch con `@media (hover: none)` + detección JS

### 📱 Responsive / Mobile
- Breakpoints: `768px` · `480px`
- `font-size: 1rem` en inputs/textareas — previene autozoom en iOS
- `.char-counter` a `0.72rem` en ≤480px
- `.field-counter-wrap { overflow: visible }` en ≤768px

### 🖼️ Galería
- Grid responsivo · overlay al hover · visor modal con zoom lens
- Carga lazy · imágenes desde Instagram CDN + Twitter CDN
- ⚠️ URLs de Instagram CDN expiran — renovar si dan 403

### ❓ FAQ Acordeón
- 22 preguntas en 5 categorías · apertura/cierre con `max-height`

### 📬 Formulario de Contacto
- Preview de imágenes adjuntas (miniaturas 76×76px, botón ✕, contador)
- Contador de caracteres con 4 estados de color y animación
- Campo de información sensible con diseño amarillo + spoiler Discord
- Ver sección dedicada para detalles técnicos

### 🥚 Easter Egg
- **Trigger 1:** Konami `↑ ↑ ↓ ↓ ← → ← → B A`
- **Trigger 2:** 5 clicks rápidos en "Jr." (compatible móvil)

---

## 🤖 Arquitectura Técnica (para IA y Desarrolladores)

```
index.html  — único archivo, HTML + CSS inline + JS inline
├── <head>
│   ├── Meta SEO · OG · Twitter Card · theme-color #c77dff
│   ├── Font Awesome 6.5.1 CDN
│   ├── Google Fonts CDN (Syne + DM Sans)
│   └── <style>  ~800 líneas
│       ├── :root dark · body.light-mode
│       ├── @media (hover: none) — cursor desactivado en touch
│       ├── .char-counter · .field-counter-wrap · .field-over
│       ├── .sensitive-field · .sensitive-disclaimer
│       ├── #cf-img-preview · .xata-prev-wrap · .xata-prev-rm
│       ├── Mobile fixes: 768px · 480px
│       └── Hero · Galería · FAQ · Formulario · Footer
├── <body data-lang="">
│   ├── #lang-popup · #controls · #cursor-dot · #cursor-ring
│   ├── <header> — Hero + canvas#particles
│   ├── <main> — todas las secciones
│   ├── <footer>
│   ├── #image-viewer (zoom lens) · #easter-egg
│   └── <script>  ~650 líneas
│       ├── updateCharCounter(el, max)
│       ├── updateXataPreview(input)
│       ├── submit handler con validación de chars
│       └── ...resto
```

---

## 📬 Formulario de Contacto → Cloudflare Worker

### Flujo v5.2

```
Usuario llena formulario
    ↓
FormData → POST https://xata-portfolio-bot.addictivegamer.workers.dev
           [source="xata"]
    ↓
Worker v5.2:
  ├── 1. Discord (CRÍTICO)
  │     XATA_WEBHOOK_URL configurado → Webhook (embed + adjuntos)
  │     Si no → Bot DM a cada ID en XATA_DISCORD_IDS
  │
  ├── 2. D1 database (NON-FATAL)
  │     Falla → se loguea, respuesta sigue siendo { success: true }
  │
  └── 3. Email HTML (non-fatal, background)
```

### Campos del formulario

| ID | `name` | Tipo | **Límite** | Notas |
|---|---|---|---|---|
| `#cf-name` | `name` | text | **80** | Requerido |
| `#cf-email` | `email` | email | **254** | Requerido · RFC 5321 |
| `#cf-social` | `social` | text | **60** | Opcional |
| `#cf-social-platform` | `socialPlatform` | select | — | Requerido si social ≠ "" |
| `#cf-reason` | `reason` | select | — | Motivo de contacto |
| `#cf-message` | `message` | textarea | **1000** | Requerido |
| `#cf-file` | `attachment` | file | PNG/JPG/GIF/WEBP · 5 MB · ×5 | Opcional · con preview |
| `#cf-sensitive` | `sensitiveInfo` | textarea | **500** | Opcional · spoiler Discord |
| *(hidden)* | `source` | — | — | `"xata"` vía `formData.append` |

### Discord Embeds (Worker v5.2)

```
Embed:
  Título:      🐱 Nuevo mensaje — Xata Jr. Portfolio
  Color:       0xc77dff  (morado xata)
  Thumbnail:   favicon.png del portfolio
  Descripción: [nombre] se ha puesto en contacto.
  Campos:
    📧 Correo          [email]         inline
    🎯 Motivo          [motivo]        inline
    🔗 Red social      plat · @user   inline  (solo si aplica)
    💬 Mensaje         [texto max 1024]
    🔒 Info sensible   ||spoiler||     (solo si aplica)
  Footer:      Xata Jr. Portfolio · Portfolio Inbox
  Timestamp:   ISO 8601
  Adjuntos:    SPOILER_archivo.ext (blur hasta click)
```

### Configuración del Worker (Cloudflare Secrets)

| Secret | Descripción |
|---|---|
| `DISCORD_BOT_TOKEN` | Token del bot — requerido para modo DM bot |
| `RESEND_API_KEY_XATA` | API key de Resend para Xata Jr. |
| `XATA_DISCORD_IDS` | IDs de Discord separados por coma |
| `XATA_EMAIL` | Email destino (default: `pepin.aquino.rivera@gmail.com`) |
| `XATA_WEBHOOK_URL` | *(opcional)* URL de Webhook de Discord — prioridad sobre DM bot |

---

## 🐛 Correcciones Pendientes Conocidas

### Página — URLs de galería con expiración (Instagram CDN)

**Severidad:** Media

Las URLs de Instagram contienen tokens de sesión (`oh=`, `oe=`) que expiran. Cuando ocurra, las imágenes darán error 403.

**Solución:** Renovar desde Instagram o migrar a GitHub raw / CDN propio.

---

### Worker — Adjuntos no llegan al email

**Severidad:** Baja — los adjuntos llegan a Discord correctamente. El email solo incluye datos de texto. Mejora futura.

---

## 📦 Historial de Versiones

### v10.12 — Worker v5.2 (24 mar 2026)

**🔧 Worker v5.2 — xata-portfolio-bot (compartido con RGS)**
- **D1 NON-FATAL:** formulario ya no muestra error falso cuando la DB falla
- **Discord Embeds:** embed rico con color morado xata, thumbnail del portfolio, campos inline, spoiler de info sensible
- **Webhook de Discord:** nuevo (`XATA_WEBHOOK_URL`) — si está configurado, se usa en vez del DM bot
- Email HTML mejorado con tabla de campos, blockquote y sección amarilla para info sensible

---

### v10.11 — Preview adjuntos + Worker v5.1 fix (24 mar 2026)

- Preview de imágenes adjuntas: miniaturas 76×76px con botón ✕ y contador
- `updateXataPreview(input)` — función JS nueva
- Fix bot: `socialPlatform` ahora aparece en Discord

---

### v10.10 — Optimización móvil + Worker v5.0 (21 mar 2026)

- `.char-counter` a `0.72rem` en ≤480px
- `.sensitive-field` padding reducido en ≤480px
- `.field-counter-wrap { overflow: visible }` en ≤768px

### v10.9 — Límite mensaje 2000→1000 (21 mar 2026)
### v10.8 — Contador de caracteres (21 mar 2026)
### v10.7 — Campo información sensible (21 mar 2026)
### v10.6 — source fix + Worker v2.0 (21 mar 2026)
### v10.5 — Red social + plataforma opcional (21 mar 2026)
### v10.4 → v9.0 — Ver historial en el repositorio.

---

## 🚀 Cómo publicar / desplegar

1. `index.html` + `favicon.png` en la raíz del repositorio
2. **Settings → Pages → Deploy from branch → main / root**
3. URL: `https://addictive-gamer.github.io/xata-jr-portfolio/`

**Conectar el Worker (bot):**
1. [workers.cloudflare.com](https://workers.cloudflare.com) → pegar `xata-portfolio-bot.js`
2. **Settings → Variables and Secrets** → todos los secrets
3. `WORKER_URL` en el HTML: `https://xata-portfolio-bot.addictivegamer.workers.dev`

**Conectar la database:**
1. Pegar `xata-messages.js` en Worker separado
2. Vincular D1 database como `DB` en los bindings
3. Acceder en `https://xata-messages.addictivegamer.workers.dev/`

---

## ✨ Créditos

| Rol | Persona / Herramienta |
|---|---|
| 💡 Idea original | **Nepo Edits** |
| 🎨 Arte, contenido e identidad | **José Luis Aquino Rivera** (Xata Jr.) |
| 🤖 Desarrollo v7 — base | **Gemini AI** (Google) |
| ✨ Rediseño v8–v10.12 | **Claude** (Anthropic) |
| 🧪 Beta Testing | **Alex GD** |
| 🌐 Hosting | **GitHub Pages** |
| 📧 Emails | **Resend** |
| ⚙️ Backend | **Cloudflare Workers v5.2** |
| 🔤 Tipografías | **Google Fonts** (Syne · DM Sans) |
| 🎨 Iconos | **Font Awesome 6.5.1** |

---

*Este proyecto es prueba de lo que la creatividad humana y la IA pueden construir juntas. · 2026*

> "Construido bajo mi comando, pero sin Gemini no tendría la página, y si no fuera por Claude no estaría tan estilizada nwn" — Xata Jr.
