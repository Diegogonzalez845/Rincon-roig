# Construcciones y Reformas Rincón Roig — Web Oficial

Sitio web corporativo de **Construcciones y Reformas Rincón Roig**, empresa de construcción y reformas con sede en Huesca, Aragón.

## 🚀 Publicar en GitHub Pages (gratis, en 5 minutos)

### Paso 1 — Sube el proyecto a GitHub
```bash
git init
git add .
git commit -m "Primer commit: web Rincón Roig"
git branch -M main
git remote add origin https://github.com/TU_USUARIO/rincon-roig-web.git
git push -u origin main
```

### Paso 2 — Activa GitHub Pages
1. Ve a tu repositorio en GitHub
2. **Settings** → **Pages** (menú lateral izquierdo)
3. En *Source* selecciona **Deploy from a branch**
4. En *Branch* selecciona **main** y carpeta **/ (root)**
5. Haz clic en **Save**

Tu web estará disponible en:
`https://TU_USUARIO.github.io/rincon-roig-web/`

---

## 🌐 Alternativas de publicación

### Netlify (recomendado — dominio personalizado gratis)
1. Ve a [netlify.com](https://netlify.com) y crea una cuenta gratuita
2. Haz clic en **Add new site → Import from Git**
3. Conecta tu repositorio de GitHub
4. En *Build settings* deja todo vacío (es HTML estático)
5. Clic en **Deploy site**

Después puedes conectar tu dominio propio (ej. `rinconroig.es`) desde Site settings → Domain management.

### Vercel
```bash
npx vercel --prod
```

---

## ✏️ Cómo editar el contenido

Abre `index.html` con cualquier editor de texto (VSCode recomendado).

| Qué editar | Dónde buscarlo en el código |
|---|---|
| Teléfonos | Busca `974 000 000` |
| Email | Busca `info@rinconroig.es` |
| Dirección | Busca `Santo Cristo de los Milagros` |
| WhatsApp | Busca `href="#"` en el botón flotante y pon `https://wa.me/34600000000` |
| Textos hero | Busca `Construimos para Durar` |
| Testimonios | Busca `Carlos Martínez` |

---

## 🗂️ Estructura del proyecto

```
rincon-roig-web/
├── index.html      ← Toda la web (una sola página)
└── README.md       ← Este archivo
```

La web usa únicamente recursos externos (CDN), no necesita instalar nada:
- **Tailwind CSS** — estilos
- **Google Fonts** — tipografías (Metropolis, Hanken Grotesk)
- **Material Symbols** — iconos

---

## 📋 Pendiente personalizar antes de publicar

- [ ] Número de teléfono real
- [ ] Email real
- [ ] Enlace de WhatsApp real (`https://wa.me/34XXXXXXXXX`)
- [ ] Fotos de proyectos realizados (sustituir imágenes de ejemplo)
- [ ] Enlace a Google Maps real (busca `Ver en Google Maps` en el HTML)
- [ ] Formulario de contacto funcional (ver sección siguiente)

### Activar el formulario de contacto
El formulario actual no envía emails. Para activarlo gratis:
1. Regístrate en [formspree.io](https://formspree.io)
2. Crea un nuevo formulario y copia tu `action URL`
3. En `index.html` busca `<form class="space-y-6">` y añade `action="https://formspree.io/f/XXXX" method="POST"`
