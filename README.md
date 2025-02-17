# Testing-Producción
#### Adrián Ucha Sousa / Diseño de interfaces WEB

Hoy vamos a realizar un testing de producción sobre la página de mi compañero Pablo Barrera, y su proyecto de **Shibuya-Station**.

## 1. Evaluación de estándares y navegación.
Vamos a realizar validaciones de estándares para ver si cumple con los estándares de W3C, que son los que debe cumplir una página para que esté técnicamente bien estructurada y correcta.
Realizamos la validación en (poner página de validación), y al realizar en algunas de las páginas para ver la estructuración podemos encontrar algunas cosas que no cumplen con los estándares.

### Validación de HTML
**Errores en el HTML:**
1. **Error**: Presenta etiquetas `main` anidadas dentro de otros `main`, lo cual no es correcto. Solo debería haber un único `main`.
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

Para que cumpla con los estándares de W3C se deben corregir los siguientes errores, por lo tanto, no cumple con los estándares de la página web.

### Usabilidad de la web
La página tiene una buena estructuración que permite ver claramente el contenido de la página con colores y tipografías legibles. Esto da a entender el concepto perfectamente de la página. El diseño web es perfectamente navegable y con algunas transiciones para suavizar la navegación y hacerla más cómoda. No se encuentran dificultades en la navegación, pero en móvil las transiciones son más escasas y encontramos problemas con el navbar y el contenido no es navegable en condiciones, lo que da problemas. Por lo tanto, en móvil no es usable.

### En conclusión
Es importante cumplir los estándares para poder tener la página bien organizada y que sea fácil de usar tanto para móvil como para escritorio. La importación de navegación intuitiva ayuda mucho a que todos los tipos de usuarios puedan entender y llegar a utilizar la página. La página en escritorio es usable, pero para móvil considero que tiene defectos que no debería tener, además de algunos fallos que tampoco debería tener. Por lo tanto, no cumple los estándares como tal, pero es una buena página a nivel de usabilidad en escritorio.

## Pruebas de usabilidad y velocidad
Vamos a utilizar una serie de herramientas para testear la app y ver los resultados que obtenemos en diferentes secciones del contenido de la página web.

