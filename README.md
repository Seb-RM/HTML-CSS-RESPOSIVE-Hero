# Hero Section Responsivo 🚀

![Responsive Design](https://img.shields.io/badge/Responsive-Yes-success?style=flat&logo=web-components)

Un proyecto demostrativo de diseño web responsivo implementando mejores prácticas modernas de desarrollo frontend.

## 📋 Descripción
Este proyecto consiste en un hero section completamente responsivo que se adapta a diferentes dispositivos y tamaños de pantalla. Desarrollado como parte de un ejercicio práctico de Responsive Web Design (RWD), implementa diversas técnicas y recursos aprendidos:

- Uso de media queries avanzadas
- Optimización de imágenes responsivas
- Tipografía escalable
- Diseño flexible basado en breakpoints estándar

## ✨ Características Principales
- **Imagen de fondo responsiva:**  
  Uso de `<picture>` con múltiples formatos (AVIF, WebP, PNG) y resoluciones
- **Navegación adaptable:**  
  Barra de navegación con efectos hover y fondo semitransparente
- **Tipografía responsiva:**  
  Textos que escalan según el tamaño de pantalla
- **Botones flexibles:**  
  Sistema de botones que se adaptan al viewport
- **Optimización de performance:**  
  Uso de gradientes CSS y carga condicional de recursos

## 🧠 Temas Abarcados
1. Fundamentos de Responsive Web Design (RWD)
2. Implementación de Media Queries con:
   - `min-width` y `max-width`
   - Operadores lógicos (`and`)
   - Orientación del dispositivo
3. Breakpoints estándar para diferentes dispositivos
4. Técnicas de optimización de imágenes:
   - Formatos modernos (AVIF, WebP)
   - Art direction con `<picture>`
   - Uso de `srcset` y `sizes`
5. Diseño fluido con:
   - Unidades relativas
   - Flexbox
   - Margenes responsivos

## 🛠 Tecnologías Utilizadas
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)

- **HTML5:** Semántica moderna y elementos embebidos
- **CSS3:**
  - Media Queries (`@media`)
  - Flexbox para layouts
  - Gradientes lineales
  - Unidades relativas (vw, %)
  - Pseudoclases de hover
  - Propiedades de transición

## 📦 Instalación
1. Clona el repositorio:
```bash
git clone [URL_DEL_REPOSITORIO]
```
2. Abre el archivo index.html en tu navegador

3. Ajustar el tamaño de la ventana del navegador para ver la adaptabilidad del diseño.

## 🎨 Detalles de Implementación
- **Breakpoints Principales**
    - 576px: Versión móvil (base)
    - 800px: Tablets pequeñas
    - 900px: Tablets grandes/escritorio
    -992px: Escritorio HD

- **Optimización de Imágenes**
```html
<picture>
  <source media="(min-width: 900px)" 
          srcset="img/Prototype.avif 1x, img/Prototype.webp 1x, img/Prototype.png 1x">
  <source srcset="img/Prototype-600.avif 1x, img/Prototype-600.webp 1x, img/Prototype-600.png 1x">
  <img src="img/Prototype-600.png" alt="Imagen de Fondo">
</picture>
```
- **Sistema Responsivo de Tipografía**
```css
.hero-content h1 {
  font-size: 30px; /* Mobile */
}

@media (min-width: 576px) {
  .hero-content h1 {
    font-size: 60px; /* Desktop */
  }
}
```
## 📌 Consideraciones Adicionales
- Las imágenes incluidas son solo demostrativas

- Se utilizan breakpoints estándar pero pueden ajustarse según necesidades

- El diseño prioriza mobile-first con mejoras progresivas para pantallas grandes

- Se recomienda utilizar herramientas como DevTools en el navegador para ver el diseño en diferentes resoluciones.