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
(function () {  
var feature = 'closures'; 
if ( typeof feature === 'undefined' ){         
var feature = 'callbacks';         
console.log('JS coders love its ' + feature );     
} else {         
console.log('JS developers love its ' + feature );     
} 
})();
```
#### Explicación del ejercicio:

En el primer codigo  la línea 1 del código inicial está definida la variable (feature = "clousure") , pero al estar ahí, se ejecuta de manera global, y la función anónima autoejecutable no la está llamando ya que para esa función anónima autoejecutable la variable que predomina seria la  (var feature = 'callbacks') arrojando como resultado el primer console.log ('JS coders love its '); por eso en el ejercicio final se coloca la variable (var feature = 'closures') dentro de la función anónima autoejecutable definiendose asi de manera local pero predominando sobre la variable dentro del if  y ya  al ejecutarse no sería verdad la primera condición, sino la segunda y  se arroja el segundo mensaje.
