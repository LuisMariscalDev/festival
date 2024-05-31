# Rave & EDM Festival

Este proyecto es un prototipo para el sitio web del Rave & EDM Festival. Fue creado como un ejercicio de aprendizaje para practicar y demostrar habilidades en HTML, Sass, JavaScript, npm y Gulp.

## Tabla de Contenidos
- [Demo](#demo)
- [Características](#características)
- [Tecnologías Utilizadas](#tecnologías-utilizadas)
- [Configuración](#configuración)
- [Uso](#uso)
- [Optimización de Rendimiento](#optimización-de-rendimiento)

## Demo
[https://festival-rave.netlify.app/](#)

## Características
- Diseño responsivo con mixins de Sass
- Navegación fija al desplazar
- Galería de imágenes con modal
- Sistema de boletos
- Efectos visuales y animaciones

## Tecnologías Utilizadas
- HTML5
- Sass (CSS preprocesado)
- JavaScript
- npm
- Gulp

## Configuración
Para configurar el proyecto localmente:

1. Clona el repositorio:
    ```sh
    git clone https://github.com/LuisMariscalDev/festival.git
    ```
2. Navega al directorio del proyecto:
    ```sh
    cd festival
    ```
3. Instala las dependencias:
    ```sh
    npm install
    ```

## Uso
Para iniciar el proyecto localmente:
1. Ejecuta Gulp para compilar Sass y otros archivos:
    ```sh
    npm run dev
    ```
2. Abre `index.html` en tu navegador.

## Optimización de Rendimiento
Este proyecto mejora el rendimiento web mediante el uso de diferentes formatos de imágenes, como AVIF y WebP, junto con JPG estándar. Aquí se explica cómo funciona:

- **AVIF y WebP**: Estos formatos de imagen son más eficientes y comprimen las imágenes mejor que JPG o PNG, lo que reduce el tamaño de los archivos y acelera el tiempo de carga de la página.
- **Carga perezosa**: Las imágenes se cargan solo cuando están en el campo de visión del usuario, mejorando la velocidad inicial de carga de la página.

### Ejemplo de Uso de Diferentes Formatos de Imagen
```html
<picture>
    <source srcset="dist/img/imagen_dj.avif" type="image/avif">
    <source srcset="dist/img/imagen_dj.webp" type="image/webp">
    <img width="300" height="200" loading="lazy" src="dist/img/imagen_dj.jpg" alt="sobre el festival">
</picture>
```
