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

Para que cumpla con los estandares de W3C se deben de corregir los siguientes errores, por lo tanto no cumple con los estandares de la página web.

### Usabilidad de la web
La página tiene una buena estructuración que permite ver claramente el contenido de la página con colores y tipografías legibles, este da a entender el concepto perfectamente de la página, el deiseño web es perfectamente navegable y con algunas transiciones para suavizar la navegación y hacerla más cómoda y no se encuentra díficultas en la navegación, en 
móvil las transiciones son más escasas y encontramos probemas con el navbar y el contenido no es navegable en condiciones y da problemas por lo tanto en móvil no es usable.

### En conclusión
Es importante cumplir los estanadares para poder tener la página bien organizada que sea fácil de usar tanto como para móvil com para escritorio, y sobre todo la importación de navegación intituiva esta ayuda mucho a que todos los tipos de usuarios puedan entender y llegar a utilizar la página .

## Pruebas de usabilidad y Velocidad
Vamos a utilizar una serie de herramientas para testear la app y ver los resultados que obtenemos en diferenestes secciones del contenido de la pagina web.
### WebPageTest

### PageSpeed Insights


### Lighthouse
- **Largest Contentful Paint (LCP):** El tiempo que targa en cargar el elemento más grande es de 8.9s
- **Interaction to Next Paint (INP):** La latencia con interación de elementos es de 130ms
- **Cumulative Layout Shift (CLS):** El contenido es muy estable 0.008
- **First Contentful Paint (FCP):** Tarda en mostrar el primer elemento visual 3.4s
- **First Input Delay (FID):** El tiempo de respuesta es rapido responde al momento, excepto en el muestero de imagenes.
- **Time to First Byte (TTFB):** El tiempo de de 114ms,es un tiempo de respuesta rápido

**Recomendaciones**
- El tiempo de carga incial es lento, probablemente debido al peso del contenido sobre todos de imagenes, comprimir imagenes para mejorar el rendimiento.
- Habilitar la compresión de texto.
- Optimizar el formato de las imágenes para hacerlas más pequeñas y mejorar el rendimmiento.
- Reducir el uso de javascript excesivo y cargar los elementos solo necesarios.
- Mejorar el minify de css quitando los comentarios innecesarios.








