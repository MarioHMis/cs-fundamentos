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
