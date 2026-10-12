# TP4 — Landing Page "Coffea" (HTML + CSS)

Landing page estática de una sola página para la cafetería ficticia **Coffea**, desarrollada para la materia **Diseño UX-UI (Licenciatura en Sistemas de Información - FCyT UADER, 2026)**. Reproduce con fidelidad visual el diseño de Figma a 1920 px y cuenta con diseño responsivo completo.

## 🚀 Stack Tecnológico
* **HTML5 Semántico** (Estructura optimizada y accesibilidad WCAG 2.2 AA).
* **CSS3 Puro** (Organizado por capas con `@layer tokens, base, layout, components, utilities`).
* **Design Tokens** (Centralización de colores, tipografías, radios y espaciados mediante Custom Properties).
* **Flexbox y CSS Grid** (Maquetación moderna sin frameworks ni preprocesadores).
* **Interacciones 100% CSS** (Carruseles con `scroll-snap`, estados `:checked` para favoritos, sin JavaScript).

## 📁 Estructura del Proyecto
```text
coffea-landing/
├── index.html          # Estructura principal de la landing page
├── 404.html            # Página de error personalizada para Netlify
├── netlify.toml        # Configuración de deploy, headers de caché y seguridad
├── README.md           # Documentación del proyecto
├── css/
│   ├── main.css        # Archivo centralizador con la directiva @layer
│   ├── tokens.css      # Variables globales (colores, fuentes, espacios)
│   ├── base.css        # Resets modernos y estilos base tipográficos
│   ├── layout.css      # Contenedores globales y grillas de sección
│   ├── utilities.css   # Clases de ayuda y accesibilidad (.visually-hidden)
│   └── components/     # Estilos específicos BEM por componente
│       ├── header.css
│       ├── hero.css
│       ├── categories.css
│       ├── product-card.css
│       ├── carousel.css
│       ├── promo.css
│       ├── testimonial-card.css
│       ├── newsletter.css
│       └── footer.css
└── assets/
    ├── img/            # Imágenes en formato AVIF / WebP con optimización
    ├── icons/          # Íconos SVG optimizados
    └── fonts/          # Fuentes locales (si aplica)
```

## 📐 Decisiones de Diseño y Responsive
* **Desktop First / Responsive Multi-breakpoint**: Adaptación fluida desde 360px hasta 1920px sin scroll horizontal, utilizando media queries orientadas a tablets (1024px, 768px) y móviles (<767px).
* **Optimización de Assets**: Uso de imágenes en formato .avif y .svg con atributos width y height explícitos para evitar el Cumulative Layout Shift (CLS).

## 🛠️ Cómo levantar el proyecto en local
* Clona o descarga este repositorio en tu computadora.
* Abre la carpeta del proyecto en tu entorno de desarrollo (como Visual Studio Code).
* Utiliza la extensión Live Server para levantar el archivo index.html en un servidor local, evitando problemas con las rutas relativas de las imágenes y los archivos CSS.

## 🌐 Despliegue
Sitio estático configurado para producción automática en Netlify con HTTPS activo, cabeceras de caché inmutables para recursos estáticos y redirección de errores a 404.html.