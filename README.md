# Manual del Sitio Web - Ingeniero Estructural

¡Felicidades! Tu sitio web está listo. Este documento te guiará para ponerlo en línea y administrarlo.

## 📂 Archivos del Proyecto

Tu sitio se encuentra en: `D:\Google Drive 2\Progra\Mi pagina web`

*   **`index.html`**: El archivo principal. Aquí está todo el texto y la estructura.
*   **`css/estilos.css`**: Aquí están los colores, fuentes y diseños.
*   **`js/script.js`**: El "cerebro" que hace funcionar los filtros y botones.
*   **`imagenes/`**: Carpeta vacía donde DEBES poner tus fotos.
*   **`documentos/`**: Carpeta para guardar tus PDFs.

---

## 🚀 Cómo Desplegar (Poner en Internet)

La forma más fácil y gratuita es usando **Netlify** o **GitHub Pages**.

### Opción A: Netlify (Recomendado - Arrastrar y Soltar)
1.  Ve a [netlify.com](https://www.netlify.com/) y crea una cuenta gratuita.
2.  Una vez dentro, verás un panel que dice "Sites".
3.  Busca la zona que dice "Drag and drop your site output folder here".
4.  Arrastra toda la carpeta `Mi pagina web` desde tu computadora hacia esa zona en el navegador.
5.  ¡Listo! Netlify te dará un enlace (ej. `pedro-ingeniero.netlify.app`).

### Opción B: GitHub Pages
1.  Crea un repositorio en GitHub.
2.  Sube tus archivos.
3.  Ve a `Settings` > `Pages`.
4.  En "Source", selecciona `main` o `master` y guarda.

---

## ✏️ Guía de Edición (Sin ser programador)

Para editar el sitio, haz clic derecho en `index.html` y elige "Abrir con Bloc de Notas" (o mejor aún, usa **Visual Studio Code** si lo tienes).

### 1. Cambiar Textos
Busca el texto que quieres cambiar. Por ejemplo, para cambiar tu nombre:
*   Busca: `Juan Pérez`
*   Cámbialo por: `Tu Nombre Real`
*   ¡Guarda el archivo!

### 2. Cambiar Imágenes
El sitio tiene "placeholders" (cajas grises). Para poner tus fotos:
1.  Copia tu foto (ej. `mifoto.jpg`) a la carpeta `imagenes`.
2.  En el HTML, busca la zona de la imagen (ej. `img-placeholder`).
3.  Borra el `<div>` del placeholder y pon esto:
    ```html
    <img src="imagenes/mifoto.jpg" alt="Foto de perfil">
    ```

### 3. Agregar un Nuevo Proyecto
Ve a la sección `<!-- Galería -->` en el HTML. Copia todo un bloque de proyecto:

```html
<div class="portfolio-item" data-category="edificaciones">
    ... contenido ...
</div>
```
Pégalo abajo y cambia los textos.
*   Importante: Si es un puente, cambia `data-category="edificaciones"` por `data-category="puentes"`.

### 4. Modificar Enlaces de Contacto
Busca la sección del pie de página (footer) o contacto y cambia los enlaces:
*   `<a href="#">`: Cambia el `#` por tu enlace real (ej. `https://linkedin.com/in/tu-perfil`).

---

## 🎨 Personalización de Colores

Si quieres cambiar el azul oscuro por otro color:
1.  Abre `css/estilos.css`.
2.  Al principio verás esto:
    ```css
    :root {
        --primary: #0A2540;
        --secondary: #1E6F9F;
        ...
    }
    ```
3.  Cambia los códigos HEX (`#...`) por los que tú quieras.

---

## 🆘 Solución de Problemas

*   **¿No se ven las tildes?**
    Asegúrate de guardar el archivo con codificación **UTF-8**.
*   **¿Las imágenes no cargan?**
    Revisa que el nombre del archivo sea EXACTAMENTE igual (mayúsculas/minúsculas importan). `foto.JPG` no es lo mismo que `foto.jpg`.
*   **¿Los filtros no funcionan?**
    Asegúrate de no haber borrado las clases `data-filter` en los botones o `data-category` en los proyectos.

---
*Generado por tu Asistente de IA - 2026*