### WebPageTest
Vamos a realizar test, al home en modo escritorio en Firefox y Google.
**Test en Firefox**
![imagen](https://github.com/user-attachments/assets/f9a4e349-da99-4962-a792-74b5b8dde0f8)

**Test en Google**
![imagen](https://github.com/user-attachments/assets/23677674-b5ff-49a8-87c9-2db4150df5f5)
Como apreciamos, las estadísticas son totalmente diferentes en cuanto a términos de rendimiento. En Firefox rinde bastante mejor; es un rendimiento normal pero mejorable según las estadísticas mostradas en las imágenes. También tener en cuenta que son ubicaciones diferentes y motores de navegación diferentes.

**Test en móvil lista**
![imagen](https://github.com/user-attachments/assets/710bdfdd-762f-4887-b905-9e2b0ff8ee06)

**Test en móvil producto**
![imagen](https://github.com/user-attachments/assets/10da5deb-0a6c-47a1-9f3a-b4e6b2d26f14)
Las páginas son usables, pero encuentran algunos problemas que requieren modificaciones ya que tienen un tiempo de respuesta largo. Eso genera problemas en la fluidez de la navegación entre secciones y páginas.

**Test en escritorio lista**
![imagen](https://github.com/user-attachments/assets/d1e6a5df-3bc4-4b68-a1b5-8e042a6aab4c)
La página tiene algún problema de usabilidad igual que la de los móviles, pero en cuanto al rendimiento es mucho mejor que en móvil, por lo tanto, la navegación es bastante mejor que en móvil.

**Test en escritorio producto**
![imagen](https://github.com/user-attachments/assets/7cfac66b-ac36-4af5-9594-5dbe0f3fda83)
Esta tiene los mismos problemas y un rendimiento similar al de móvil.

### PageSpeed Insights
**Página Inicial**
![imagen](https://github.com/user-attachments/assets/732065c5-a265-4f4c-ab54-6635dc1ea7e2)
![imagen](https://github.com/user-attachments/assets/9ca872de-52f6-4688-bfef-ad5b4fa3a5a2)
Podemos observar que el rendimiento es mejor en el modo escritorio que en el de móvil, principalmente porque el renderizado en el móvil es mucho más lento que en el de escritorio. También se recomienda reducir los recursos de JS para mejorar el elemento y renderizar el elemento más grande de la página para mejorar su rendimiento ya que ralentiza mucho el muestreo de información, sobre todo en móvil. Codificar las imágenes y optimizarlas en otro formato para mejorar el rendimiento.

**Listado de Animes**
![imagen](https://github.com/user-attachments/assets/95c272d0-75cb-4144-b810-5a69aba2c595)
![imagen](https://github.com/user-attachments/assets/0dca121c-d6f8-4609-bd9c-0b5c134a725c)
Aquí, podemos observar muchos más problemas de rendimiento, sobre todo en móvil, debido a que no está del todo bien creado el diseño responsive. El rendimiento sufre cambios de diseño importantes y la carga es más lenta debido a la gran cantidad de contenido que tiene. Eso hace que en móvil sea peor todavía.

**Manga y Episodios**
![imagen](https://github.com/user-attachments/assets/b99c4b13-742b-4dc0-b268-a846997d7943)
![imagen](https://github.com/user-attachments/assets/7c17d17c-815b-4a50-8dae-58d529e01fa1)
Si analizamos un manga en concreto, podemos ver que el rendimiento en este caso es mucho peor en escritorio que en móvil ya que se muestra mucho más contenido y está muy mal optimizado. El mayor problema que tiene es el renderizado de tanto contenido. El tiempo de respuesta es muy largo, además de los problemas comentados anteriormente en otras secciones.

### Lighthouse
Vamos a realizar test de escritorio y móvil.
**Test en Escritorio**
![imagen](https://github.com/user-attachments/assets/4621ae96-3069-4fef-a46a-15418c36cad6)
![imagen](https://github.com/user-attachments/assets/92c8d35d-b3c3-4d3a-8d8d-84d8a14aef84)

- **Largest Contentful Paint (LCP):** El tiempo que tarda en cargar el elemento más grande es de 1s.
- **Interaction to Next Paint (INP):** Tiene una interacción entre páginas de 90ms.
- **Cumulative Layout Shift (CLS):** El contenido es muy estable, 0.017.
- **First Contentful Paint (FCP):** Tarda en mostrar el primer elemento visual 0.7s.
- **First Input Delay (FID):** No tiene bloqueo ni delay alguno.
- **Time to First Byte (TTFB):** El tiempo es de 330ms, es un tiempo de respuesta lento.

Algunas **recomendaciones** serían solucionar la carga de las tipografías ya que esta retrasa la carga en 270ms, y reducir el código JS a la hora del despliegue. Cambiar el formato de las imágenes también es útil para liberar el peso.

En total, la página tiene una puntuación de 98 en performance, lo cual está muy bien. En navegación entre páginas sí que encontramos algo de pérdida de puntuación.

### Ghost Inspector
![imagen](https://github.com/user-attachments/assets/f5b564e6-bfb4-4089-be2c-b5bd9ecda2a9)
Nos registramos y instalamos la extensión. Entonces, ahora te vas a la página principal y realizas la grabación de la navegación.
![imagen](https://github.com/user-attachments/assets/84619cff-9ddc-4d90-8a8c-f5b45b58973c)
Como se puede ver, el test pasó correctamente y sin problemas.
![Video de la prueba](https://github.com/user-attachments/assets/9a5257cf-c26f-4f7c-8c27-715a49f13dd9)






