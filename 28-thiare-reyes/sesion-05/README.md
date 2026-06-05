# sesión 04 - 17/04
# Transformaciones y condicionales

## Transformaciones

**ÁNGULOS 
angleMode();**

* angleMode(RADIANS)
  Por defecto p5.js usa RADIANES para medir los ángulos.
* angleMode(DEGREES)
  Para cambiar a grados se usa esto en el fuction SETUP.

 * Hay que pensarlo como se mueven las agujas del reloj:
TWO_PI 360 ̊
PI 180 ̊
HALF_PI 90 ̊
QUARTER_PI 45 ̊


**ROTACIÓN
rotate();**
* Sirve para rotar elementos.
**SIEMPRE ROTA ALREDEDOR DEL PUNTO DE ORIGEN (0,0)**
  * Se recomienda usar con translate();
  * En algunos casos con rectMode(CENTER);

 * Sintaxis rotate(valor radianes o en grados);
 * Ejemplo: rotate(20);


**TRASLADAR
translate();**
* Sirve para trasladar el PUNTO DE ORIGEN (0,0) a otra cordenada de mi
canvas.

 * Sintaxis translate(x,y);
 * Ejemplo: translate(200,200);


**GUARDAR Y
RESTAURAR
push();
pop();**

* Funciones que trabajan juntas como un "sistema de memoria temporal" para el estilo y las transformaciones.

  * Sintaxis: push();
  * Sintaxis: pop();

**ESCALA
scale();**

* La función scale() ajusta la escala del sistema de coordenadas actual por el factor especificado.

  * Sintaxis scale(x,y);
  * Ejemplo: scale(2,2);


## Condicionales

*Expresión Booleana*

Una expresión booleana es cualquier enunciado, dato o instrucción que, al ser evaluado, sólo puede arrojar uno de dos valores posibles: verdadero (True) o falso (False).

* Es como hacer una afirmación y preguntarse: ¿Esto es cierto o no?

5 > 3 - verdadero
10 == 7 - falso

* Para construir este tipo de expresiones se utilizan 3 tipos de elementos:

 1. Operandos (o Valores):
    *  Son los datos básicos que se evalúan, pueden ser:
    *  Variables: (como x, y o mouseX, mouseY, etc).

 2. Operadores de Comparación:
     Permiten contrastar dos valores.
 == (igual a)
!= (diferente de)
o < (Mayor o igual)
= o <= (Mayot o igual / Menor o igual)

3. Operadores Lógicos:
    Sirven para combinar expresiones.
AND (&&): Es verdadero solo si ambas partes son verdaderas.
OR (||): Es verdadero si al menos una de las partes es verdadera.
NOT (!): Invierte el valor (si era verdadero, pasa a ser falso).
(5 > 3) AND (2 < 4) → verdadero
(10 == 5) OR (3 > 1) → verdadero
NOT (7 < 2) → verdadero

<img width="960" height="573" alt="Captura de pantalla 2026-05-21 143618" src="https://github.com/user-attachments/assets/c786d001-9ca6-4e18-82a3-f70b250a52b9" />

<img width="973" height="537" alt="Captura de pantalla 2026-05-21 143830" src="https://github.com/user-attachments/assets/30859e68-19c2-4f99-824c-08ac5cef1448" />


## Sentencia Condicional (If - else if - else)

* La sentencia if es una estructura especial que existe en casi todos los lenguajes de
programación; toma una condición –expresada como un booleano– y ejecuta una
pieza de código contenida dentro de las llaves { }

If (condición) {ejecuta este código si es true}
Si algún estudiante apaga por completo las luces de la sala, la profesora debe bailar.

**If - else if - else**
* La sentencia if puede complementarse con la sentencia (else if), que añade
condiciones de prueba complementarias a la original, y con la sentencia (else), que
implica todos los casos que no cumplen con la condición original.
* Nota: puedes añadir tantas sentencias (else if) como desees.
  
  * If (condición) {ejecuta este código si es true}
  *else if (condición 2) {ejecuta este código si es true}
  *else {ejecuta este código si ambas condiciones son falsas}

Si algún estudiante apaga por completo las luces de la sala, la profesora debe bailar.
Si no se cumple lo anterior SI la ayudante se levanta de su silla, la profesora debe cantar.
Y SI NO SE CUMPLEN NINGUNA DE LAS ANTERIORES, los estudiantes guardan silencio.


### Ejemplo square en p5.js
[P5.js](https://editor.p5js.org/ThiareReyes/sketches/Y3gV-r_uM)
