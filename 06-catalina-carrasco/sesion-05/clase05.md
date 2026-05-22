# Apuntes


## Pensamiento Computacional

El pensamiento computacional consiste en resolver problemas mediante procesos lógicos y organizados.

En programación, esto significa crear instrucciones claras que una computadora pueda ejecutar paso a paso.

---

# Algoritmos

Un algoritmo es una secuencia de instrucciones diseñada para resolver un problema o realizar una tarea.

- Precisión
- Orden lógico
- Finitud
- Resultados consistentes

## Estructura básica

```text
Entrada → Proceso → Salida
```

### Ejemplo

```text
Entrada: ingredientes
Proceso: preparar sandwich
Salida: sandwich listo
```

---

# Diagramas de Flujo

Los diagramas de flujo representan visualmente un algoritmo.

Sirven para:

- Organizar ideas
- Planificar programas
- Comprender procesos antes de programar

Utilizan símbolos estándar para representar acciones y decisiones.



# ¿Qué es p5.js?

p5.js es una librería de JavaScript orientada al creative coding.

Permite crear:

- Dibujos
- Animaciones
- Interacciones visuales
- Arte generativo

## Recursos

- https://p5js.org/es/
- https://p5js.org/reference/

---

# Estructura Básica de p5.js

Las dos funciones principales son:

## setup()

Se ejecuta una sola vez al iniciar el programa.

Se usa para:

- Crear el canvas
- Configurar variables
- Inicializar elementos

```javascript
function setup() {
  createCanvas(500, 500);
}
```

---

## draw()

Se ejecuta constantemente en bucle.

Se usa para:

- Crear movimiento
- Actualizar elementos
- Generar animaciones

```javascript
function draw() {
  background(220);
}
```

---

# Canvas

El canvas es el espacio donde se dibuja.

## createCanvas()

```javascript
createCanvas(ancho, alto);
```

### Ejemplo

```javascript
createCanvas(500, 500);
```



# Background

La función `background()` define el color del fondo.

## Ejemplos

### Escala de grises

```javascript
background(200);
```

### RGB

```javascript
background(255, 0, 0);
```

### Transparencia

```javascript
background(0, 0, 255, 50);
```

## Diferencia importante

- En `setup()` → fondo fijo
- En `draw()` → el canvas se limpia constantemente

---

# Modos de Color

## RGB

```javascript
colorMode(RGB);
```

Valores:

- Red
- Green
- Blue

Rango: `0 - 255`

---

## HSB

```javascript
colorMode(HSB);
```

Valores:

- Hue
- Saturation
- Brightness

---

## HSL

```javascript
colorMode(HSL);
```

Valores:

- Hue
- Saturation
- Lightness

---

# Sistema de Coordenadas

En p5.js:

```text
(0,0)
```

se encuentra en la esquina superior izquierda.

- X aumenta hacia la derecha
- Y aumenta hacia abajo

---

# Figuras Básicas

## Punto

```javascript
point(x, y);
```

## Línea

```javascript
line(x1, y1, x2, y2);
```

## Rectángulo

```javascript
rect(x, y, ancho, alto);
```

## Elipse

```javascript
ellipse(x, y, ancho, alto);
```

## Círculo

```javascript
circle(x, y, diametro);
```

## Cuadrado

```javascript
square(x, y, lado);
```

## Triángulo

```javascript
triangle(x1, y1, x2, y2, x3, y3);
```

## Cuadrilátero

```javascript
quad(x1, y1, x2, y2, x3, y3, x4, y4);
```

---

# Bordes y Líneas

## strokeWeight()

Controla el grosor del borde.

```javascript
strokeWeight(10);
```

---

## stroke()

Define el color del borde.

```javascript
stroke(255, 0, 0);
```

---

## strokeCap()

Define la forma de los extremos de línea.

```javascript
strokeCap(ROUND);
strokeCap(SQUARE);
strokeCap(PROJECT);
```

---

## noStroke()

Elimina el borde.

```javascript
noStroke();
```

---

# Relleno

## fill()

Define el color interior de las figuras.

```javascript
fill(252, 159, 216);
```

---

# Arcos

## arc()

Permite crear arcos y semicircunferencias.

```javascript
arc(x, y, w, h, inicio, fin);
```

### Ejemplo

```javascript
arc(250, 250, 100, 100, 270, 90);
```

---

# Ángulos en p5.js

Por defecto:

| Ángulo | Dirección |
|---|---|
| 0° | Derecha |
| 90° | Abajo |
| 180° | Izquierda |
| 270° | Arriba |

## Recomendación

```javascript
angleMode(DEGREES);
```

---

# Resumen

p5.js simplifica la programación visual utilizando JavaScript como base.

Conceptos fundamentales vistos:

- Algoritmos
- Diagramas de flujo
- Canvas
- Color
- Coordenadas
- Figuras geométricas
- Bordes y rellenos
- Animación mediante `draw()`
- Organización mediante `setup()`
