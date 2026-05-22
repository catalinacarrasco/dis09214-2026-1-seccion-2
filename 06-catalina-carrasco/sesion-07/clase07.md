
LOOPS EN p5.js
WHILE, FOR Y NESTED LOOPS
====================================================


====================================================
¿QUÉ ES UN LOOP?
====================================================

Un loop (o bucle) es una estructura que permite
repetir instrucciones automáticamente.

Las instrucciones se repiten:

✔ mientras se cumpla una condición
✔ o hasta alcanzar un estado específico


----------------------------------------------------
DEFINICIÓN
----------------------------------------------------

Un loop es una serie de instrucciones que se
repiten indefinidamente mientras NO se cumpla
una condición previamente establecida.


====================================================
TIPOS DE LOOPS
====================================================

1. while
2. for


====================================================
WHILE LOOP
====================================================

El loop while ejecuta código mientras una
condición sea verdadera.


----------------------------------------------------
ESTRUCTURA
----------------------------------------------------
*/

while (condicionBooleana) {

  // código que se repite

}

/*
----------------------------------------------------
FUNCIONAMIENTO
----------------------------------------------------

1. Se evalúa la condición
2. Si es true → ejecuta el código
3. Se repite el proceso
4. Termina cuando la condición es false


====================================================
EJEMPLO BÁSICO
====================================================
*/

let x = 0;

while (x <= 10) {

  console.log(x);

  x = x + 1;

}

/*
----------------------------------------------------
EXPLICACIÓN
----------------------------------------------------

✔ x comienza en 0
✔ mientras x <= 10
✔ x aumenta de 1 en 1
✔ el loop termina cuando x > 10


====================================================
EJEMPLO EN p5.js
====================================================
*/

function setup() {

  createCanvas(400, 400);

  background(30);

  let x = 0;

  while (x <= width) {

    fill(255);

    ellipse(x, 200, 20);

    x = x + 25;

  }

}

/*
Este loop dibuja una fila de círculos.
*/


/*
====================================================
CUIDADO: LOOP INFINITO
====================================================

Si la condición nunca cambia,
el loop nunca termina.

Ejemplo peligroso:
*/

let numero = 0;

while (numero < 10) {

  console.log(numero);

  // FALTA actualizar numero

}

/*
Esto genera un LOOP INFINITO.
*/


/*
====================================================
USOS DEL WHILE
====================================================

Se utiliza cuando:

✔ NO sabemos exactamente cuántas veces
  se repetirá el proceso

✔ depende de una condición dinámica


====================================================
FOR LOOP
====================================================

El loop for se utiliza cuando conocemos
la cantidad aproximada de iteraciones.


----------------------------------------------------
ESTRUCTURA
----------------------------------------------------
*/

for (inicializacion; condicion; actualizacion) {

  // código

}


/*
====================================================
ELEMENTOS DEL FOR
====================================================

1. Inicialización
2. Condición
3. Actualización
4. Código a ejecutar


----------------------------------------------------
EJEMPLO SIMPLE
----------------------------------------------------
*/

for (let i = 0; i < 10; i = i + 1) {

  console.log(i);

}

/*
----------------------------------------------------
EXPLICACIÓN
----------------------------------------------------

✔ i comienza en 0
✔ mientras i < 10
✔ i aumenta en 1
✔ se imprime el número


====================================================
EJEMPLO EN p5.js
====================================================
*/

function setup() {

  createCanvas(600, 400);

  background(20);

  for (let x = 0; x <= width; x = x + 25) {

    fill(0, 200, 255);

    ellipse(x, 200, 20);

  }

}

/*
Esto dibuja múltiples círculos automáticamente.
*/


/*
====================================================
EJEMPLO CON RANDOM()
====================================================
*/

function setup() {

  createCanvas(600, 400);

  background(0);

  for (let x = 0; x <= width; x = x + 20) {

    fill(random(255), random(255), random(255));

    ellipse(x, height / 2, random(10, 100));

  }

}

/*
Cada círculo tiene:
✔ tamaño aleatorio
✔ color aleatorio
*/


/*
====================================================
NESTED LOOPS
LOOPS ANIDADOS
====================================================

Un nested loop es un loop dentro de otro loop.


----------------------------------------------------
ESTRUCTURA
----------------------------------------------------
*/

