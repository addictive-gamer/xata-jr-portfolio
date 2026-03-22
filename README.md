# 🐱 Xata Jr. — Portfolio

> ### 🌐 [Ver Portafolio en Vivo](https://addictive-gamer.github.io/xata-jr-portfolio/) &nbsp;·&nbsp; 📁 [Ver Repositorio](https://github.com/addictive-gamer/xata-jr-portfolio)

![version](https://img.shields.io/badge/version-10.6-blueviolet?style=for-the-badge)
![host](https://img.shields.io/badge/Hosted_by-GitHub_Pages-black?style=for-the-badge&logo=github)
![lang](https://img.shields.io/badge/Bilingüe-ES%20%7C%20EN-9146ff?style=for-the-badge)
![theme](https://img.shields.io/badge/Tema-Oscuro%20%2F%20Claro-c77dff?style=for-the-badge)
![worker](https://img.shields.io/badge/Backend-Cloudflare_Worker-orange?style=for-the-badge&logo=cloudflare)

Portafolio personal bilingüe (ES/EN) de **Xata Jr.** (también conocido como **Addictive Gamer**) —
ilustrador, adaptador musical y traductor.
Construido en HTML/CSS/JS vanilla puro, sin frameworks ni bundlers, con diseño editorial refinado y experiencia interactiva completa.

**Versión actual:** `v10.6` · **Última actualización:** 21 de marzo de 2026
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

Xata Jr. se creó originalmente para un concurso de versiones alternas de la mascota de un servidor llamado **Xata Family**. La mascota oficial se llamaba Xata — un gato con el ojo derecho morado, femenino. Xata Jr. es esa mascota pero con sombrero de copa, corbata y masculino. Según el servidor, "Xata" significaba amante de los gatos, aunque el autor nunca ha tenido uno. Actualmente cuida dos tortugas 🐢🐢

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
- Implementado con atributo `data-lang` en `<body>` + clases `.es` / `.en` en cada elemento de texto
- Pop-up de selección de idioma al cargar, con botón de toggle fijo en esquina superior derecha
- Todo el contenido está traducido: FAQ (22 preguntas), formulario, secciones, mensajes de error, preview en tiempo real, easter egg

### 🎨 Diseño & Identidad Visual

- **Tipografía:** Syne (headings, labels, UI) + DM Sans (cuerpo de texto) vía Google Fonts
- **Paleta oscura** por defecto con design tokens en variables CSS (`--bg`, `--surface`, `--accent`, etc.)
- **Modo claro / oscuro** con toggle ☀️/🌙, persistido en `localStorage`
- Efecto de ruido (noise texture SVG) como overlay global para profundidad visual
- Grilla de fondo sutil en el hero con mask radial CSS

### 🦸 Hero Section

- Full-screen con animaciones de entrada escalonadas (`@keyframes fadeUp` + `animation-delay`)
- Título con efecto tipográfico: "X" en outline (`-webkit-text-stroke`), "ata" en color acento
- **Partículas flotantes** en `<canvas>`: puntitos animados en el color de acento, se adaptan al tamaño de ventana y al modo claro/oscuro

### 🖱️ Cursor Personalizado

- Punto pequeño (`#cursor-dot`) que sigue al mouse en tiempo real vía `mousemove`
- Anillo exterior (`#cursor-ring`) con lag suave vía `requestAnimationFrame` (lerp al 12%)
- Se agranda al pasar sobre elementos interactivos (links, botones, cards, inputs)
- Oculto automáticamente en dispositivos touch (`@media (hover: none)`)

### 📱 Redes Sociales

- Grid responsivo de 9 plataformas con logos SVG inline monocromáticos en `var(--accent)`
- Hover con lift + glow + escala del logo

### 🖼️ Galería de Portfolio

- Grid responsivo con imágenes desde Instagram CDN + Twitter/X CDN
- Overlay con nombre de la obra al hacer hover
- **Visor modal** a pantalla completa con zoom lens (lupa que sigue el cursor al mantener click presionado)
- Carga lazy (`loading="lazy"`)

### ❓ FAQ Acordeón (22 preguntas)

Agrupadas por categoría:
- **General** — comisiones, disponibilidad, tipos de trabajo, arte en proyectos ajenos
- **Arte** — overlays/emotes, formatos, OCs vs fanart, estilos
- **Proyectos** — rol en Talk to the Hand, requisitos de The Baka Paradise
- **Música y traducción** — translyrics, idiomas (ES/EN)
- **Setup** — tableta recomendada, origen del portfolio (Gemini + Claude), nombre "Xata", las tortugas

Apertura/cierre con `max-height` transition. Solo uno puede estar abierto a la vez.

### 📬 Formulario de Contacto (Cloudflare Worker)

Ver sección dedicada más abajo para detalles completos.

### 🥚 Easter Egg

- **Trigger 1 — Código Konami:** `↑ ↑ ↓ ↓ ← → ← → B A` en el teclado
- **Trigger 2 — 5 clicks rápidos** sobre el texto "Jr." en el hero (compatible con móvil)
- Abre popup con mensaje personal + dato curioso sobre el origen del nombre "Xata"
- Al activarse, fuerza el cierre del lang-popup con `setProperty('display','none','important')`

### 📋 Secciones Adicionales

- **Sobre Mí** — descripción, especialidades y proyectos activos
- **Colegas** — links a RabGamesStudio y Nightmare Labs
- **Mi Setup** — 3 tarjetas: Arte, Música, PC Specs
- **Créditos Especiales** — Nepo Edits y Alex GD
- **Scroll Reveal** — todas las secciones entran con fade-up via `IntersectionObserver` (clase `.reveal` + `.visible`)

---

## 🤖 Arquitectura Técnica (para IA y Desarrolladores)

### Estructura del archivo

```
index.html                    ← único archivo — HTML + CSS inline + JS inline
├── <head>
│   ├── Meta tags (SEO, OG, Twitter Card, theme-color)
│   ├── Google Fonts CDN (Syne + DM Sans)
│   ├── Font Awesome 6.5.1 CDN
│   └── <style> — Todo el CSS (~600 líneas)
│       ├── :root — design tokens (dark mode)
│       ├── body.light-mode — design tokens (light mode)
│       ├── Cursor personalizado
│       ├── Lang popup
│       ├── Hero + partículas
│       ├── Secciones: redes, galería, FAQ, setup, créditos, contacto
│       └── Footer + Easter egg
├── <body data-lang="">
│   ├── #lang-popup
│   ├── #controls (lang toggle + theme toggle)
│   ├── #cursor-dot + #cursor-ring
│   ├── <header> — Hero + canvas#particles
│   ├── <main> — Todas las secciones
│   ├── <footer>
│   ├── #image-viewer — Modal de galería con zoom lens
│   ├── #easter-egg — Popup del easter egg
│   └── <script> — Todo el JS (~450 líneas)
```

### Sin dependencias externas instaladas

- **Sin npm · Sin bundler · Sin framework · Sin build step**
- Solo 2 CDNs: Font Awesome 6.5.1 + Google Fonts
- Funciona abriendo `index.html` directo en el navegador (excepto el formulario, que necesita el Worker)

### Sistema de Idiomas

```html
<!-- Estructura base -->
<body data-lang="es">
  <p class="es">Hola</p>    <!-- visible solo en español -->
  <p class="en">Hello</p>   <!-- visible solo en inglés -->
</body>
```
```css
[data-lang="es"] .en { display: none !important; }
[data-lang="en"] .es { display: none !important; }
```
```js
function selectLang(l) {
    document.body.setAttribute('data-lang', l);
    // muestra toggle de idioma + toggle de tema
}
```

### Variables CSS (Design Tokens)

```css
:root {
  /* Fondos */
  --bg: #070709;
  --surface: #0f0f14;
  --surface2: #16161e;
  --border: rgba(255,255,255,0.07);

  /* Acentos */
  --accent: #c77dff;
  --accent2: #7b2fff;
  --accent-dim: rgba(199,125,255,0.12);
  --accent-glow: rgba(199,125,255,0.35);

  /* Texto */
  --text: #ececf1;
  --muted: #6b6b7e;
  --muted2: #9898ab;
}

/* Modo claro: body.light-mode { ... } sobrescribe todas las variables */
```

### Lógica del Cursor

```js
// Dot: sigue al mouse exactamente en mousemove
document.addEventListener('mousemove', e => { mouseX = e.clientX; mouseY = e.clientY; });

// Ring: sigue con retraso (lerp 12%) en requestAnimationFrame
function animateCursor() {
    ringX += (mouseX - ringX) * 0.12;
    ringY += (mouseY - ringY) * 0.12;
    ring.style.transform = `translate(${ringX}px, ${ringY}px)`;
    requestAnimationFrame(animateCursor);
}
```

### Lógica de Partículas

```js
// Canvas dentro del <header>, z-index: 0
// Densidad: count = Math.floor((W * H) / 14000)
// Cada partícula: { x, y, vx, vy, r, alpha, da }
// Color: getComputedStyle(document.documentElement).getPropertyValue('--accent')
// Se redimensiona con window.resize → reinicia las partículas
```

### Funciones JS Globales

| Función | Descripción |
|---|---|
| `selectLang(l)` | Aplica idioma 'es' / 'en' al `data-lang` del body |
| `toggleTheme()` | Alterna dark/light mode, persiste en `localStorage` |
| `updatePreview()` | Actualiza la vista previa del formulario en tiempo real |
| `updateSocialPlatformVisibility()` | Muestra/oculta el selector de plataforma según si hay nick |
| `validateFiles(input)` | Valida tipo y tamaño de archivos adjuntos (PNG/JPG/GIF/WEBP, máx 5 MB, hasta 5) |
| `toggleFaq(btn)` | Abre/cierra ítems del acordeón FAQ |
| `openEgg()` / `closeEgg()` | Abre/cierra el easter egg |
| `toggleEggFact()` | Despliega el dato curioso dentro del easter egg |

### Responsive Breakpoints

| Breakpoint | Cambios |
|---|---|
| `768px` | Grid de redes a 3 columnas, cards de setup apiladas, inputs `font-size: 1rem` (anti-zoom iOS) |
| `480px` | Reducción de padding, tipografía más pequeña, elementos de UI más compactos |

---

## 📬 Formulario de Contacto → Cloudflare Worker

### Flujo de envío

```
Usuario llena formulario
       ↓
FormData enviado a Cloudflare Worker (POST)
  con campo source="xata" (explícito en JS)
       ↓
Worker identifica fuente → config Xata Jr.
       ↓
Worker procesa y envía en paralelo:
  ├── 📧 Email HTML estilizado vía Resend → 3 destinatarios
  │     (adjuntos incluidos como attachments en Resend)
  └── 💬 Discord DM con Embed Discohook → IDs configurados
        (adjuntos como embeds separados con imagen inline + spoiler)
```

### Campos del formulario

| Campo HTML | `name` | Tipo | Notas |
|---|---|---|---|
| `#cf-name` | `name` | text | Requerido |
| `#cf-email` | `email` | email | Requerido |
| `#cf-social` | `social` | text | Opcional — nick/usuario |
| `#cf-social-platform` | `socialPlatform` | select | Requerido si `social` tiene valor |
| `#cf-reason` | `reason` | select | Motivo de contacto |
| `#cf-message` | `message` | textarea | Requerido |
| `#cf-file` | `attachment` | file | Opcional · PNG/JPG/GIF/WEBP · máx 5 MB · hasta 5 archivos |
| *(hidden)* | `source` | hidden | `value="xata"` — identifica el origen al Worker |

### Plataformas disponibles en el selector de red social

`discord` · `twitter` · `instagram` · `gamejolt` · `itchio` · `bluesky` · `facebook` · `youtube` · `tiktok` · `otro`

### Validación en el cliente

- Si `social` está vacío → `#cf-platform-row` permanece oculto
- Si `social` tiene texto → `#cf-platform-row` aparece (oninput)
- Al intentar enviar: si `social` ≠ "" y `socialPlatform` = "" → muestra el selector y detiene el envío
- Al resetear el formulario (éxito): oculta el selector y limpia su valor

### Respuesta del Worker

```json
{
  "success": true,
  "results": { "email": true, "discord": true, "source": "Xata Jr. Portfolio" },
  "errors": []
}
```

### Configuración del Worker (Cloudflare Secrets)

| Secret | Descripción |
|---|---|
| `DISCORD_BOT_TOKEN` | Token del bot de Discord |
| `RESEND_API_KEY_XATA` | API key de Resend para este portfolio |
| `XATA_DISCORD_ID_1` | ID Discord: Addictive Gamer (920017830605361232) |
| `XATA_DISCORD_ID_2` | ID Discord: Colega Xata (536493452549160970) |
| `XATA_DISCORD_ID_3` | (vacío por ahora) |

### Embeds de Discord (estilo Discohook)

- **`content`:** `🐱 Nuevo mensaje en Xata Jr. Portfolio` (texto sobre el embed)
- **`author`:** `Xata Jr. Portfolio · Formulario de contacto` + favicon Xata como icono izquierdo
- **`title`:** `👤 [Nombre del remitente]`
- **`thumbnail`:** Favicon de Xata Jr. en esquina superior derecha del embed
  - URL: `https://raw.githubusercontent.com/addictive-gamer/xata-jr-portfolio/refs/heads/main/favicon.png`
- **`color`:** `0x7b2fff` — morado Xata
- **Campos inline (fila 1):** Correo · Red social con emoji de plataforma · spacer invisible
- **Campos block:** Motivo (blockquote) · Mensaje
- **`footer`:** `Xata Jr. Portfolio · timestamp horario México` + favicon como icono
- **Adjuntos:** Cada imagen va en un embed separado con `image.url = attachment://SPOILER_nombre` — renderiza inline con efecto blur (spoiler) hasta que el usuario haga click
- **⚠️ Fix v10.6:** `source='xata'` ahora se incluye explícitamente en el `FormData` del JS

---

## 📦 Historial de Versiones

### v10.6 — Worker v2.0: Discohook + fuente correcta + source fix (21 mar 2026)

**🐛 Bug fix crítico**
- `source='xata'` ahora se añade correctamente al `FormData` en el submit handler de JS
  - Antes: el campo `<input type="hidden" name="source" value="xata">` existía en el HTML pero el JS construía el `FormData` manual y **no lo incluía** — el Worker recibía `source=undefined` y usaba el fallback `xata`, pero era incorrecto por diseño
  - Ahora: `formData.append('source', 'xata')` explícito en la primera línea del handler

**➕ Añadido / Mejorado (Worker v2.0)**
- Embeds de Discord rediseñados al estilo **Discohook**:
  - `author.icon_url` → favicon de Xata Jr. como icono en la línea de autor
  - `title` → `👤 Nombre del remitente`
  - `thumbnail` → favicon de Xata Jr. en esquina superior derecha del embed
    - URL: `https://raw.githubusercontent.com/addictive-gamer/xata-jr-portfolio/refs/heads/main/favicon.png`
  - `footer.icon_url` → favicon de Xata Jr. junto al timestamp
- Adjuntos en Discord: cada imagen en embed separado con `image.url = attachment://SPOILER_nombre` (render inline + spoiler blur)
- Adjuntos en email: incluidos como `body.attachments` en Resend

---

### v10.5 — Nick + Plataforma en formulario & Discord Embeds (2026)

**➕ Añadido**
- 🎯 Campo de **Nick/usuario** en el formulario ahora es **opcional** — cuando se escribe algo, aparece dinámicamente el selector de **red social** (`#cf-platform-row`)
- 🌐 Selector de plataforma con 10 opciones y emoji: Discord · Twitter/X · Instagram · GameJolt · itch.io · Bluesky · Facebook · YouTube · TikTok · Otro
- ✅ Validación: si hay nick sin plataforma → muestra el selector y detiene el envío con feedback visual
- 💬 Discord ahora usa **embeds enriquecidos** en lugar de texto plano: título coloreado, campos estructurados, timestamp ISO, footer, imágenes como embeds spoiler separados
- `socialPlatform` añadido al `FormData` y enviado al Worker

**✏️ Editado**
- Label del campo cambiado a "Nick / usuario (opcional)" / "Nick / username (optional)"
- El campo de red social ya no es un texto libre `@usuario en Instagram, Discord...` — ahora está separado en nick + selector
- Al resetear el formulario (éxito): `#cf-platform-row` vuelve a ocultarse y el select se limpia
- Versión actualizada a `v10.5` en el pie de página

---

### v10.4 — Cloudflare Worker unificado (2026)

**➕ Añadido**
- Integración con **Cloudflare Worker** unificado (`xata-portfolio-bot.addictivegamer.workers.dev`)
- Campo `source="xata"` (hidden) para que el Worker distinga el origen
- Campo de **Red social / Nick** (`#cf-social`) como texto libre
- **Adjuntos** múltiples (`#cf-file`): PNG, JPG, GIF, WEBP · máx 5 MB por archivo · hasta 5 archivos
- Validación de archivos en el cliente (tipo + tamaño) con mensajes bilingües de error y lista de archivos seleccionados
- Feedback visual del botón durante el envío (deshabilitado + texto "Enviando...")
- Mensajes de éxito ✅ y error ❌ debajo del formulario

**✏️ Editado**
- Formulario migrado de Web3Forms a Cloudflare Worker
- Submit handler completamente reescrito

---

### v10.0 → v10.3 — Cloudflare Worker (iteraciones) (2026)

- Worker conectado inicialmente solo a Resend (email)
- DM de Discord añadido en v10.1
- Campo de adjuntos en v10.2
- Correcciones de `FormData` y manejo de errores en v10.3

---

### v9.9 — Fix formulario Web3Forms (2026)

**🐛 Bug fix**
- Eliminado `formData.append('access_key', ...)` duplicado — el doble envío causaba el error
- Cambiado `response.ok` por `data.success` para la verificación del resultado

---

### v9.8 — Web3Forms oficial + adjuntar imagen (2026)

**➕ Añadido**
- Campo de adjuntar imagen: PNG, JPG, GIF, WEBP · máx 5 MB
- Validación de tamaño en el cliente con mensaje localizado ES/EN
- Estilos para `input[type="file"]` con `::file-selector-button` en color acento

**✏️ Editado**
- Submit handler reescrito con patrón oficial Web3Forms
- Botón restaura HTML original tras el envío (ícono + texto) usando `finally`

---

### v9.7 — Migración a Web3Forms (2026)

**✏️ Editado**
- Formulario migrado de Formspree a Web3Forms (`https://api.web3forms.com/submit`)
- Campos hidden: `access_key`, `subject`, `from_name`, `botcheck`

**🗑️ Removido**
- Endpoint de Formspree

---

### v9.6 — Fixes eyebrow y easter egg (2026)

**🐛 Bug fix**
- Hero eyebrow EN tenía `style="display:none"` hardcodeado — eliminado, ahora lo controla `.en`
- Easter egg: `openEgg()` usa `setProperty('display','none','important')` — fix superposición definitivo con lang-popup

---

### v9.5 — FAQ expandido + galería ampliada (2026)

**➕ Añadido**
- 2 nuevas imágenes en galería: *Dibujo de Xata Jr Humano* y *Dibujo de Kasane Teto* (desde Twitter/X CDN)
- 11 nuevas preguntas al FAQ (total: **22 preguntas** en 5 categorías)
- Easter egg: `overflow-y: auto` para scroll en pantallas pequeñas

**🐛 Bug fix**
- Easter egg ya no muestra el popup de idioma por encima — `z-index` subido y `openEgg()` fuerza el cierre del lang-popup

---

### v9.4 — Scroll Reveal + FAQ + Móvil (2026)

**➕ Añadido**
- Animaciones de scroll con `IntersectionObserver` (`.reveal` + `.visible`)
- 3 nuevas preguntas al FAQ (total: 11)
- Versión `v9.4` visible en footer

**✏️ Editado**
- Grid de redes a 3 columnas en móvil, `font-size: 1rem` en inputs (anti-zoom iOS)
- Responsive con breakpoints `768px` y `480px`

---

### v9.3 — Formulario a correo (Formspree) (2026)

**✏️ Editado**
- Formulario migrado de Instagram DM a Formspree
- Submit asíncrono con feedback ✅/❌ sin recargar la página
- Campo `email` añadido para poder responder directamente

**🗑️ Removido**
- Lógica `buildDM()` e integración con `ig.me/m/addictiive.gamer`

---

### v9.2 — SEO + Discord Embed (2026)

**➕ Añadido**
- Meta tags Open Graph completos (Discord, WhatsApp, Facebook, Telegram)
- Meta tags Twitter/X Card
- `theme-color` → `#c77dff` (borde del embed en Discord)
- Meta tags SEO: `description`, `author`

---

### v9.1 — Fix controles superpuestos (2026)

**🐛 Bug fix**
- Contenedor `#controls` con `display: flex` y `gap: 8px` — botones de idioma y tema ya no se superponen

---

### v9.0 — Interactividad completa (2026)

**➕ Añadido**
- 🌙 Modo claro/oscuro con toggle ☀️/🌙, persistido en `localStorage`
- ✨ Canvas de partículas flotantes en el hero
- 🥚 Easter egg con dos triggers (Konami + 5 clicks en "Jr.")
- 📬 Formulario con preview en tiempo real → DM a `@addictiive.gamer`
- 🖱️ Cursor personalizado: punto + anillo con lerp 12%
- 4 nuevas preguntas al FAQ

---

### v8.0 — Rediseño completo (2026)

**➕ Añadido**
- Nueva tipografía: Syne + DM Sans (reemplaza Inter)
- Hero full-screen con animaciones escalonadas
- Logos SVG inline para 9 redes sociales
- Galería con overlay al hover + visor modal con zoom lens
- Grid de setup en 3 cards (Arte / Música / PC)
- Footer rediseñado con nombre tipográfico

**✏️ Editado**
- FAQ de lista estática a acordeón interactivo

**🗑️ Removido**
- Fuente Inter · Estilos glassmorphism · `h2` con decoración de línea

---

### v7.0 — Base original (2026)

- Sistema bilingüe ES/EN dinámico
- Visor de imágenes modal con zoom lens
- 8 redes sociales + 2 perfiles de Instagram
- FAQ estático
- Setup grid básico

---

## 🚀 Cómo publicar / desplegar

### GitHub Pages (método actual)

1. Crea un repositorio en GitHub
2. Asegúrate de que el archivo se llame `index.html`
3. Ve a **Settings → Pages → Source → Deploy from branch → main / root**
4. Tu web estará en `https://TU_USUARIO.github.io/NOMBRE_DEL_REPO/`

Para dominio personalizado: agrega un archivo `CNAME` con tu dominio y configura los DNS.

### Estructura recomendada del repo

```
/
├── index.html          ← el portfolio completo (un solo archivo)
├── favicon.png         ← ícono del tab y embed de redes
└── README.md           ← este archivo
```

### Conectar el Cloudflare Worker

1. Crea una cuenta en [workers.cloudflare.com](https://workers.cloudflare.com)
2. Crea un nuevo Worker y pega el código de `worker-unified.js`
3. Ve a **Settings → Variables and Secrets** y configura todos los secrets (ver tabla arriba)
4. En `index.html`, cambia `WORKER_URL` por la URL de tu Worker:
   ```js
   const WORKER_URL = 'https://TU-WORKER.TU-CUENTA.workers.dev';
   ```

---

## ✨ Créditos

| Rol | Persona / Herramienta |
|---|---|
| 💡 Idea original del portafolio | **Nepo Edits** |
| 🎨 Dirección de arte, contenido e identidad | **José Luis Aquino Rivera** · [@Addictiive](https://github.com/addictive-gamer) |
| 🤖 Desarrollo v7 — estructura y lógica base | **Gemini AI** (Google) |
| ✨ Rediseño v8–v10.5 — identidad visual, interactividad, worker, embeds | **Claude** (Anthropic) |
| 🧪 Apoyo & Beta Testing | **Alex GD** |
| 🌐 Hosting | **GitHub Pages** |
| 📧 Emails | **Resend** |
| ⚙️ Backend | **Cloudflare Workers** |
| 🔤 Tipografías | **Google Fonts** (Syne · DM Sans) |
| 🎨 Iconos UI | **Font Awesome 6.5.1** |

---

*Este proyecto es prueba de lo que la creatividad humana y la IA pueden construir juntas. · 2026*

> "Construido bajo mi comando, pero sin Gemini no tendría la página, y si no fuera por Claude no estaría tan estilizada nwn" — Xata Jr.
