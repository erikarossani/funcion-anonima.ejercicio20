# funcion-anonima.ejercicio20

##Contexto
###Ejercicio Inicial
```javascript

var feature = 'closures'; 
(function () {     
     if ( typeof feature === 'undefined' ){         
         var feature = 'callbacks';         
         console.log('JS coders love its ' + feature );     
      } else {         
        console.log('JS developers love its ' + feature );     
} 
})();
```
###Resultado final del ejercicio final 
```javascript

var feature = 'closures'; 
(function () {    
    if ( typeof feature === 'undefined' ){         
        feature = 'callbacks';         
        console.log('JS coders love its ' + feature );     
} else {         
        console.log('JS developers love its ' + feature );     
} 
})();
```
#### Explicación del ejercicio:

En el primer codigo  la línea 1 del código inicial está definida la variable (feature = "clousure") , pero al estar ahí, se ejecuta de manera global, y la función anónima autoejecutable  está llamando a la variable (var feature = 'callbacks') que es la que predomina(se eleva) arrojando como resultado el primer console.log ('JS coders love its '); por eso en el ejercicio final se borra el (var) de la variable dentro de la función para que asi predomine la variable local.
