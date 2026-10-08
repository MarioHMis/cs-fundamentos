# Notas del Nivel 0

## Sesión 1: binario, bits y bytes

### Qué es un bit

Un bit es la unidad de información más pequeña que usa una computadora.
Funciona como un interruptor de luz: solo tiene 2 estados,
encendido (`1`) o apagado (`0`).

### Qué es un byte

Un byte son 8 bits juntos. Puede formar 256 valores distintos,
del 0 al 255. El máximo es 255 porque el 0 también cuenta.

### De decimal a binario

Un número decimal se puede escribir en binario y viceversa.
Por ejemplo, el 10 en binario es `1010` (8 + 2).

**Método:** un byte tiene estas posiciones:

`128  64  32  16  8  4  2  1`

Para escribir el 10 decimal en binario: el 16 no cabe en 10, así que
paso al 8. Si sumo el 4 me paso (12), así que no lo uso. Si sumo el 2
llego a 10. El 1 no es necesario. A cada número que uso le pongo `1`
y al que no, `0`. El resultado es `1010`.

Comprobación: 8 + 2 = 10.

### Reglas para contar en binario

+ 1 Incrementar la columna del extremo derecho en 1
 * Las columnas restantes se bajan
+  Cuando te quedes sin digitos:
 * Incrementa la siguiente columna en 1

## Sesión 2: cómo se guarda el texto

### ASCII

Es una tabla que le asigna un número a cada carácter del inglés para
poder identificarlo. Tiene 128 caracteres, numerados del 0 al 127,
porque eso es lo que cabe en 7 bits.

### Unicode vs UTF-8

Unicode amplía ASCII: le asigna un número único a cada carácter de
todos los idiomas, incluidos símbolos y emojis.
UTF-8 indica cuántos bytes usa cada carácter para guardarse.

### Caracteres y bytes

Se cuentan letra por letra. Por ejemplo, "Ñu" tiene 2 caracteres y
3 bytes: la Ñ usa 2 bytes y la u usa 1.

### Python

El prefijo `0b` indica que un número está escrito en binario.
Por ejemplo, `chr(0b1001101)` da `'M'`.

`SyntaxError`: Python no puede leer el código porque está mal escrito.
Ejemplo: `chr(01001101)`, porque un número no puede empezar con cero.

`NameError`: el código se lee bien, pero usa un nombre que no existe.
Ejemplo: `char(65)` en lugar de `chr(65)`.

