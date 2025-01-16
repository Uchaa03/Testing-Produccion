# Testing-Producciom
#### Adrián Ucha Sousa / Diseño de interfaces WEB

Hoy vamos a realizar un testing  de producción sobre la página de mi compañero Pablo Barrera, y su proyecto de **Shibuya-Station**.

## 1. Evaluación de estandares y navegación.
### Evaluación de estructura semántica HTML y CSS
Realizamos la validación en (poner pagina de validación), y al realizar en algunas de las páginas para ver la estrucutración podemos encotrar algunas cosas que no cumplen con los estandares 
#### Página de inicio
Principalmente presenta algunos errores y warnings en el HTML:
1. Presenta etiquetas `main` anidados dentro de otros `main` que no es correcto solo debería de tener uno.
2. Tambien pasa lo mismo con el `footer` tiene mas de anidado.
3. Tienes alguna alerta por uso excesivo de `h1` cosa que puede empeorar la accesibilidad y el posicionamiento SEO de la página.
4. Y tambien alerta de que se a usado el elemento `section` para agrupar contenido sin darle encabezado alguno ni nada, esto puede ocasionar los mismos problemas que la alerta anterior.

