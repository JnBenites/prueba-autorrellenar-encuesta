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
