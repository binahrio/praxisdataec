# Praxis Data - Landing Page

Landing page profesional para Praxis Data, empresa especializada en protección de datos personales y mitigación de riesgos para el sector salud en Ecuador.

## 🌐 Estructura del Sitio

```
/
├── index.html          # Página principal (Landing Page)
├── aplicaciones.html   # Página de aplicaciones/herramientas
├── logo.png           # Logo de la empresa
├── _redirects         # Configuración de redirecciones para Netlify
├── netlify.toml       # Configuración de Netlify
└── README.md          # Este archivo
```

## 📋 Características

### Página Principal (index.html)
- **Hero Section**: Presentación clara del servicio con llamado a la acción
- **Servicios**: 4 servicios principales explicados detalladamente
- **Proceso**: Metodología en 4 fases (Radiografía, Receta, Tratamiento, Seguro)
- **Sector Objetivo**: Médicos, Clínicas, Hospitales, Laboratorios, Aseguradoras
- **CTA**: Llamado a la acción sobre el costo de no gestionar riesgos
- **Formulario de Contacto**: Funcional y listo para integración

### Página de Aplicaciones (aplicaciones.html)
- **Grid de Apps**: Visualización de herramientas disponibles
- **Subida de Archivos**: Interfaz para subir archivos HTML
- **Instrucciones**: Guía para subir aplicaciones a Netlify

## 🎨 Diseño

- **Paleta de colores**: Azul oscuro (#0a1628) y Dorado (#c9a227)
- **Tipografía**: Inter (cuerpo) + Playfair Display (títulos)
- **Estilo**: Profesional, sobrio, elegante
- **Responsive**: Adaptable a todos los dispositivos

## 🚀 Despliegue en Netlify

### Opción 1: Drag and Drop (Más Simple)
1. Comprima todos los archivos en un archivo ZIP
2. Vaya a [Netlify Drop](https://app.netlify.com/drop)
3. Arrastre y suelte el ZIP
4. ¡Listo! Su sitio estará en línea

### Opción 2: Desde GitHub (Recomendado)
1. Cree un repositorio en GitHub
2. Suba estos archivos al repositorio
3. En Netlify, haga clic en "New site from Git"
4. Seleccione su repositorio
5. Configure:
   - Build command: (dejar vacío)
   - Publish directory: `/`
6. Haga clic en "Deploy site"

### Opción 3: Netlify CLI
```bash
# Instalar Netlify CLI
npm install -g netlify-cli

# Login
netlify login

# Deploy
netlify deploy --prod --dir=.
```

## 📁 Subir Aplicaciones HTML

### Para agregar nuevas aplicaciones:

1. **Simple (un archivo HTML)**:
   - Vaya a la página "Aplicaciones"
   - Use el área de arrastrar y soltar
   - O suba directamente a Netlify

2. **Múltiples archivos**:
   - Cree una carpeta con su aplicación
   - Incluya todos los archivos necesarios (HTML, CSS, JS)
   - Suba la carpeta a Netlify

3. **Vía Netlify Dashboard**:
   - Vaya a su sitio en Netlify
   - Site configuration → File browser
   - Suba sus archivos directamente

## 📧 Configuración del Formulario de Contacto

El formulario está preparado para Netlify Forms:

1. Agregue `data-netlify="true"` al tag `<form>`:
```html
<form class="contact-form" id="contactForm" data-netlify="true" name="contact">
```

2. En Netlify, vaya a Forms para ver las respuestas

O use un servicio como:
- [Formspree](https://formspree.io)
- [Getform](https://getform.io)
- [Netlify Forms](https://docs.netlify.com/forms/setup/)

## 🔧 Personalización

### Cambiar colores:
Edite las variables CSS en `:root`:
```css
:root {
    --color-primary: #0a1628;    /* Azul principal */
    --color-accent: #c9a227;      /* Dorado */
    --color-text: #f8f9fa;        /* Texto claro */
}
```

### Cambiar contenido:
- Edite directamente el HTML en cada sección
- Las secciones están claramente marcadas con comentarios

### Agregar más servicios:
Copie y pegue el bloque `.service-card` en la sección de servicios

## 📱 SEO

El sitio incluye:
- Meta tags descriptivos
- Open Graph tags (para redes sociales)
- Favicon
- Estructura semántica HTML5
- URLs amigables

## 🛡️ Seguridad

Configuración incluida en `netlify.toml`:
- X-Frame-Options: DENY
- X-XSS-Protection
- X-Content-Type-Options
- Referrer-Policy

## 📞 Soporte

Para soporte o consultas:
- Email: info@praxisdata.ec
- Web: [su-sitio].netlify.app

---

**Praxis Data** - Protegemos tu data, cuidamos tu reputación.
