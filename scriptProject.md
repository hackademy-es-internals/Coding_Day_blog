# SCRIPT PROYECTO Lorem Blog 
## Setup: 

#### Tecnologias usadas: 
- ##### HTML 5 
- ##### CSS 
- ##### Framework front-end Bootstrap 5 
- ##### CDN libreria Bootstrap iconos

#### Inicio

1. Primer paso cojer starter template desde la pagina web: https://getbootstrap.com/docs/5.1/getting-started/introduction/ borrando los varios comentarios y dejando las metas informaciones incluidas por defecto 

2. le doy un titulo a la pagina atraves de la meta info title dentro del head : Blog

3. hago un import de la CDN de los inconos de bootstrap desde la pagina: https://icons.getbootstrap.com/, probablemente los necisitaré mas adelante 

4. hago una referencia en las meta info con una hoja de estilo personal que llamo main.css

5. hago un import de una fuente de texto desde Google fonts: @import url('https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,100;0,200;0,300;0,500;0,600;0,700;1,100;1,200;1,400;1,600;1,700&display=swap');
eligo de google font Montserrat ancho 100, 200, 300, 500, 600, 700

6. ultimo paso de setup, en la hoja main.css,uso el selector universal * para usar esa fuente en toda la pagina 

### Inicio Diseño 

1. quiero un contenedor que coja el 100% del altura del dispositivo, de doy un tag semantico header para indicale que será el encabezado de la pagina 

2. dentro de este header quiero ponerle una bara de navegacion superior arriba del todo y una bara de nagavacion inferior bajo de la primera 

3. uso container fluid del grid system de bootstrap para cojer el ancho total del dispositivo, a esta le agrego una clase custum "head" para estar mas seguro que vaya posicionandose donde yo quiero 

4. clase head quiero que tenga estas caracteristicas:
* alto el 70% del dispositivo 
* ancho el 100% del dispositivo 
* una imagen de fondo centrada 

.head {
  height: 70vh; 
  min-height: 500px; 
  width: 100%; o  
  background-image:linear-gradient(rgba(65, 65, 65, 0.749), rgba(0, 0, 0, 0.434)), url('./media/head01.jpg'); 
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}

5. una vez que la imagen este centrada mira la version movil, desde la version movil quiero estas caracteristicas: 
* alto el 100% del dispositivo 
* ancho el el 100% del dispositivo 
* misma imagen de fondo 

creo una media query que, por tamaño de pantalla inferior a 767.98px, coja las siguente clase: 

@media (max-width: 767.98px) {
  .head {
    height: 100vh;
    min-height: 500px;
    width: 100%;
    background-image:linear-gradient(rgba(65, 65, 65, 0.749), rgba(0, 0, 0, 0.434)), url('./media/head01.jpg');
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
  }
}

comprobamos que el emcabezado este listo y seguimos con la barra de navegacion 


### Navbar 


 


