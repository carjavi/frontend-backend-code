<p align="center"><img src="https://raw.githubusercontent.com/carjavi/frontend-backend-code/master/img/markdown_logo.png" height="100" alt=" " /></p>
<br>
<h1 align="center">Frontend Backend Code</h1> 
<h4 align="right">Oct 22</h4>

<img src="https://img.shields.io/badge/OS-Linux%20GNU-yellowgreen">
<img src="https://img.shields.io/badge/OS-Windows%2011-blue">


# Launching the browser in 'Full screen' mode

command: <br>
```chromium-browser --[mode] http://example.com``` <br>
```chromium-browser --[mode] localhost:4000```

**Application Mode**: ```chromium-browser --app```. El navegador se inicia sin mostrar ninguna barra de herramientas.

**Full-screen mode**: ```chromium-browser --start-fullscreen```.El navegador se inicia en app. pero ampliado a pantalla completa. Puede presionar la tecla F11 para salir del modo de pantalla completa.

Kiosk mode: ```chromium-browser --kiosk```. El navegador se inicia en modo de pantalla completa, pero no responde a la tecla F11 ni a ningún comando para que cambie de tarea.

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



---
Copyright &copy; 2022 [carjavi](https://github.com/carjavi). <br>
```www.instintodigital.net``` <br>
carjavi@hotmail.com <br>
<p align="center">
    <a href="https://instintodigital.net/" target="_blank"><img src="https://raw.githubusercontent.com/carjavi/frontend-backend-code/master/img/developer.png" height="100" alt="www.instintodigital.net"></a>
</p>
