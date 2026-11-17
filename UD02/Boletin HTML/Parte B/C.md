# Parte C. Práctica 2. Las estaciones (enlaces e imágenes)  

## Codigo

## Estaciones

```html
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="utf-8">
  <title>Estaciones</title>
</head>
<body>
  <h1>ESTACIONES</h1>

  <h2>Primavera</h2>
  <a href="primavera.html">
    <img src="imagenes/primavera.jpg" alt="Paisaje de primavera"
         style="width: 300px; height: 300px; border: 5px solid green;">
  </a>

  <h2>Verano</h2>
  <a href="verano.html">
    <img src="imagenes/verano.jpg" alt="Paisaje de verano"
         style="width: 300px; height: 300px; border: 5px solid orange;">
  </a>

  <h2>Otoño</h2>
  <a href="otono.html">
    <img src="imagenes/otono.jpg" alt="Paisaje de otoño"
         style="width: 300px; height: 300px; border: 5px solid brown;">
  </a>

  <h2>Invierno</h2>
  <a href="invierno.html">
    <img src="imagenes/invierno.jpg" alt="Paisaje de invierno"
         style="width: 300px; height: 300px; border: 5px solid blue;">
  </a>
</body>
</html>
```

## Primavera

```html
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="utf-8">
  <title>Primavera</title>
</head>
<body>
  <h1>Primavera</h1>

  <img src="imagenes/primavera.jpg" alt="Paisaje de primavera"
       style="width: 600px; height: 600px; border: 5px solid green;">

  <p><a href="estaciones.html">Volver a la página principal</a></p>
</body>
</html>
```

## Verano

```html
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="utf-8">
  <title>Verano</title>
</head>
<body>
  <h1>Verano</h1>

  <img src="imagenes/verano.jpg" alt="Paisaje de verano"
       style="width: 600px; height: 600px; border: 5px solid orange;">

  <p><a href="estaciones.html">Volver a la página principal</a></p>
</body>
</html>
```

## Otoño

```html
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="utf-8">
  <title>Otoño</title>
</head>
<body>
  <h1>Otoño</h1>

  <img src="imagenes/otono.jpg" alt="Paisaje de otoño"
       style="width: 600px; height: 600px; border: 5px solid brown;">

  <p><a href="estaciones.html">Volver a la página principal</a></p>
</body>
</html>
```

## Invierno

```html
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="utf-8">
  <title>Invierno</title>
</head>
<body>
  <h1>Invierno</h1>

  <img src="imagenes/invierno.jpg" alt="Paisaje de invierno"
       style="width: 600px; height: 600px; border: 5px solid blue;">

  <p><a href="estaciones.html">Volver a la página principal</a></p>
</body>
</html>
```

## Reflexión

**1. ¿Qué ruta relativa usará estaciones.html para cargar primavera.jpg?**
`imagenes/primavera.jpg`, porque estaciones.html está en la carpeta principal y la imagen está dentro de la subcarpeta `imagenes`.

**2. ¿Qué pasaría si movieras las páginas de cada estación a una carpeta paginas/?**
Dejarían de funcionar varias rutas y habría que cambiarlas:
- En estaciones.html, los enlaces pasarían a ser `paginas/primavera.html`, etc.
- Dentro de cada página de estación, la imagen pasaría a ser `../imagenes/primavera.jpg` (`..` = subir una carpeta).
- El enlace de vuelta pasaría a ser `../estaciones.html`.

**3. Si las fotos miden 600 × 600 y deben verse a 300 × 300, ¿las recortas o cambias el tamaño con HTML/CSS?**
Cambio el tamaño con HTML/CSS (`style="width: 300px; height: 300px;"`), sin recortar la imagen. Así uso el mismo archivo en las dos páginas.
