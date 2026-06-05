# sesión 06 - 15/05
# Loops, while y for

**LOOP**

El loop es un bucle, ¿Qué es un bucle?
1. Rizo de cabello en forma de helicoidal.
2. Objeto cuya forma recuerda la del bucle.
3. Proceso que se repite indefinidamente.
4. Informática. Serie de instrucciones que se repiten indefinidamente mientras no se cumpla una condición previamente establecida.

Loop: Estructura de control que permite ejecutar un bloque de instrucciones de manera repetida mientras cumpla una condición específica o hasta que se alcance un estado determinado.

**WHILE** 
Los bucles while son útiles para repetir instrucciones mientras una condición sea verdadera. Son como sentencias if que se repite.
- while(condición booleana){ejecuta este código si este true}

**FOR**
 * Este se usa mas que el while.
Una forma de repetir un bloque de código cuando se conoce el número de iteraciones. Los bucles "for" son útiles para repetir instrucciones un número determinado de veces. Son una especie de SHORTCUT para hacer loops y siempre tienen 4 elementos: 
1. Inicialización de una variable.
2. Condición booleana (V-F).
3. Actualización (Incrementación o decrementación).
4. Lo que queremos que pasé cuando la condición sea TRUE.

for (inicialización variable; condición booleana; actualización){ Lo que queremos que pase cuando la condición sea verdadera }
// Integra la variable dentro del comando

for (let x=0; x <= width; x=x+1) {

ellipse (x, 200,random(300))
}

* Ejemplo for
[P5.js](https://editor.p5js.org/ThiareReyes/sketches/-g84sMAV3)


