# sesión 03 - 27/03
# P5.js

### Algoritmo
Secuencia de instrucciones finitas, lógicas, definidas, ordenadas y sin ambigüedad, la cual se realiza paso a paso.

* Estructura
  * Input (Entrada). 
  * Proceso.
  * Output (Salida).

**Ejemplo:**

1. Información (ingredientes y utensilios para comenzar).
2. Pasos lógicos (lista de instrucciones para hacer un sandwich).
3. Resultado final (sandwich terminado).


* Diagrama de flujo
  * Representación gráfica del algoritmo o de los pasos, se utiliza simbología.
 
* Lenguaje de programación
  * Principalmente en p5 se utiliza el lenguaje JavaScript.
 
### Funciones
* Setup: Una vez al principio, es el tamaño del lienzo, sonido, etc. (configuraciones que no cambian).
* createCanvas: Determinar el tamaño del lienzo (ancho y alto).
* Draw: Repetición infinita (60 veces por segundo), crea un movimiento o animación.
* Background: Color.
  * Escala de grises 220, 0 es negro y 255 es blanco.
  * rgb 3 números (255, 0, 0)(rojo, verde, azul).
  * Nombre de colores: ("blue"), siempre entre comillas.
  * Transparencia: 4 números (0, 0, 255); (rgb y el cuarto es canal "Alpha").

## Dibujar en p5
Sistema de coordenadas (plamo cartesiano).
* x (horizontal).
* y (vertical).
* 0, 0 (esquina superior izquierda).

### Figuras geométricas
* point:(x, y), crea un punto (300, 300).
  * stroke: Color del punto.
  * strokeWeight: Tamaño del borde.
* line:(x1, y1, x2, y2).
* rect:(x, y, ancho, alto).
* ellipse:(x, y, ancho, alto).
* circle:(x, y, diámetro).
* square:(x, y, lado).
* triangle:(x1, y1, x2, y2, x3, y3).
* quad:(x1, y1, x2, y2, x3, y3, x4, y4).
  * noStroke: Quitar el borde. 
  * fill: Relleno de color para las figuras.
* arc:(x, y, w, h, start, stop).
  * w y h son la anchura y alto del circulo que contiene el arco.
  * start y stop, es donde comienza y termina el ángulo del arco.
  * para activar los ángulos en SETUP(); debe estar:
  **angleMode(DEGREES);**
  * Los ángulos funcionan en dirección contraria al reloj.

