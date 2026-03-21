# Xata Jr. — Portfolio

> ### 🌐 [Ver Portafolio en Vivo](https://addictive-gamer.github.io/xata-jr-portfolio/) &nbsp;·&nbsp; 📁 [Ver Repositorio](https://github.com/addictive-gamer/xata-jr-portfolio)

![version](https://img.shields.io/badge/version-9.9-blueviolet?style=for-the-badge)
![host](https://img.shields.io/badge/Hosted_by-GitHub_Pages-black?style=for-the-badge&logo=github)
![lang](https://img.shields.io/badge/Bilingüe-ES%20%7C%20EN-9146ff?style=for-the-badge)
![theme](https://img.shields.io/badge/Tema-Oscuro%20%2F%20Claro-c77dff?style=for-the-badge)

Portafolio personal bilingüe (ES/EN) de **Xata Jr.** (también conocido como **Addictive Gamer**) —
ilustrador, adaptador musical y traductor.
Construido en HTML/CSS/JS vanilla puro, sin frameworks, con diseño editorial refinado y experiencia interactiva completa.

---

## ✨ Features completas (v9.0)

### 🌐 Internacionalización
- Sistema bilingüe **Español / English** sin recargar la página
- Implementado con atributo `data-lang` en `<body>` + clases `.es` / `.en` en cada elemento
- Pop-up de selección de idioma al cargar, con botón de toggle fijo en esquina superior derecha
- Todo el contenido (FAQ, formulario, contacto, secciones) está traducido

### 🎨 Diseño & Identidad Visual
- Tipografía: **Syne** (headings, labels, UI) + **DM Sans** (cuerpo) vía Google Fonts
- Paleta oscura por defecto con variables CSS (`--bg`, `--surface`, `--accent`, `--text`, etc.)
- **Modo claro / oscuro** con toggle ☀️/🌙, persistido en `localStorage`
- Efecto de ruido (noise texture) como overlay global para profundidad visual
- Grilla de fondo sutil en el hero con mask radial

### 🦸 Hero Section
- Full-screen con animaciones de entrada escalonadas (`@keyframes fadeUp` con `animation-delay`)
- Título con efecto tipográfico: "X" en outline (`-webkit-text-stroke`), "ata" en color acento
- **Partículas flotantes** en canvas: puntitos animados en el color de acento, se adaptan al tamaño de la ventana y al modo claro/oscuro
- Indicador de scroll animado con pulso

### 🖱️ Cursor Personalizado
- Punto pequeño (`#cursor-dot`) que sigue al mouse exactamente
- Anillo exterior (`#cursor-ring`) con lag suave via `requestAnimationFrame` (lerp al 12%)
- Se agranda al pasar sobre elementos interactivos (links, botones, cards, inputs)
- Oculto automáticamente en dispositivos touch (`@media (hover: none)`)

### 📱 Redes Sociales
- Grid responsivo de 9 plataformas
- Logos SVG inline monocromáticos en `var(--accent)` — coherentes con la paleta
- Hover con lift + glow + escala del logo

### 🖼️ Galería de Portfolio
- Grid responsivo con imágenes desde Instagram CDN
- Overlay con nombre de la obra al hacer hover
- **Visor modal** al hacer click: imagen a pantalla completa con zoom lens (lupa que sigue el cursor al mantener click)
- Carga lazy (`loading="lazy"`)

### ❓ FAQ Acordeón (22 preguntas)
1. ¿Estás disponible para comisiones?
2. ¿Qué herramientas usas para tu música?
3. ¿Puedo entrar a tu servidor de Minecraft?
4. ¿Cómo trabajas en traducciones?
5. ¿Aceptas comisiones de personas que no conoces?
6. ¿Cuánto tardas en entregar una comisión?
7. ¿Qué tipos de trabajo ofreces exactamente?
8. ¿Se puede usar tu arte para proyectos ajenos?

Cada ítem usa `max-height` transition para apertura suave. Solo uno puede estar abierto a la vez.

### 📬 Formulario de Contacto → Instagram DM
- Campos: nombre/usuario, motivo (dropdown), mensaje libre
- Vista previa del mensaje en tiempo real mientras el usuario escribe
- Al enviar, abre Instagram con el DM a **@addictiive.gamer** pre-rellenado via `https://ig.me/m/addictiive.gamer?text=...`
- Completamente bilingüe

### 🥚 Easter Egg (doble trigger)
- **Código Konami**: `↑ ↑ ↓ ↓ ← → ← → B A` en el teclado
- **5 clicks rápidos** sobre el texto "Jr." en el hero (para móvil)
- Abre popup con mensaje personal + dato curioso sobre el origen del nombre "Xata"

### 📋 Otras Secciones
- **Sobre Mí** — descripción y proyectos
- **Colegas** — links a Rab Games Studio y Nightmare Labs
- **Mi Setup** — 3 tarjetas: Arte, Música, PC Specs
- **Créditos Especiales** — Nepo Edits y Alex GD

---

## 🔗 Redes

| Plataforma | Usuario |
|---|---|
| 𝕏 Twitter | [@XataJr](https://x.com/XataJr) |
| Instagram (principal) | [@addictiive.gamer](https://www.instagram.com/addictiive.gamer/) |
| Instagram (arte) | [@xata.jr](https://www.instagram.com/xata.jr/) |
| VGen (comisiones) | [XataJr](https://vgen.co/XataJr) |
| YouTube | [@XATAJr](https://www.youtube.com/@XATAJr) |
| Twitch | [xatajr](https://www.twitch.tv/xatajr) |
| Kick | [addictivegamer](https://kick.com/addictivegamer) |
| GameJolt | [@Addictiive](https://gamejolt.com/@Addictiive) |
| Ko-fi | [xatajr](https://ko-fi.com/xatajr) |

---

## 🤝 Colegas

- **[Rab Games Studio](https://gamejolt.com/@RabGamesStudio)** — Ilustrador y Sprite Artist en *Talk to the Hand*
- **[Nightmare Labs](https://gamejolt.com/@NightmareLabs)** — Traductor oficial a Español Latino

---

## 🛠️ Herramientas y Setup

**🎨 Arte y Diseño**
Clip Studio Paint · Photoshop · Affinity Suite · Photopea · Aseprite · Ibis Paint X · Blockbench · Blender · Tableta Veikk

**🎵 Música y Audio**
BandLab · LMMS · Cakewalk · Synthesizer V · Vocaloid 4 · OpenUtau · Audacity · OBS Studio

**💻 PC**
Mini PC Machenike · AMD Ryzen 7 · AMD Radeon 7600 · 16 GB RAM · Windows 11

---

## 🤖 Información Técnica para IA y Desarrolladores

### Arquitectura
- **Un solo archivo**: todo el proyecto vive en `index.html` (HTML + CSS inline + JS inline)
- **Sin frameworks ni bundlers** — vanilla puro, sin npm, sin build step
- **Dependencias externas** (solo CDN):
  - `font-awesome 6.5.1` — iconos UI
  - `Google Fonts` — Syne + DM Sans

### Sistema de Idiomas
```html
<body data-lang="es">
  <p class="es">Hola</p>   <!-- visible solo en español -->
  <p class="en">Hello</p>  <!-- visible solo en inglés -->
</body>
```
```css
[data-lang="es"] .en { display: none !important; }
[data-lang="en"] .es { display: none !important; }
```

### Variables CSS (Design Tokens)
```css
:root {
  --bg, --surface, --surface2    /* fondos */
  --border                        /* bordes sutiles */
  --accent, --accent2             /* colores de acento */
  --accent-dim, --accent-glow     /* variantes de acento */
  --text, --muted, --muted2       /* tipografía */
}
/* Modo claro: body.light-mode { ... } sobrescribe las variables */
```

### Lógica del Cursor
```js
// Dot sigue al mouse en tiempo real via mousemove
// Ring usa lerp (12%) dentro de requestAnimationFrame
ringX += (mouseX - ringX) * 0.12;
ringY += (mouseY - ringY) * 0.12;
```

### Lógica de Partículas
```js
// Canvas dentro del <header>, z-index: 0
// Densidad: count = Math.floor((W * H) / 14000)
// Cada partícula: posición, velocidad, radio, alpha, delta-alpha
// Color: getComputedStyle(document.documentElement).getPropertyValue('--accent')
// Se redimensiona con window.resize
```

### Formulario → Correo via Web3Forms
```js
// Campos hidden en el form:
// access_key = "fc28079c-..."  ← autentica con Web3Forms
// subject    = "Nuevo mensaje desde el Portfolio de Xata Jr."
// from_name  = "Portfolio de Xata Jr."
// botcheck   = ""  ← honeypot anti-spam

const res = await fetch('https://api.web3forms.com/submit', {
    method: 'POST',
    body: new FormData(form),
    headers: { 'Accept': 'application/json' }
});
```

### Easter Egg
```js
// Trigger 1: secuencia de keyCodes [38,38,40,40,37,39,37,39,66,65] — Konami code
// Trigger 2: 5 clicks en .name-jr dentro de 1500ms
document.getElementById('easter-egg').classList.add('show');
```

### Zoom Lens (visor de imágenes)
```js
// Al mantener click sobre .img-protector:
// - #zoom-lens posicionado en clientX/Y (transform: translate(-50%,-50%))
// - #zoomed-image escalada a 2.5x, desplazada para centrar en el cursor
const f = 2.5;
zi.style.width = (r.width * f) + 'px';
zi.style.left  = -(x * f - 90) + 'px';
zi.style.top   = -(y * f - 90) + 'px';
```

### Prompt sugerido para regenerar o extender con IA
> "Genera un portafolio estático en un solo archivo HTML/JS/CSS. Bilingüe ES/EN via atributo `data-lang` en body + clases `.es`/`.en`. Tema oscuro por defecto con toggle a modo claro usando variables CSS, persistido en localStorage. Canvas de partículas flotantes en el hero. Cursor personalizado: punto exacto + anillo con lerp al 12%. Galería con visor modal y zoom lens (imagen duplicada escalada 2.5x). FAQ acordeón con max-height transition. Formulario que genera DM de Instagram via `ig.me/m/usuario?text=` con preview en tiempo real. Easter egg con Konami code y 5 clicks en el título. Sin frameworks. Dependencias externas solo: Font Awesome 6.5.1 y Google Fonts (Syne + DM Sans)."

---

## 📜 Changelog completo

### v9.9 — Fix formulario Web3Forms (2026)

**🐛 Bug fix**
- Eliminado `formData.append('access_key', ...)` duplicado — ya estaba en el `<input type="hidden">` del HTML, el doble envío causaba el error
- Cambiado `response.ok` por `data.success` para la verificación del resultado — Web3Forms devuelve `{ success: true }` en su JSON, no un HTTP 200 estándar

---

### v9.8 — Web3Forms oficial + adjuntar imagen (2026)

**➕ Añadido**
- 📎 Campo de adjuntar imagen en el formulario de contacto (PNG, JPG, GIF, WEBP · máx. 5 MB)
- Validación de tamaño de archivo en el cliente antes de enviar (muestra error localizado ES/EN si supera 5 MB)
- Estilos propios para `input[type="file"]` con `::file-selector-button` en color acento

**✏️ Editado**
- Submit handler reescrito siguiendo el patrón oficial de Web3Forms (sin header `Accept`, `formData.append('access_key', ...)` explícito, manejo de `data.message` en errores, botón con texto "Enviando..." / "Sending..." durante el envío)
- Botón restaura su HTML original tras el envío (ícono + texto) usando `finally`

**📱 Compatibilidad móvil**
- Cursor personalizado desactivado en touch (`@media (hover: none)`) ✅
- `font-size: 1rem` en inputs previene zoom automático en iOS ✅
- Grid de redes 3 columnas en móvil ✅
- `input[type="file"]` nativo — funciona con la galería de fotos del teléfono ✅

---

### v9.7 — Migración a Web3Forms (2026)

**✏️ Editado**
- Formulario de contacto migrado de **Formspree** a **Web3Forms** (`https://api.web3forms.com/submit`)
- Access key configurada via campo `<input type="hidden" name="access_key">`
- Añadidos campos hidden: `subject` (asunto del email), `from_name` (nombre del remitente) y `botcheck` (anti-spam)
- La lógica de envío asíncrono (`fetch`, feedback ✅/❌) permanece igual

**🗑️ Removido**
- Endpoint y lógica de Formspree (`https://formspree.io/f/xqeyokrq`)

---

### v9.6 — Fixes de eyebrow y easter egg (2026)

**🐛 Bug fix**
- Hero eyebrow EN tenía `style="display:none"` hardcodeado que ignoraba el sistema de idiomas — eliminado, ahora lo controla correctamente la clase `.en`
- Easter egg: `openEgg()` ahora usa `setProperty('display','none','important')` para forzar el cierre del lang-popup sin importar su estado, solucionando el bug de superposición definitivamente

**✏️ Editado**
- Versión actualizada a `v9.6` en el pie de página

---

### v9.5 — FAQ expandido + Easter egg fix (2026)

**🐛 Bug fix**
- Easter egg ya no muestra el popup de idioma por encima — `z-index` subido a `100001` y se fuerza el cierre del lang-popup al abrirlo con `openEgg()`
- Easter egg ahora tiene `overflow-y: auto` para scroll en pantallas pequeñas

**➕ Añadido**
- 🖼️ 2 nuevas imágenes en la galería: *Dibujo de Xata Jr Humano* y *Dibujo de Kasane Teto* (desde Twitter/X CDN), colocadas al inicio
- ❓ 11 nuevas preguntas al FAQ (ahora **22 en total**), agrupadas por categoría:
  - **Arte** — overlays/emotes para streamers, formato PNG, OCs vs fanart, estilos (Furry/Anime/Realista)
  - **Proyectos** — rol exacto en Talk to the Hand, requisitos de The Baka Paradise
  - **Música y traducción** — translyrics, idiomas disponibles (ES/EN)
  - **Setup** — recomendación Parblo Ninos Q, origen del portfolio (Gemini + Claude), historia del nombre "Xata" y las tortugas 🐢🐢
- 🏷️ Versión actualizada a `v9.5` en el pie de página

---

### v9.4 — Scroll, Mobile, FAQ & Versión (2026)

**➕ Añadido**
- ✨ Animaciones de scroll: todas las secciones entran con fade-up usando `IntersectionObserver` (clase `.reveal` + `.visible`)
- ❓ 3 nuevas preguntas al FAQ (11 en total):
  - ¿Tienes Discord?
  - ¿Haces streams o publicas contenido seguido?
  - ¿Qué es Talk to the Hand?
- 🏷️ Versión `v9.4` visible en el pie de página

**✏️ Editado**
- **Móvil mejorado** — grid de redes 3 columnas, logos más compactos, fuente de inputs `1rem` (evita zoom en iOS), padding ajustado en cards, controles más pequeños
- Responsive rediseñado con breakpoints `768px` y `480px` más completos y detallados

---

### v9.3 — Formulario a correo via Formspree (2026)

**✏️ Editado**
- Formulario de contacto migrado de Instagram DM a **Formspree** (`https://formspree.io/f/xqeyokrq`)
- Ahora envía directamente al correo del autor con los campos: nombre, correo de respuesta, motivo y mensaje
- Submit asíncrono con `fetch` — muestra mensaje de éxito ✅ o error ❌ sin recargar la página
- Botón deshabilitado durante el envío para evitar doble submit
- Campo `email` añadido para que el autor pueda responder directamente

**🗑️ Removido**
- Lógica `buildDM()` e integración con `ig.me/m/addictiive.gamer`

---

### v9.2 — Embed de Discord / SEO (2026)

**➕ Añadido**
- Meta tags **Open Graph** para embed rico en Discord, WhatsApp, Telegram y similares
- Meta tags **Twitter/X Card** para preview al compartir en X
- Meta tag `theme-color` — el borde del embed en Discord aparece en `#c77dff` (acento del portfolio)
- Meta tags de SEO: `description` y `author`
- Imagen del embed: `favicon.png` via URL absoluta de GitHub Pages

---

### v9.1 — Fix botones superpuestos (2026)

**🐛 Bug fix**
- Botones de idioma y tema ahora viven dentro de un contenedor `#controls` con `display: flex` y `gap: 8px` en la esquina superior derecha — ya no se superponen

---

### v9.0 — Interactividad & Pulido (2026)

**➕ Añadido**
- 🌙 Modo claro / oscuro con toggle ☀️/🌙 — persistido en `localStorage`
- ✨ Canvas de partículas flotantes animadas en el hero, adaptadas al color de acento activo
- 🥚 Easter egg con dos triggers: Konami code (teclado) y 5 clicks en "Jr." (móvil/desktop)
- ❓ 4 nuevas preguntas al FAQ acordeón:
  - ¿Aceptas comisiones de personas que no conoces?
  - ¿Cuánto tardas en entregar una comisión?
  - ¿Qué tipos de trabajo ofreces exactamente?
  - ¿Se puede usar tu arte para proyectos ajenos?
- 📬 Formulario de contacto completo con preview en tiempo real → DM a `@addictiive.gamer`
- 🖱️ Cursor personalizado: punto + anillo con efecto lag (lerp 12%)
- 🏷️ "También conocido como Addictive Gamer" visible en el hero eyebrow

**✏️ Editado**
- DM del formulario redirige a `@addictiive.gamer` (Instagram principal correcto)
- Logos de redes sociales unificados en `var(--accent)` monocromático para coherencia visual
- Badge de versión actualizado a v9.0

**🗑️ Removido**
- Logos con colores de marca originales (gradiente Instagram, rojo YouTube, verde Kick, etc.)

---

### v8.0 — Rediseño completo (2026)

**➕ Añadido**
- Nueva tipografía: Syne + DM Sans (reemplaza Inter)
- Hero full-screen con animaciones de entrada escalonadas
- Logos SVG inline reales para las 9 redes sociales
- Galería con overlay de nombre al hover + animación zoom/lift
- Tarjetas de créditos con badges de estrella
- Grid de setup dividido en 3 cards (Arte / Música / PC)
- Footer rediseñado con nombre tipográfico como marca

**✏️ Editado**
- FAQ convertido de lista estática a acordeón interactivo
- Layout general rediseñado con estética editorial refinada
- Paleta de colores con design tokens en variables CSS

**🗑️ Removido**
- Fuente Inter
- Estilos glassmorphism (`backdrop-filter` en cards) del v7
- `h2` con decoración de línea (reemplazado por `.section-label`)

---

### v7.0 — Definitive Edition (base original)
- Sistema bilingüe ES/EN dinámico
- Visor de imágenes modal con zoom lens
- 8 redes sociales + 2 perfiles de Instagram
- FAQ estático con `border-left` coloreado
- Setup grid básico en tarjeta única

---

## ✨ Créditos

| Rol | Persona |
|---|---|
| 💡 Idea original del portafolio | **Nepo Edits** |
| 🎨 Dirección de arte, contenido e identidad | **José Luis Aquino Rivera** · [@Addictiive](https://github.com/addictive-gamer) |
| 🤖 Desarrollo v7 — estructura y lógica base | **Gemini AI** |
| ✨ Rediseño v8–v9 — identidad visual, interactividad y features | **Claude** (Anthropic) |
| 🧪 Apoyo & Beta Testing | **Alex GD** |
| 🌐 Hosting | **GitHub Pages** |

---

*Este proyecto es prueba de lo que la creatividad humana y la IA pueden construir juntas. · 2026*
