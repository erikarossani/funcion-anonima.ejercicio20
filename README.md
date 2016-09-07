# funcion-anonima.ejercicio20

##Contexto
###Ejercicio Inicial

var feature = 'closures'; 
(function () {     
if ( typeof feature === 'undefined' ){         
var feature = 'callbacks';         
console.log('JS coders love its ' + feature );     
} else {         
console.log('JS developers love its ' + feature );     
} 
})();

###Resultado final del ejercicio final 
(function () {  
var feature = 'closures'; 
if ( typeof feature === 'undefined' ){         
var feature = 'callbacks';         
console.log('JS coders love its ' + feature );     
} else {         
console.log('JS developers love its ' + feature );     
} 
})();
#### Explicación del ejercicio:

En el primer codigo  la línea 1 del código inicial está definida la variable (feature = "clousure") , pero al colocarla ahí, de manera global, la función anónima autoejecutable no la está llamando ya que para esa función anónima autoejecutable la variableque que predomina seria la  (var feature = 'callbacks');  y por eso arroja como resultado el primer mensaje ('JS coders love its '); por eso en el ejercicio final se coloca la variable (var feature = 'closures') definiendose asi de manera local pero predominando sobre la variable dentro del if  y ya  al ejecutarse no sería verdad la primera condición, sino la segunda y  se arroja el segundo mensaje.
