# Puerto_Post2_U8
# Checkpoints de Operaciones en Ensamblador

## Checkpoint 1: Suma de 32 bits (ADC)
En este apartado se implementó la suma de dos valores de 32 bits utilizando las instrucciones `ADD` y `ADC`. La instrucción `ADC` permite incluir el acarreo generado en la suma de la parte baja, asegurando así un resultado correcto en la parte alta.
Resultado esperado: Suma OK: 0003:0000

Se verifica que:

AX = 0000h
DX = 0003h

## Checkpoint 2: Resta de 32 bits (SBB)
Se desarrolló una resta de 32 bits empleando las instrucciones `SUB` y `SBB`. En este caso, `SBB` toma en cuenta el préstamo generado en la operación previa.
Resultado esperado: Resta OK

Se verifica que:

AX = FFFFh
DX = 0001h

## Checkpoint 3: Suma en BCD (DAA)
Se realizaron operaciones de suma con números en formato BCD empaquetado. Para garantizar que el resultado sea válido, se utilizó la instrucción `DAA`, la cual ajusta automáticamente el valor obtenido.

**Ejemplo:**
47 + 38 = 85

Resultado esperado: BCD suma: 85

## Checkpoint 4: Resta en BCD (DAS)
Se implementó la resta de valores en formato BCD, empleando la instrucción `DAS` para corregir el resultado y mantener su validez dentro de este formato.

**Ejemplo:**
73 - 28 = 45

Resultado esperado: 45

## Checkpoint 5: Calculadora básica (MUL y DIV)
Se desarrolló una calculadora sencilla capaz de realizar multiplicaciones y divisiones con números de un solo dígito, haciendo uso de las instrucciones `MUL` y `DIV`.

**Casos de prueba:**
7 * 8 = 56 9 / 3 = 3 División por 0 → muestra error
