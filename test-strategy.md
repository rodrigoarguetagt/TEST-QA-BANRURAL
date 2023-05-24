Aquí están los errores que encontré en el código:

## Error en el script:
* El evento para el botón de envío (guessSubmit) está escrito como addeventListener, pero debería ser addEventListener (con una "E" mayúscula).

## Error en el selector de lowOrHi: 
* En la línea donde se selecciona el elemento con la clase lowOrHi, falta el punto antes del nombre de la clase. Debería ser .lowOrHi.

## Error en la generación del número aleatorio: 
En la línea donde se genera el número aleatorio, falta multiplicar por 100 para asegurarse de que el número esté en el rango de 1 a 100. Debería ser Math.random() * 100.

## Error en la comparación de cadenas y números: 
En la comparación userGuess === randomNumber, se compara una cadena con un número. Deberías convertir userGuess a número utilizando parseInt(userGuess) para hacer una comparación numérica en lugar de una comparación de cadenas.

## Error en la generación del nuevo número aleatorio en resetGame(): 
En la línea donde se genera el nuevo número aleatorio, la función Math.floor(Math.random()) debe incluir Math.random() * 100 para asegurarse de que el número esté en el rango de 1 a 100. Debería ser Math.floor(Math.random() * 100) + 1.