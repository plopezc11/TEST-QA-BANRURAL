Errores encontrados y sus soluciones
Aquí estaré presentando los errores que he encontrado por los cuales la página web no estaba funcionando.

Función
1. En la nueva página en la línea 64 he agregado un bloque if para poder validar si el usuario ingreso un número valido utilizando 'Number.isNaN()'.

Errores
1.El número aleatorio generado no está dentro del rango 1-100:
En la línea 48 al igual que en la línea 124, el número aleatorio se genera con Math.random() * 10, lo que significa que el número generado estará entre 0 y 9.9999... Para generar un número aleatorio entre 1 y 100, debes multiplicar Math.random() por 100 y luego usar Math.floor() para redondearlo a un número entero. Así, la línea 36 debería ser: 'let randomNumber = Math.floor(Math.random() * 100) + 1;'
2. Así mismo, me fije que el orden de los colores no era el correcto, con lo cual lo arregle, así como en la línea 76 en el 'lastResult.style.background = black' pero en realidad el color tenía que ser rojo con lo cual lo cambie a 'red'; Igual en la línea 86, para cuando el mensaje dijera "Felicitaciones" el color indicado era el verde y aparecía rojo, con lo cual realice el cambio de 'red' a 'green'; Y por último en la líneea 85, me indicaba que el color era rojo, pero tenía que mostrar 'lastResult.style.background = 'black' así que realice ese cambio para que los colores estuvieran correctamente. 
3. En la línea 53 se realizo modificaciones ya que principalmente aparecía 'const lowOrHi = document.querySelector('lowOrHi')' pero recordemos que al momento de nosotros de seleccionar una clase es importante colocar un punto antes del nombre de la clase, con lo cual nos quedaría de la siguiente manera 'const lowOrHi = document.querySelector('.lowOrHi')'.
4. En la línea 50 y 79 únicamente realice el cambio de 'ATTEMPS' a 'ATTEMPTS' para mantener la ortografía.
5. En la línea 97 y 105 se esta utilizando 'addeventListener' en lugar de 'addEventListener'. Javascript es sensible con las mayúsculas y minúsculas, por lo que se debe de escribir el nombre del método correctamente. Así 'guessSubmit.addEventListener('click', checkGuess);' y 'resetButton.addEventListener('click', resetGame);'
6. Esos serían los errores que he encontrado con sus soluciones, se han realizado las distintas pruebas y se ha concluido de que el juego funciona a su 100%. 

