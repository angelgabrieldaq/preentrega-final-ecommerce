# Portfolio Personal — Ángel Acuña

Portfolio web profesional de **Ángel Acuña**, médico interesado en optimización de sistemas de salud mediante tecnología, health operations e interoperabilidad de datos.

---

## 📋 Propósito

Este sitio presenta:
- **Quién soy:** Médico en formación, desarrollador y especialista en health systems operations
- **Qué trabajo:** Proyectos en trazabilidad quirúrgica (KAIROS), automaciones hospitalarias y herramientas de análisis médico
- **Cómo colaborar:** Canal directo para profesionales, instituciones y mentores interesados en mejorar operaciones de salud mediante tecnología

El sitio cumple como:
1. **Portfolio profesional** para mostrar expertise en medicina + desarrollo + ops
2. **Landing page** para KAIROS y otros proyectos
3. **Herramienta de networking** para colaboraciones significativas

---

## 🎯 Contenido Principal

### Secciones
- **Inicio (Hero):** Proposición de valor clara
- **Sobre mí:** Bio, contexto, intereses centrales
- **Proyectos:** KAIROS, automaciones, self-knowledge frameworks
- **Skills:** Expertise en clínica, desarrollo, operaciones y análisis
- **Contacto:** Formulario para colaboraciones y consultas

---

## 🛠️ Tecnologías Utilizadas

### Frontend
- **HTML5:** Estructura semántica completa (`<header>`, `<nav>`, `<main>`, `<section>`, `<footer>`)
- **CSS3:** Responsive design con Flexbox y Grid
  - Variables CSS para consistencia de diseño
  - Media queries para móvil, tablet y desktop
  - Gradientes lineales y propiedades de background
- **Google Fonts:** Tipografías profesionales
  - **Playfair Display:** Display/headings
  - **Inter:** Body text y UI

### Formulario
- **Formspree:** Manejo de envío de mensajes de contacto (gratuito)

### Deployment
- **GitHub Pages:** Hosting gratuito y directo desde repositorio

---

## 📁 Estructura de Archivos

```
portfolio/
├── index.html         # HTML semántico principal
├── styles.css         # CSS responsivo (Flexbox, Grid, Media Queries)
├── README.md          # Este archivo
└── .gitignore         # (Opcional) Archivos a ignorar en Git
```

---

## 🚀 Quick Start

### 1. Clonar el repositorio
```bash
git clone https://github.com/tu-usuario/portfolio.git
cd portfolio
```

### 2. Abrir localmente
Simplemente abre `index.html` en tu navegador, o usa un servidor local:

```bash
# Con Python 3
python -m http.server 8000

# Con Node.js (si tienes live-server instalado)
live-server
```

Luego visita `http://localhost:8000` en tu navegador.

---

## ⚙️ Configuración Formspree

El formulario de contacto usa **Formspree** para recibir mensajes sin backend.

### Setup (una sola vez)

1. **Ir a https://formspree.io**
2. **Crear cuenta gratuita** con tu email
3. **Crear nuevo formulario** (nombre: ej. "portfolio-contact")
4. **Copiar el Form ID** que Formspree te genera (ej. `f_xxxxxx`)
5. **Editar `index.html`** y reemplazar:
   ```html
   action="https://formspree.io/f/YOUR_FORM_ID"
   ```
   Por:
   ```html
   action="https://formspree.io/f/f_xxxxxx"
   ```
6. **Guardar y listo.** Los mensajes llegarán a tu email.

---

## 📱 Responsive Design

El sitio es **100% responsivo** en:
- **Desktop:** 1200px+
- **Tablet:** 768px - 1024px
- **Mobile:** hasta 768px

Implementado con:
- `display: flex` (proyectos, navegación, layout general)
- `display: grid` (skills, secciones de contenido)
- `@media queries` (adaptación automática a tamaños)

---

## 🌐 Deploying a GitHub Pages

### Opción 1: Repositorio con nombre especial (Sitio personal)

Si tu repositorio se llama `tu-usuario.github.io`:

1. Push de cambios
2. GitHub Pages está **automáticamente activo**
3. Tu sitio es accesible en `https://tu-usuario.github.io`

### Opción 2: Repositorio con otro nombre (Sitio de proyecto)

Si tu repositorio se llama `portfolio`:

1. **En GitHub:** Ve a Repo → Settings → Pages
2. **Source:** Selecciona `main` (o tu rama)
3. **Directory:** Mantén `/ (root)`
4. **Save**
5. Tu sitio es accesible en `https://tu-usuario.github.io/portfolio`

