##  meta viwport
wiewport: la parte visible de navegador

esta es una etiqueta de metadatos que te ayudará a configurar tu website para que sea visible en dispositivos de menor tamaño. 

```html
<meta name="viewport" content="width=device-width, initial-scale=1">
```

Uno de los objetivos principales al usar esta etiqueta será que conserves la legibilidad de tu página web, al variar el escalado de tus contenidos.

`width=device-width`para que se adapte según la pantalla del dispositivo

`initial-scale=1.0
` para indicar el escalado según el dispositivo (1 = 100% del zoom)

## Medidas relativas útiles en Responsive Design

### pixel:
 unidad de color minima dentro de medios digitales 

### porcentaje:
 longitud referente al tamaño del padre

### em

unidad relativa al tamaño de fuente especificada mas cercana

```html
<nav> font-zise: 16px;
  <ul> font-size: 2em, 32px;
    <li> font-size: 1em, 32px;
    <a href=""> hola </a> font-size: .5em; 16px; padding: 2em; 32px;
    <li>
  <ul>
<nav> 
```
### rem

unidad relativa al tamaño de fuente especificada en el ancestro mas lejano (html o body)
```html
<!DOCTYPE html>
<html lang="en">font-size: 32px;
<head>
</head>
<body>font-size: 16px;
  <ul>font-size: 2rem; 64px
    <li>font-size: 1rem; 32px;
      <a href=""></a> font-size:.5rem; 16px;
    </li>
  </ul>
</body>
</html>
```
### vw / vh

unidad relativa porcentual con respecto al viweport 

100vw = 1024 viewport

## media Queries
gracias a este modulo exite responsive desing

mudulo CSS3S que permite adaptar la representacion del contenido a caracteristicas del dispositivo

```css
@media media type and (condición) { }
```
se compone de un media type y una o mas condiciones

#### ejemplo

```css
@media screen type and (max-width: 768px) { }
```
todas las pantallas con un ancho inferior o igual a 768px cumplen con esta funcion
```css
@media screen type and (max-width: 768px) and (min-width: 480px) { }
```
todas las pantallas con un ancho de 480px hasta 768px cumplen con esta funcion

### Mobile Firts

```css
@media screen type and (max-width: 320px) { }
@media screen type and (max-width: 480px) { }
@media screen type and (max-width: 768px) { }
@media screen type and (max-width: 1024px) { }
```
usa min-width (min-width = desde)
### Desktop Firts

```css
@media screen type and (min-width: 1024px) { }
@media screen type and (min-width: 768px) { }
@media screen type and (min-width: 480px) { }
@media screen type and (min-width: 320px) { }
```
usa max-width (max-width = hasta)

## Breakpoints estandarizados
 que debemos de tener en cuenta:

#### Móviles:
  entre 320 y 480 píxeles. 
#### Tablets:
 entre 768 y 1024 píxeles.

#### Pantallas grandes:
 más de 1024 píxeles o más.

 se utlizan mas que todo en la hoja de estilos

  Por otro lado, para hacer esto posible, aprenderás a aplicar las etiquetas de max-width y flex- wrap; éstas también te ayudarán a evitar que tu usuario necesite navegar la página de forma horizontal, pues la información se organizará en forma vertical para facilitar la experiencia.