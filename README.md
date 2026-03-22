# 🐱 Xata Jr. — Portfolio

> ### 🌐 [Ver Portafolio en Vivo](https://addictive-gamer.github.io/xata-jr-portfolio/) &nbsp;·&nbsp; 📁 [Ver Repositorio](https://github.com/addictive-gamer/xata-jr-portfolio)

![version](https://img.shields.io/badge/version-10.8-blueviolet?style=for-the-badge)
![host](https://img.shields.io/badge/Hosted_by-GitHub_Pages-black?style=for-the-badge&logo=github)
![lang](https://img.shields.io/badge/Bilingüe-ES%20%7C%20EN-9146ff?style=for-the-badge)
![theme](https://img.shields.io/badge/Tema-Oscuro%20%2F%20Claro-c77dff?style=for-the-badge)
![worker](https://img.shields.io/badge/Backend-Cloudflare_Worker_v3.0-orange?style=for-the-badge&logo=cloudflare)

Portafolio personal bilingüe (ES/EN) de **Xata Jr.** (también conocido como **Addictive Gamer**) —
ilustrador, adaptador musical y traductor.
Construido en HTML/CSS/JS vanilla puro, sin frameworks ni bundlers.

**Versión actual:** `v10.8` · **Última actualización:** 21 de marzo de 2026
**Mantenido por:** José Luis Aquino Rivera (Xata Jr. / Addictive Gamer)
**Contacto:** [pepin.aquino.rivera@gmail.com](mailto:pepin.aquino.rivera@gmail.com)

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
9. [Cómo publicar / desplegar](#cómo-publicar--desplegar)
10. [Créditos](#créditos)

---

## 🎨 Sobre Xata Jr.

**Xata Jr.** es el alias artístico de **José Luis Aquino Rivera**, también conocido como **Addictive Gamer**. Ilustrador digital, adaptador musical (translyrics) y traductor (ES/EN) con base en México.

### Identidad

| Campo | Detalle |
|---|---|
| **Alias principal** | Xata Jr. |
| **Alias alternativo** | Addictive Gamer |
| **Disciplinas** | Ilustración · Pixel Art · Música / Translyrics · Traducción |
| **Idiomas de trabajo** | Español · Inglés |
| **Correo** | pepin.aquino.rivera@gmail.com · nekoaddictive@gmail.com |

### El origen del nombre "Xata"

Xata Jr. se creó originalmente para un concurso de versiones alternas de la mascota de un servidor llamado **Xata Family**. La mascota oficial se llamaba Xata — un gato con el ojo derecho morado, femenino. Xata Jr. es esa mascota pero con sombrero de copa, corbata y masculino. Actualmente cuida dos tortugas 🐢🐢

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

**🎨 Arte y Diseño**
Clip Studio Paint · Photoshop · Affinity Suite · Photopea · Aseprite (Pixel Art) · Ibis Paint X · Blockbench · Blender (3D) · Tableta Gráfica Veikk

**🎵 Música y Audio**
BandLab · LMMS · Cakewalk · Synthesizer V · Vocaloid 4 · OpenUtau · Audacity · OBS Studio

**💻 PC Specs**
Mini PC Machenike · AMD Ryzen 7 · AMD Radeon 7600 · 16 GB RAM · Windows 11

---

## 🤝 Colegas y Proyectos

| Proyecto / Estudio | Rol de Xata Jr. | URL |
|---|---|---|
| **RabGamesStudio** — Talk to the Hand | Ilustrador & Sprite Artist | https://gamejolt.com/@RabGamesStudio |
| **Nightmare Labs** | Traductor oficial a Español Latino | https://gamejolt.com/@NightmareLabs |

---

## ✨ Features Completas

### 🌐 Internacionalización (ES/EN)
- Sistema bilingüe **Español / English** sin recargar la página
- `[data-lang]` en `<body>` + clases `.es` / `.en` en cada elemento de texto
- Pop-up de idioma al cargar, con botón toggle fijo en esquina superior derecha
- Todo el contenido traducido: FAQ (22 preguntas), formulario, secciones, mensajes de error, easter egg

### 🎨 Diseño & Identidad Visual
- **Tipografía:** Syne (headings, labels) + DM Sans (cuerpo) vía Google Fonts
- **Paleta oscura** por defecto con variables CSS (`--bg`, `--surface`, `--accent`, etc.)
- **Modo claro / oscuro** con toggle ☀️/🌙, persistido en `localStorage`
- Efecto de ruido (noise texture SVG) como overlay global
- Grilla de fondo sutil en el hero con mask radial CSS

### 🦸 Hero Section
- Full-screen con animaciones de entrada escalonadas (`@keyframes fadeUp`)
- Título con efecto tipográfico: "X" en outline, "ata" en color acento
- **Partículas flotantes** en `<canvas>`: animadas, adaptadas al modo claro/oscuro

### 🖱️ Cursor Personalizado
- Punto (`#cursor-dot`) + anillo (`#cursor-ring`) con lag lerp 12%
- Se agranda al pasar sobre elementos interactivos
- Oculto automáticamente en dispositivos touch

### 📱 Redes Sociales
- Grid responsivo de 9 plataformas con logos SVG inline monocromáticos

### 🖼️ Galería de Portfolio
- Grid responsivo · Overlay al hover · **Visor modal** con zoom lens
- Carga lazy · imágenes desde Instagram CDN + Twitter/X CDN

### ❓ FAQ Acordeón (22 preguntas)
Agrupadas en 5 categorías: General · Arte · Proyectos · Música y traducción · Setup

### 📬 Formulario con contador de caracteres
Ver sección dedicada más abajo.

### 🥚 Easter Egg
- **Trigger 1:** Código Konami `↑ ↑ ↓ ↓ ← → ← → B A`
- **Trigger 2:** 5 clicks rápidos sobre "Jr." en el hero (compatible con móvil)
- Fuerza el cierre del lang-popup con `setProperty('display','none','important')`

---

## 🤖 Arquitectura Técnica (para IA y Desarrolladores)

### Estructura del archivo

```
index.html                    ← único archivo — HTML + CSS inline + JS inline
├── <head>
│   ├── Meta tags (SEO, OG, Twitter Card, theme-color #c77dff)
│   ├── Google Fonts CDN (Syne + DM Sans)
│   ├── Font Awesome 6.5.1 CDN
│   └── <style>  ~700 líneas
│       ├── :root — design tokens dark
│       ├── body.light-mode — design tokens light
│       ├── Cursor personalizado
│       ├── .char-counter · .field-counter-wrap · .field-over
│       ├── .sensitive-field · .sensitive-disclaimer
│       ├── Lang popup · Hero · Partículas
│       ├── Secciones: redes, galería, FAQ, setup, contacto
│       └── Footer · Easter egg · Responsive
├── <body data-lang="">
│   ├── #lang-popup
│   ├── #controls (lang toggle + theme toggle)
│   ├── #cursor-dot + #cursor-ring
│   ├── <header> — Hero + canvas#particles
│   ├── <main> — Todas las secciones
│   ├── <footer>
│   ├── #image-viewer — Modal galería con zoom lens
│   ├── #easter-egg — Popup del easter egg
│   └── <script>  ~550 líneas
│       ├── updateCharCounter(el, max)
│       ├── submit handler con validación de chars
│       └── ...resto de lógica
```

### Sin dependencias externas instaladas

**Sin npm · Sin bundler · Sin framework · Sin build step**
Solo 2 CDNs: Font Awesome 6.5.1 + Google Fonts

### Sistema de Idiomas

```css
[data-lang="es"] .en { display: none !important; }
[data-lang="en"] .es { display: none !important; }
```

---

## 📬 Formulario de Contacto → Cloudflare Worker

### Flujo de envío

```
Usuario llena formulario
       ↓
FormData enviado a Cloudflare Worker (POST)
  con campo source="xata"  ← formData.append explícito en JS
       ↓
Worker identifica fuente → config Xata Jr.
       ↓
Worker envía en paralelo:
  ├── 📧 Email HTML vía Resend → 3 destinatarios
  │     · Adjuntos como body.attachments
  │     · Info sensible en sección amarilla
  └── 💬 Discord DM (bot) → IDs configurados
        · Intento 1: embed Discohook
        · Fallback: markdown enriquecido si DM de bot
        · Adjuntos: embeds SPOILER_ con imagen inline
        · Info sensible: ||spoiler|| al click
```

### Campos del formulario

| ID | `name` | Tipo | Límite | Notas |
|---|---|---|---|---|
| `#cf-name` | `name` | text | **80** | Requerido |
| `#cf-email` | `email` | email | **254** | Requerido · RFC 5321 |
| `#cf-social` | `social` | text | **60** | Opcional — nick/usuario |
| `#cf-social-platform` | `socialPlatform` | select | — | Requerido si `social ≠ ""` |
| `#cf-reason` | `reason` | select | — | Motivo de contacto |
| `#cf-message` | `message` | textarea | **2000** | Requerido · límite Discord |
| `#cf-file` | `attachment` | file | PNG/JPG/GIF/WEBP · 5 MB · ×5 | Opcional |
| `#cf-sensitive` | `sensitiveInfo` | textarea | **500** | Opcional · spoiler Discord |
| *(hidden)* | `source` | — | — | `"xata"` hardcoded |

### Indicador de caracteres restantes

Contador `restantes / máximo` a la derecha debajo de cada campo:

| Nivel | Color | Condición | Animación |
|---|---|---|---|
| Normal | Gris muted | > 50 restantes | — |
| Advertencia | 🟡 Amarillo (`#e8c000`) | ≤ 50 | `c-pulse` |
| Peligro | 🟠 Naranja (`#ff9500`) | ≤ 20 | `c-pulse` |
| Límite | 🔴 Rojo (`#ff4466`) + negrita | ≤ 0 | `c-shake` + borde rojo |

`maxlength` en HTML + validación JS en submit. Reset automático al enviar con éxito.

### Campo de información sensible

Visible siempre. Diseño con borde amarillo tenue, ícono 🔐, franja superior degradada.
Disclaimer de privacidad bilingüe (ES/EN) encima del textarea.

- **Discord (embed):** campo `🔐 Información sensible` con `||contenido||`
- **Discord (markdown):** `> 🔐 **INFORMACIÓN SENSIBLE:**` + `|| contenido ||`
- **Email:** sección con fondo amarillo etiquetada "Información sensible"

### Embeds de Discord (estilo Discohook)

```
content: 🐱 Nuevo mensaje en Xata Jr. Portfolio

[EMBED]
 author: 🖼 Xata Jr. Portfolio · Formulario de contacto
 title:  👤 Nombre del remitente
 color:  #7b2fff (morado Xata)
 fields:
   📧 Correo          [inline]
   🌐 Red social      [inline]  ← solo si se proporcionó
   ␣ spacer           [inline]
   🎯 Motivo          [full]
   💬 Mensaje         [full]
   🔐 Info sensible   [full]  ← ||spoiler|| si se proporcionó
   📎 Adjuntos        [full]  ← solo si los hay
 footer: Xata Jr. Portfolio · favicon
 timestamp: <t:UNIX:f>
```

**Favicon URL:** `https://raw.githubusercontent.com/addictive-gamer/xata-jr-portfolio/refs/heads/main/favicon.png`

### Configuración del Worker (Cloudflare Secrets)

| Secret | Valor |
|---|---|
| `DISCORD_BOT_TOKEN` | Token del bot de Discord |
| `RESEND_API_KEY_XATA` | API key de Resend para Xata Jr. |
| `XATA_DISCORD_ID_1` | `920017830605361232` (Addictive Gamer) |
| `XATA_DISCORD_ID_2` | `536493452549160970` (Colega Xata) |
| `XATA_DISCORD_ID_3` | vacío o `blank` |

### Respuesta del Worker

```json
{
  "success": true,
  "results": { "email": true, "discord": true, "source": "Xata Jr. Portfolio" },
  "errors": []
}
```

---

## 📦 Historial de Versiones

### v10.8 — Contador de caracteres (21 mar 2026)

**➕ Añadido**
- Contador `restantes / máximo` en todos los campos de texto del formulario
- 4 estados: normal → 🟡 amarillo (≤50) → 🟠 naranja (≤20) → 🔴 rojo+shake (≤0)
- `maxlength` en HTML + validación JS secundaria antes del fetch
- Función `updateCharCounter(el, max)` reutilizable
- Reset automático al enviar exitosamente
- Límites: nombre 80 · correo 254 · nick 60 · mensaje 2000 · sensible 500

---

### v10.7 — Campo de información sensible (21 mar 2026)

**➕ Añadido**
- Campo `Información sensible` opcional con diseño amarillo + ícono 🔐
- Disclaimer de privacidad bilingüe
- Discord: `||spoiler||` en embed y markdown · Email: sección amarilla

---

### v10.6 — Worker v2.0 · source fix · Discohook (21 mar 2026)

**🐛 Bug fix crítico**
- `source='xata'` ahora se añade explícitamente en `formData.append('source','xata')` — antes se omitía del FormData manual

**➕ Añadido**
- Embeds Discohook con favicon correcto de Xata Jr.
- Timestamps nativos `<t:UNIX:f>` + `<t:UNIX:R>`
- Adjuntos `SPOILER_` · base64 chunked 32 KB

---

### v10.5 — Red social opcional + selector de plataforma (21 mar 2026)

- `#cf-social` con selector `#cf-social-platform` que aparece dinámicamente
- Validación: si hay nick sin plataforma → error + foco

---

### v10.4 — Cloudflare Worker unificado (2026)

- Integración con Worker unificado · campo `source="xata"`
- Adjuntos múltiples · validación de archivos · feedback visual

---

### v10.0 → v10.3 — Worker iteraciones (2026)

- v10.1: DM Discord · v10.2: adjuntos · v10.3: fixes FormData

---

### v9.x — Web3Forms · Formspree · SEO · Easter Egg · Galería

Ver historial completo en el repositorio.

---

## 🚀 Cómo publicar / desplegar

### GitHub Pages (método actual)

1. Repositorio con `index.html` en la raíz
2. **Settings → Pages → Deploy from branch → main / root**
3. URL: `https://addictive-gamer.github.io/xata-jr-portfolio/`

### Conectar el Cloudflare Worker

1. [workers.cloudflare.com](https://workers.cloudflare.com) → nuevo Worker
2. Pegar `worker-unified.js` (compartido con RabGamesStudio)
3. **Settings → Variables and Secrets** → todos los secrets de la tabla
4. `WORKER_URL` en `index.html` ya apunta a `https://xata-portfolio-bot.addictivegamer.workers.dev`

### Estructura recomendada del repo

```
/
├── index.html   ← el portfolio completo (un solo archivo)
├── favicon.png  ← ícono del tab, embed de redes y cabecera Discord
└── README.md    ← este archivo
```

---

## ✨ Créditos

| Rol | Persona / Herramienta |
|---|---|
| 💡 Idea original del portafolio | **Nepo Edits** |
| 🎨 Dirección de arte, contenido e identidad | **José Luis Aquino Rivera** · [@Addictiive](https://github.com/addictive-gamer) |
| 🤖 Desarrollo v7 — estructura y lógica base | **Gemini AI** (Google) |
| ✨ Rediseño v8–v10.8 — identidad visual, interactividad, worker, embeds | **Claude** (Anthropic) |
| 🧪 Apoyo & Beta Testing | **Alex GD** |
| 🌐 Hosting | **GitHub Pages** |
| 📧 Emails | **Resend** |
| ⚙️ Backend | **Cloudflare Workers v3.0** |
| 🔤 Tipografías | **Google Fonts** (Syne · DM Sans) |
| 🎨 Iconos UI | **Font Awesome 6.5.1** |

---

*Este proyecto es prueba de lo que la creatividad humana y la IA pueden construir juntas. · 2026*

> "Construido bajo mi comando, pero sin Gemini no tendría la página, y si no fuera por Claude no estaría tan estilizada nwn" — Xata Jr.
