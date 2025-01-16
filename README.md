# Testing-Producción
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
La página tiene una buena estructuración que permite ver claramente el contenido de la página con colores y tipografías legibles, este da a entender el concepto perfectamente de la página, el deiseño web es perfectamente navegable y con algunas transiciones para suavizar la navegación y hacerla más cómoda y no se encuentra díficultas en la navegación, en móvil las transiciones son más escasas y encontramos probemas con el navbar y el contenido no es navegable en condiciones y da problemas por lo tanto en móvil no es usable.

### En conclusión
Es importante cumplir los estanadares para poder tener la página bien organizada que sea fácil de usar tanto como para móvil com para escritorio, y sobre todo la importación de navegación intituiva esta ayuda mucho a que todos los tipos de usuarios puedan entender y llegar a utilizar la página la página en escritorio si que es usable
pero para móvil considero que tiene defectos que no debería de tener, además de algunos fallitos que tampoco deberia de tener por lo tanto no cumple los estándares como tal pero una buena página a nivel de usabilidad en escritorio.

## Pruebas de usabilidad y Velocidad
Vamos a utilizar una serie de herramientas para testear la app y ver los resultados que obtenemos en diferenestes secciones del contenido de la pagina web.
### WebPageTest
Vamos a realizar test, al home en modo escritorio en firefox y google.
**Test en Firefox**
![imagen](https://github.com/user-attachments/assets/f9a4e349-da99-4962-a792-74b5b8dde0f8)


**Test en Google**
![imagen](https://github.com/user-attachments/assets/23677674-b5ff-49a8-87c9-2db4150df5f5)
Como apreciamos las estadisticas son totalmente diferentes en cuanto a terminos de rendimeinto, en firefox rinde bastante mejor es un rendimiento normal pero mejorable según las estadisiticas mostradas en las imagenes, también tener en cuenta que son ubicaciones diferentes y motores de navegación diferentes.

### PageSpeed Insights
**Pagina Incial**
![imagen](https://github.com/user-attachments/assets/732065c5-a265-4f4c-ab54-6635dc1ea7e2)
![imagen](https://github.com/user-attachments/assets/9ca872de-52f6-4688-bfef-ad5b4fa3a5a2)

Podemos observar que el rendimiento es mejor en el modo escritorio que en el de móvil, principalmente porque el renderizado en el móvil es mucho mas lento que en el de escritorio, también se recomienda reducir los recursos de JS para mejor el elmento y renderizar el elemento más grande de la página para mejorar su rendimiento ya que relentiza mucho el muestreo de información sobre todo en móvil, codificar las imagenes y optimizarlas en otro formato para mejorar el rendimeinto.


**Listado de Animes**


**Anime y Episodios**


### Lighthouse
Vamos a realizar test de escritorio y movil.
**Test en Escritorio**
![imagen](https://github.com/user-attachments/assets/4621ae96-3069-4fef-a46a-15418c36cad6)
![imagen](https://github.com/user-attachments/assets/92c8d35d-b3c3-4d3a-8d8d-84d8a14aef84)

- **Largest Contentful Paint (LCP):** El tiempo que targa en cargar el elemento más grande es de 1s
- **Interaction to Next Paint (INP):** Tiene una interacción entre páginas de 90ms
- **Cumulative Layout Shift (CLS):** El contenido es muy estable 0.017
- **First Contentful Paint (FCP):** Tarda en mostrar el primer elemento visual 0.7s
- **First Input Delay (FID):** No tiene bloquo ni diley ninguno.
- **Time to First Byte (TTFB):** El tiempo de de 330ms ,es un tiempo de respuesta lento.

Algunas **recomendaciones** serian solucuionar la carga de las tipografías ya que esta retrasa la carca en 270ms, y reducir el código JS a la hora del despligue, cambiar el formato de las imagenes tambien es útil para liberar el peso.

En total la página tiene un puntuación de 98 en performance que esta muy bien la verdad, en navegación entre páginas si que encontramos algo de perdida de puntuación.

### Ghost Inspector







