# Testing-Producciom
#### Adrián Ucha Sousa / Diseño de interfaces WEB

Hoy vamos a realizar un testing  de producción sobre la página de mi compañero Pablo Barrera, y su proyecto de **Shibuya-Station**.

## 1. Evaluación de estandares y navegación.
Vamos a realizar validaciones de estandares para ver si cumple con los estandares de W3C, que son los que debe cumplir una página para que esta técnicmaente bien estructurada y correcta.
### Evaluación de estructura semántica HTML y CSS
Realizamos la validación en (poner pagina de validación), y al realizar en algunas de las páginas para ver la estrucutración podemos encotrar algunas cosas que no cumplen con los estandares 

**Principalmente presenta algunos errores y warnings en el HTML:**
1. Presenta etiquetas `main` anidados dentro de otros `main` que no es correcto solo debería de tener uno.
2. Tambien pasa lo mismo con el `footer` tiene mas de anidado.
3. Existen `section` que no tiene ningun título por lo tanto este esto puede provocar dificultades de accesibilidad, SEO..
se debe usar div en estos casos.
4. Error en las `label` de login y registro debido a que estas no estan enlazadas a ningun **id** de cualquiera de los elementos de los formularios como por ejemplo un `input`.
5. Ecnontramos `p` dentro de los `button` cosa que no es correcta.
6. Utilizaxión de `span` dentro de `figure` no es correcto, lo correcto es utilizar `figcaption`.
7. Tiene alguna alerta por uso excesivo de `h1` cosa que puede empeorar la accesibilidad y el posicionamiento SEO de la página.
8. Y tambien alerta de que se a usado el elemento `section` para agrupar contenido sin darle encabezado alguno ni nada, esto puede ocasionar los mismos problemas que la alerta anterior.

