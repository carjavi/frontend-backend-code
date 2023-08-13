<p align="center"><img src="https://raw.githubusercontent.com/carjavi/frontend-backend-code/master/img/frontend_backend.jpg" height="250" alt=" " /></p>
<br>
<h1 align="center">Frontend Backend Code</h1> 
<h4 align="right">Oct 22</h4>

<img src="https://img.shields.io/badge/OS-Linux%20GNU-yellowgreen">
<img src="https://img.shields.io/badge/OS-Windows%2011-blue">

<br>

# Launching the browser in 'Full screen' mode 

> :memo: **Note:** chromium open source of Chrome

command: <br>
```
chromium-browser --[mode] http://www.example.com
chromium-browser --[mode] http://localhost:8080
chromium-browser --[mode] http://192.168.X.X:8080
chromium-browser -start-maximized
```

**Application Mode**: ```chromium-browser --app```. El navegador se inicia sin mostrar ninguna barra de herramientas.

**Full-screen mode**: ```chromium-browser --start-fullscreen```.El navegador se inicia en app. pero ampliado a pantalla completa. Puede presionar la tecla <kbd>F11</kbd> para salir del modo de pantalla completa.

Kiosk mode: ```chromium-browser --kiosk```. El navegador se inicia en modo de pantalla completa, pero no responde a la tecla F11 ni a ningún comando para que cambie de tarea. La única forma de salir de la ventana es <kbd>Alt+Tab</kbd> out o <kbd>Alt+F4</kbd> para cerrar la ventana por completo.

sample:
```
var http = require("http");

var srv = http.createServer(...);
srv.listen(8000, ExecuteChromium);

function ExecuteChromium() {
    exec("chromium-browser --kiosk http://example.com", function(error, stdout, stderr) {
        console.log("stdout: " + stdout);
        console.log("stderr: " + stderr);
        if (error !== null) {
            console.log("exec errror: " + error);
        }
    });
}
```
## Launching the browser in SSH 
Se debe indicar que se iniciara el browser en pantalla predeterminada. ***DISPLAY=:0*** <br>
Sample:
```
DISPLAY=:0 chromium-browser --kiosk --app=localhost:8080
DISPLAY=:0 chromium-browser http://localhost:8080
```
## 
chrome


# CCS

 – Imagen responsive de ancho completo
Para obtener imágenes responsive de ancho completo, lo único que hay que hacer es configurar el ancho del DIV contenedor de la imagen a 100% o dejarlo sin ancho.

Y luego a la etiqueta de la imagen colocarle un ancho del 100%.

En CSS:
```
?
.container {
width: 100%;
}
En HTML:

?
<div class="container">
<img  src="image01.jpg" width="100%" />
</div>
```
## CSS Padding

El relleno se utiliza para crear espacio alrededor del contenido de un elemento, dentro de los bordes definidos.

```
<style>
div {
  border: 1px solid black;
  background-color: lightblue;
  padding-top: 50px;
  padding-right: 30px;
  padding-bottom: 50px;
  padding-left: 80px;
}
</style>
```

## CSS Grid Layout Module

```
display: grid / inline-grid;
```

<br>
<br>

---
Copyright &copy; 2022 [carjavi](https://github.com/carjavi). <br>
```www.instintodigital.net``` <br>
carjavi@hotmail.com <br>
<p align="center">
    <a href="https://instintodigital.net/" target="_blank"><img src="https://raw.githubusercontent.com/carjavi/frontend-backend-code/master/img/developer.png" height="100" alt="www.instintodigital.net"></a>
</p>