for (let x = 0; x < 10; x++) {

  for (let y = 0; y < 10; y++) {

    // código

  }

}


/*
----------------------------------------------------
FUNCIONAMIENTO
----------------------------------------------------

✔ El loop exterior recorre X
✔ El loop interior recorre Y
✔ Permite trabajar en 2 dimensiones


====================================================
EJEMPLO GRID
====================================================
*/

function setup() {

  createCanvas(500, 500);

  background(30);

  for (let x = 0; x <= width; x = x + 25) {

    for (let y = 0; y <= height; y = y + 25) {

      fill(0, 0, 255);

      ellipse(x, y, 15);

    }

  }

}

/*
----------------------------------------------------
EXPLICACIÓN
----------------------------------------------------

✔ x avanza horizontalmente
✔ y avanza verticalmente
✔ se crea una grilla de círculos


====================================================
VARIACIÓN DE GRID
====================================================
*/

function setup() {

  createCanvas(500, 500);

  background(10);

  for (let x = 0; x <= width; x += 40) {

    for (let y = 0; y <= height; y += 40) {

      fill(random(255), 100, 255);

      rect(x, y, 30, 30);

    }

  }

}

/*
Este ejemplo crea una grilla de cuadrados.
*/


/*
====================================================
frameCount
====================================================

frameCount es una variable incorporada de p5.js.

Guarda la cantidad de frames dibujados desde
que comenzó el sketch.


----------------------------------------------------
CARACTERÍSTICAS
----------------------------------------------------

✔ En setup() vale 0

✔ Aumenta automáticamente en draw()

✔ Se actualiza cada frame


====================================================
EJEMPLO frameCount
====================================================
*/

function setup() {

  createCanvas(500, 500);

}

function draw() {

  background(30);

  let x = frameCount;

  fill(255);

  circle(x, height / 2, 50);

}

/*
----------------------------------------------------
EXPLICACIÓN
----------------------------------------------------

✔ frameCount aumenta constantemente
✔ el círculo se mueve automáticamente


====================================================
frameCount + SIN()
====================================================
*/

function setup() {

  createCanvas(600, 400);

}

function draw() {

  background(0);

  let y = sin(frameCount * 0.05) * 100 + height / 2;

  fill(0, 200, 255);

  circle(width / 2, y, 80);

}

/*
Esto genera movimiento oscilatorio.
*/


/*
====================================================
USOS DE frameCount
====================================================

✔ Animaciones
✔ Tiempo
✔ Movimiento
✔ Eventos automáticos
✔ Control temporal


====================================================
COMPARACIÓN WHILE vs FOR
====================================================

WHILE
-------------------------
✔ depende de condición
✔ iteraciones desconocidas

FOR
-------------------------
✔ número de repeticiones conocido
✔ estructura más ordenada


====================================================
IDEAS CLAVES
====================================================

✔ Los loops automatizan tareas repetitivas

✔ while depende de una condición

✔ for funciona mejor cuando sabemos
  cuántas veces repetir

✔ nested loops permiten trabajar
  en estructuras bidimensionales

✔ frameCount ayuda a controlar
  tiempo y animación


====================================================
RESUMEN RÁPIDO
====================================================

✔ while → repite mientras algo sea true

✔ for → repite una cantidad específica

✔ nested loops → loops dentro de loops

✔ frameCount → cuenta frames automáticamente

✔ loops → automatizan dibujo y animación


====================================================
EJEMPLO FINAL COMPLETO
====================================================
*/

function setup() {

  createCanvas(600, 600);

}

function draw() {

  background(20);

  for (let x = 0; x <= width; x += 50) {

    for (let y = 0; y <= height; y += 50) {

      let tamano = map(
        dist(mouseX, mouseY, x, y),
        0,
        300,
        50,
        5
      );

      fill(
        random(255),
        100,
        255
      );

      ellipse(x, y, tamano);

    }

  }

}

/*
----------------------------------------------------
ESTE EJEMPLO UTILIZA:
----------------------------------------------------

✔ for
✔ nested loops
✔ map()
✔ mouseX / mouseY
✔ random()
✔ animación
✔ interacción

*/
