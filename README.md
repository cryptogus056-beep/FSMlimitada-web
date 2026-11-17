# FSM Ltda. — Sitio web

Landing de una sola página para **FSM Ltda.** (automatización industrial y sistemas de control ABB), hecha por Barreau Mol.
Reemplaza el sitio WordPress 4.5 (2016) de https://www.fsmltda.cl/.

## Estructura

```
index.html                  Página completa (HTML + CSS + JS en un solo archivo)
assets/brand/               Logo FSM redibujado en vectorial (SVG)
  fsm-logo.svg              Versión principal (fondo rojo)
  fsm-logo-blanco.svg       Para fondos oscuros
  fsm-logo-rojo.svg         Para fondos claros
assets/clientes/            Logos de clientes tomados del sitio original (WebP transparente)
assets/img/                 Fotos del sitio original mejoradas con IA (2K, WebP)
                            *-sm.webp = versión liviana de 800 px
```

## Diseño

- Portada con animación al hacer scroll sobre la foto aérea de Minera Candelaria (inspirada en *Freight Scroll Hero*, motionsites.ai).
- Resto de la página con estilo de catálogo técnico (inspirado en *teenage engineering*, styles.refero.design).
- Colores de FSM: rojo `#E8312A`, grafito `#0E0F11` y papel `#F3F1EC`. Tipografías: Archivo y JetBrains Mono.
- Responde a `prefers-reduced-motion` y funciona sin JavaScript (salvo la animación y el menú móvil).

## Contenido

Todo el texto, los nombres y logos de clientes y las fotos provienen del sitio publicado. No se agregaron clientes ni cifras nuevas.

## Pendiente antes de publicar

- [ ] **Confirmar el teléfono.** El sitio antiguo muestra `56322990953` y su botón llama a `+56322215174`. Se usó el primero (buscar `data-phone` en `index.html`).
- [ ] WhatsApp, si lo tienen.
- [ ] Vigencia del certificado ABB Authorized Value Provider (el publicado vencía en septiembre de 2017).
- [ ] El formulario abre el correo del visitante (`mailto`). Para recibirlo sin eso, conectar Formspree, Netlify Forms o similar.

## Crédito

El pie de página incluye "Sitio desarrollado por Barreau Mol" con la marca `bm`. Si Barreau Mol publica su sitio, enlazarlo ahí.

## Ver en local

```bash
python3 -m http.server 8000
```

Luego abrir http://localhost:8000

## Publicar

Es un sitio estático: sirve en GitHub Pages, Netlify, Vercel o Cloudflare Pages sin compilación.
