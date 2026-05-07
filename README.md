# Mi E-commerce - Proyecto Front-End

## Descripción
Sitio web de e-commerce con sección de productos, reseñas de clientes y formulario de contacto. Diseño responsivo que se adapta a celulares, tablets y computadoras de escritorio.

## Características
- **Sección de Productos**: 3 productos con imagen, descripción, precio y botón "Agregar al carrito"
- **Sección de Reseñas**: Testimonios de clientes organizados en grid
- **Formulario de Contacto**: Integrado con Formspree para recibir mensajes
- **Diseño Responsivo**: Adaptado para todos los tamaños de pantalla con Media Queries
- **Tipografía**: Usa Google Fonts (Roboto)
- **Navegación**: Estructura HTML semántica con header, main, sections y footer

## Tecnologías Usadas
- **HTML5**: Estructura semántica
- **CSS3**: Flexbox, CSS Grid, Media Queries
- **Google Fonts**: Roboto
- **Formspree**: Formulario de contacto

## Estructura del Proyecto
```
proyecto-final-ecommerce-tu-nombre/
├── index.html
├── styles.css
├── README.md
```

## Cómo Usar
1. Clonar o descargar el repositorio
2. Abrir `index.html` en un navegador
3. El sitio es completamente responsive — probá en celular y computadora

## Layouts Usados
- **Productos**: Flexbox con `flex-wrap: wrap` para adaptabilidad
- **Reseñas**: CSS Grid con 3 columnas (1 columna en móvil)
- **Formulario**: Flexbox centrado

## Media Queries
- **Móvil** (hasta 768px): Una columna para productos y reseñas
- **Tablet/Desktop** (768px+): Múltiples columnas

## Formulario
Los mensajes se envían a través de Formspree. Cada envío genera un email de confirmación.

## Autor
Angel Acuña

## Próximos Pasos
- Agregar más productos
- Implementar carrito de compras con JavaScript
- Mejorar validación del formulario
- Agregar animaciones con transiciones CSS
