# sesión 24/04
arreglar bitacora
comentar el codigo para que sirva hasta para una persona que no sabe nada de codigo y lo entienda 
4 PILARES DEL PENSAMIENTO COMPUTACIONAL 
1 descomposición: tomar un problema grande y complejo y romperlo en partes mas pequeñas, uso de funciones propias 
2 reconocimiento de patrones: observar tendencias o irregularidades dentro de un problema. si algo se repite o sigue una logica constante, podemos automatizarlo
3 abstraccion: representación simbolica de la realidad
4ALGORITMOS: serie de reglas ordenadas logicas, plan de accion, flujo de la experiencia, diagrama deflujo y condicionales 

TIPOS DE INTERACCIÓM:
Interaccion discreta: accioón reacción, algo especificpo
interacción continua, reacciona sin necesidad de hacer algo especifico

FUNCIONES PROPIAS: 
da modularidad al código y reusabilidad
https://editor.p5js.org/catalinacarrasco/sketches/9n5YSr74D (EJECRICIOCIRCULOSMOVIMIENTO)

https://editor.p5js.org/catalinacarrasco/sketches/T0Qiu1EdJ(RJRCRCICIO FUNCIONES PROPIAS)

https://editor.p5js.org/catalinacarrasco/sketches/1NPqmQQ6I(EJECRICIOELIPSEREBOTANDO) # Clase 06 — Funciones Propias

## Pensamiento Computacional

### 4 pilares

1. Descomposición  
2. Reconocimiento de patrones  
3. Abstracción  
4. Algoritmos  

---

# 1. Descomposición

- Dividir un problema grande en partes más pequeñas.
- Ayuda a ordenar el proyecto.
- En vez de hacer todo en `draw()`, separar tareas.

Ejemplo:

```javascript
function dibujarFondo() {

}

function dibujarPersonajes() {

}

function mostrarTexto() {

}
```

Idea:
- Cada función hace solo una tarea.
- Código más limpio y fácil de corregir.

---

# 2. Reconocimiento de patrones

- Buscar cosas que se repiten.
- Si algo se repite muchas veces → usar `for`.

Ejemplo:

```javascript
for(let i = 0; i < 10; i++) {
  ellipse(i * 50, 100, 20, 20);
}
```

Notas:
- Evita escribir el mismo código muchas veces.
- Sirve para automatizar elementos.

---

# 3. Abstracción

- Quedarse solo con lo importante.
- Transformar datos en representaciones visuales.

Ejemplo:

```javascript
let tamaño = map(mouseX, 0, width, 10, 100);
```

Notas:
- `mouseX` puede controlar tamaño, color, velocidad, etc.
- No se necesita representar todo literalmente.

---

# 4. Algoritmos

- Serie de pasos para resolver algo.
- Uso de reglas y decisiones.

Ejemplo:

```javascript
if(mouseIsPressed) {
  background(255);
} else {
  background(0);
}
```

Notas:
- Importante para interacciones.
- Relacionado con lógica y flujo.

---

# Tipos de interacción

## Interacción discreta

- Ocurre con un evento específico.
- Ejemplo: click.

```javascript
function mousePressed() {
  ellipse(mouseX, mouseY, 20, 20);
}
```

---

## Interacción continua

- El sistema responde constantemente.
- Ejemplo: movimiento del mouse.

```javascript
ellipse(mouseX, 200, 50, 50);
```

---

# Funciones propias

## Ideas importantes

- Modularidad
- Reusabilidad
- Ordenar el código
- Evitar repetir instrucciones

---

# Sintaxis básica

```javascript
function nombreFuncion() {

}
```

---

# Ejemplo completo

```javascript
function setup() {
  createCanvas(400, 400);
}

function draw() {
  background(200);

  dibujarCirculo();
}

function dibujarCirculo() {
  fill(100, 200, 255);
  ellipse(mouseX, mouseY, 50, 50);
}
```

---

# Markdown para GitHub

## Bloque de código

````markdown

