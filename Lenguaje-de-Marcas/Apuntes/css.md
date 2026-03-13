# Apuntes Extendidos de CSS: Guía Completa

## 1. Introducción a CSS

### 1.1. ¿Qué es CSS?
CSS (Cascading Style Sheets), u Hojas de Estilo en Cascada, es un lenguaje de diseño gráfico que se utiliza para definir y crear la presentación de un documento escrito en HTML o XML. Es el encargado de controlar colores, fuentes, espaciado, distribución y, en general, el aspecto visual de una página web, separando así el contenido (HTML) de la presentación (CSS).

### 1.2. ¿Por qué usamos CSS?
- **Separación de contenido y diseño**: Permite que el HTML se enfoque en la estructura semántica del contenido, mientras el CSS maneja cómo se ve.
- **Mantenibilidad**: Al cambiar una sola línea en un archivo CSS, se puede modificar el estilo de cientos de páginas que enlacen a él.
- **Reutilización**: Un mismo archivo CSS puede ser usado por múltiples páginas, garantizando una coherencia visual en todo el sitio web.
- **Flexibilidad y eficiencia**: Ofrece herramientas mucho más potentes que las antiguas etiquetas HTML para el formato (como `<font>`), permitiendo diseños complejos y adaptables.

## 2. Formas de Insertar CSS en HTML

Existen tres métodos principales para aplicar estilos CSS a un documento HTML:

### 2.1. CSS Externo (Recomendado)
Consiste en crear un archivo separado con extensión `.css` y vincularlo desde el documento HTML. Esta es la mejor práctica, ya que mantiene los estilos completamente separados del contenido y permite la reutilización en múltiples páginas.

**Ejemplo:**
```html
<!-- Dentro de la sección <head> del HTML -->
<head>
  <link rel="stylesheet" href="styles.css">
</head>
