# prueba-llenar-encuesta
Un código javascript que se ejecuta en la consola del navegador, con el fin llenar un formulario. Selecciona los input de tipo radio que tenga valor de 4, llena los textarea con una cadena con espacios y finalmente selecciona el botón con Id grabar.


```
const sugerencias = document.querySelectorAll('textarea');
const opciones = document.querySelectorAll('input[type="radio"][value="4"]');

sugerencias.forEach((sugerencia) =>{
    sugerencia.value = '                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                ';
});

opciones.forEach((opcion) =>{
    opcion.click();
});

document.getElementById('grabar').click();
```
E D
```
var opciones = document.querySelectorAll('select option');

if (opciones.length === 0) {
    console.log('No se encontraron opciones en los elementos select.');
} else {
    var opcionesASeleccionar = [];

    opciones.forEach(function(opcion) {
        if (opcion.value === "4" || opcion.value === "5") {
            opcionesASeleccionar.push(opcion);
        }
    });

    opciones.forEach(function(opcion) {
        if (opcion.value === "4" || opcion.value === "5") {
            opcionesASeleccionar.push(opcion);
        }
    });

    if (opcionesASeleccionar.length === 0) {
        console.log('No se encontraron opciones con valores 4 o 5.');
    } else {
        opcionesASeleccionar.forEach(function(opcion) {

            opcion.selected = Math.random() < 0.5; // 50% de probabilidad de seleccionar cada opción
        });
    }
}
```
