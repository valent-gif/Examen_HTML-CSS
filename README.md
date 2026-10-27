# 🌿 EcoMarket | Compra responsable, vive sostenible

**EcoMarket** es una tienda en línea dedicada exclusivamente a productos ecológicos, reutilizables y sustentables. Su objetivo es ofrecer una plataforma accesible, limpia y atractiva donde los usuarios puedan explorar alternativas sostenibles, conocer el impacto positivo de cada compra y comunicarse con la tienda, todo desarrollado con **HTML5 semántico y CSS3 puro (Cero JavaScript)**.

---

## 📋 Características y Vistas del Proyecto

1. **Página de Inicio (`index.html`)**
   - Encabezado sticky con navegación principal (`Inicio`, `Productos`, `Nosotros`, `Contacto`) y accesos directos a buscador y carrito.
   - Banner principal (*Hero*) a ancho completo con animación de entrada (`@keyframes aparecer`) y llamado a la acción (*CTA*).
   - Cuadrícula responsiva de **6 productos destacados** con efecto de elevación suave (`hover`).
   - Pie de página común con información de contacto, enlaces legales y redes sociales.

2. **Catálogo de Productos (`views/productos.html`)**
   - Barra superior con buscador estilizado.
   - Matriz responsiva con **CSS Grid** de **20 productos ecológicos** (`1 columna` en móvil, `2 columnas` en tablet y `4 columnas` en escritorio).
   - Tarjetas de producto con insignia de disponibilidad (*En Stock* / *Agotado*), categoría, precio y botón interactivo de **Favoritos** sin JavaScript (implementado mediante `input[type="checkbox"]` + `:checked` y `:active`).
   - Bloque de paginación visual al final del catálogo (`Anterior`, `1`, `2`, `3`, `Siguiente`).

3. **Sobre Nosotros (`views/sobre-nosotros.html`)**
   - **Nuestra Misión**: Sección de historia maquetada con **Flexbox** adaptativo (imagen + relato del origen en Bucaramanga).
   - **Principios Ecológicos**: Cuadrícula de 4 pilares (*100% Sin Plástico*, *Comercio Justo*, *Economía Circular*, *Cruelty Free*) con iconografía vectorial propia en `img/icons/`.
   - **Testimonios**: Carrusel horizontal con `scroll-snap` en móvil/tablet y cuadrícula en escritorio con tarjetas interactivas (`hover`), estrellas de calificación y avatares ilustrados.

4. **Página de Contacto (`views/contacto.html`)**
   - **Formulario Inteligente**: Campos para Nombre, Correo electrónico y Mensaje con **validación visual en tiempo real mediante pseudo-clases CSS (`:valid` / `:invalid`)** — bordes rojos para campos vacíos o inválidos y verdes para campos válidos, además de mensaje de confirmación con `:target`.
   - **Mapa de Ubicación**: Mapa estático estilizado de la tienda física en Bucaramanga (`img/hero/mapa-ubicacion.svg`) junto con horarios y datos de atención.
   - **Redes Sociales**: Botones con iconos vectoriales y animación `transform: scale()` al pasar el cursor (`hover`).

---

## 🛠️ Tecnologías Utilizadas

- **HTML5 Semántico**: Uso de etiquetas estructurales (`<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<aside>`, `<figure>`, `<figcaption>`, `<footer>`) y atributos de accesibilidad (`aria-label`, `aria-current`).
- **CSS3 Puro (0% JavaScript)**:
  - **Variables CSS (`:root`)**: Paleta natural (`#2ecc71`, `#27ae60`, `#f5f5dc`, `#ffffff`, `#2d3436`, `#e74c3c`).
  - **CSS Grid & Flexbox**: Maquetación responsiva con enfoque **Mobile First**.
  - **Pseudo-clases interactivas**: `:hover`, `:focus`, `:active`, `:checked`, `:valid`, `:invalid`, `:target`.
  - **Animaciones y Transiciones**: `@keyframes`, `transform: translateY()`, `transform: scale()`, `scroll-snap-type`.
- **Git & GitFlow**: Flujo de trabajo organizado por ramas (`main`, `develop`, `feature/base-css`, `feature/home`, `feature/catalogo`, `feature/nosotros`).

---

## 📂 Estructura de Archivos

```text
EcoMarket_ValentinaRojas/
├── css/
│   ├── main.css                # Reset, variables (:root), tipografía base
│   ├── layout.css              # Header, Footer, sistemas Grid y Flexbox responsivos
│   ├── components.css          # Tarjetas, botones, buscador, formulario, badges
│   └── animations.css          # Keyframes y transiciones interactivas
├── img/
│   ├── products/               # 20 imágenes de productos del catálogo
│   ├── icons/                  # Iconos SVG de principios ecológicos, avatares y redes
│   └── hero/                   # Imagen principal del Hero y mapa estilizado de ubicación
├── views/
│   ├── productos.html          # Vista de Catálogo (20 productos + paginación)
│   ├── sobre-nosotros.html     # Vista de Historia, Principios y Testimonios
│   └── contacto.html           # Vista de Contacto, Formulario (:valid/:invalid) y Mapa
├── index.html                  # Página de Inicio (Home)
└── README.md                   # Documentación del proyecto
```

---

## 🚀 Instrucciones de Visualización

1. **Clonar el repositorio:**
   ```bash
   git clone https://github.com/valent-gif/EcoMarket_ValentinaRojas.git
   cd EcoMarket_ValentinaRojas
   ```
2. **Abrir en el navegador:**
   - Abre directamente el archivo `index.html` en cualquier navegador web moderno (Chrome, Firefox, Edge, Safari), o
   - Usa la extensión **Live Server** en Visual Studio Code haciendo clic derecho sobre `index.html` → *Open with Live Server*.

---

## 📱 Diseño Responsivo (Mobile First)

| Punto de quiebre (Breakpoint) | Dispositivo | Distribución Catálogo | Distribución Destacados / Principios |
| :--- | :--- | :--- | :--- |
| `< 600px` | Móvil | 1 columna | 1 columna + Carrusel táctil `scroll-snap` |
| `>= 600px` | Tablet | 2 columnas | 2 columnas |
| `>= 900px / 1024px` | Escritorio | 4 columnas | 3 / 4 columnas + Layout horizontal |

---
## Link de la pagina web debe ser deplegada

El proyecto se encuentra alojado y funcionando en tiempo real en el siguiente enlace 
**[https://splendid-conkies-2ef162.netlify.app/](https://splendid-conkies-2ef162.netlify.app/)**[cite: 6]

---

##Capturads de Pantalla

### Vista Movil
<p align="center">
  <img src="img/captura_movil.jpeg" alt="Vista movil de Ecomarket" width="330">
</p>

### Vista Computador
<p align="center">
  <img src="img/captura-computador.jpeg" alt="Vista en computador de EcoMarket width="850">
</p>

---


**Autora:** Valentina Rojas Moratto — *Bucaramanga, Colombia (2026)*

