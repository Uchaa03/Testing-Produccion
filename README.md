# Testing-Producciom
#### Adrián Ucha Sousa / Diseño de interfaces WEB

Hoy vamos a realizar un testing de producción sobre la página de mi compañero Pablo Barrera, y su proyecto de **Shibuya-Station**.

## 1. Evaluación de estándares y navegación.
Vamos a realizar validaciones de estándares para ver si cumple con los estándares de W3C, que son los que debe cumplir una página para que esta técnicamente esté bien estructurada y correcta.
Realizamos la validación en (poner página de validación), y al realizar en algunas de las páginas para ver la estructuración podemos encontrar algunas cosas que no cumplen con los estándares.

### Validación de HTML
**Errores en el HTML:**
1. **Error**: Presenta etiquetas `main` anidados dentro de otros `main`, lo cual no es correcto. Solo debería haber un único `main`.
2. **Error**: Múltiples `footer` anidados, lo cual también es incorrecto.
3. **Error**: Existen `section` que no tienen ningún título, lo que puede provocar dificultades de accesibilidad y SEO. Se debe usar `div` en estos casos.
4. **Error**: `label` no enlazadas a ningún **id** de elementos de formularios como `input`.
5. **Error**: `p` dentro de `button`, lo cual no es correcto.
6. **Error**: `span` dentro de `figure`, lo correcto es utilizar `figcaption`.

**Advertencias en el HTML:**
1. **Advertencia**: Uso excesivo de `h1`, lo que puede empeorar la accesibilidad y el posicionamiento SEO de la página.
2. **Advertencia**: Uso de `section` para agrupar contenido sin encabezado alguno, lo que puede causar problemas similares a la advertencia anterior.

### Validación de CSS
Realizamos la validación del CSS en (poner enlace de página).

**Errores en el CSS:**
1. **Error**: `.hamburger-menu__toggle` - Propiedad no válida: `color`. Error de análisis sintáctico `--color-secondary`.
2. **Error**: `.home__title` - La propiedad `font-display` no existe: `swap`.
3. **Error**: `.home__button` - Error de análisis sintáctico `var();`.
4. **Error**: `.home__button` - Error de análisis sintáctico `cursor: pointer;`.
5. **Error**: `.home__button` - Error de análisis sintáctico `transition: transform 0.2s ease, box-shadow 0.2s ease;`.
6. **Error**: `.profile__date` - Propiedad no válida: `color`. Error de análisis sintáctico `--color-text`.

**Advertencias en el CSS:**
1. **Advertencia**: Las hojas de estilo importadas no se comprueban en los modos de entrada directa y carga de archivo.
2. **Advertencia**: Debido a su naturaleza dinámica, las variables CSS actualmente no se verifican estáticamente.

Para que cumpla con los estandares de W3C se deben de corregir los siguientes errores, por lo tanto no cumple con los estandares de la página web