### Pasos detallados

```bash
# 1. Inicializar Git (si no está)
git init

# 2. Agregar archivos
git add .

# 3. Primer commit
git commit -m "Initial commit: portfolio setup"

# 4. Crear rama main (si no existe)
git branch -M main

# 5. Conectar con GitHub
git remote add origin https://github.com/tu-usuario/portfolio.git

# 6. Push a GitHub
git push -u origin main

# 7. Esperar ~30 segundos, luego visitar tu URL
# https://tu-usuario.github.io (o .../portfolio si es repo de proyecto)
```

---

## 🎨 Personalización

### Cambiar colores

En `styles.css`, edita las variables CSS:

```css
:root {
    --primary-color: #0066cc;      /* Azul por defecto */
    --primary-dark: #004499;
    --secondary-color: #f0f4ff;
    --text-dark: #1a1a1a;
    --text-light: #666666;
    /* ... más variables */
}
```

### Cambiar tipografías

En `index.html` `<head>`:

```html
<link href="https://fonts.googleapis.com/css2?family=NuevaFuente:wght@400;700&display=swap" rel="stylesheet">
```

En `styles.css`:

```css
:root {
    --font-display: 'NuevaFuente', serif;
    --font-primary: 'Otra Fuente', sans-serif;
}
```

### Agregar más proyectos

En `index.html`, dentro de `.projects-grid`, duplica una tarjeta `.project-card` y edita contenido:

```html
<article class="project-card">
    <div class="project-header">
        <h3>Mi nuevo proyecto</h3>
        <span class="project-status">En progreso</span>
    </div>
    <p class="project-description">Descripción...</p>
    <!-- ... más contenido ... -->
</article>
```

---

## 📋 Requisitos Cumplidos (Clase 8 — Pre-Entrega)

### ✅ 1. Estructura Básica HTML
- HTML5 semántico con `<header>`, `<nav>`, `<main>`, `<section>`, `<footer>`
- README.md incluido explicando propósito de la página

### ✅ 2. Formulario de Contacto
- Campos: Nombre, Email, Asunto, Mensaje
- Integración Formspree funcional
- Validación HTML nativa (`required`)

### ✅ 3. Estilos CSS
- Archivo `styles.css` externo
- Google Fonts (Playfair Display + Inter) correctamente implementadas
- Propiedades background: gradientes lineales en header, colores en secciones

### ✅ 4. Diseño Responsivo
- **Proyectos:** Flexbox con `flex-wrap` y `gap`
- **Skills:** CSS Grid con `grid-template-columns: repeat(auto-fit, minmax(...))`
- **Contacto:** Media queries para adaptación móvil (responsive en todos los tamaños)

### ✅ 5. Multimedia y Navegación
- SVG inline en hero (visualización de datos)
- Navegación interna con lista `<ul>` y enlaces `<a>`
- Links en footer a GitHub, LinkedIn, Email

### ✅ 6. Hosting
- Instrucciones incluidas para GitHub Pages
- Sitio público y funcional

---

## 🔍 Testing

### Verificar responsividad
- Abre en navegador (cualquiera)
- Abre DevTools (`F12`)
- Toggle device toolbar (`Ctrl+Shift+M`)
- Prueba tamaños: iPhone (375px), iPad (768px), Desktop (1200px+)

### Verificar Formspree
- Completa el formulario de contacto
- Deberías recibir un email en tu bandeja

### Verificar enlaces
- Todos los links de navegación deben scrollear suave a la sección
- Links externos abren en tab nuevo

---

## 📝 Licencia

Este proyecto es de código abierto. Siéntete libre de adaptarlo para tu uso.

---

## 👤 Autor

**Ángel Acuña**
- Email: [tu-email@example.com](mailto:tu-email@example.com)
- GitHub: [github.com/tu-usuario](https://github.com)
- LinkedIn: [linkedin.com/in/tu-perfil](https://linkedin.com)

---

## 🤝 Créditos

- **Diseño & Desarrollo:** HTML5 + CSS3 puro (sin frameworks)
- **Tipografía:** Google Fonts
- **Formulario:** Formspree
- **Hosting:** GitHub Pages

---

## 🐛 Soporte

Si encuentras problemas:
1. Verifica que `index.html` y `styles.css` estén en la misma carpeta
2. Revisa la consola del navegador (`F12` → Console) para errores
3. Asegúrate de que el Form ID de Formspree es correcto
4. Limpia caché del navegador si cambios no se ven

---

**Última actualización:** 2026
