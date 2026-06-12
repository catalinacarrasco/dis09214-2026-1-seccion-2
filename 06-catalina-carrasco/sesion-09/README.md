# sesión 06 - 12/06
# Apuntes: Crear un Sketch Adaptable al Tamaño de la Pantalla

## Objetivo
Diseñar un sketch que se adapte automáticamente a diferentes tamaños de pantalla utilizando medidas relativas en lugar de valores fijos.

---

## 1. Utilizar las variables integradas del sistema

Las variables:

- `windowWidth`
- `windowHeight`

permiten obtener el ancho y alto actuales de la ventana o pantalla.

```
createCanvas(windowWidth, windowHeight);
```

---

## 2. Trabajar con valores relativos

En lugar de usar medidas absolutas (píxeles fijos), utilizar:

- Fracciones
- Proporciones
- Porcentajes relativos al tamaño de la ventana

Ejemplo:

```javascript
let anchoFigura = windowWidth * 0.3;
let altoFigura = windowHeight * 0.2;
```

---

## 3. Crear un factor de referencia global

Se recomienda crear una variable global que sirva como referencia para escalar todos los elementos del sketch.

La referencia debe calcular el valor más pequeño entre el ancho y el alto de la ventana.

```javascript
let referencia;

function setup() {
  createCanvas(windowWidth, windowHeight);

  referencia = min(windowWidth, windowHeight);
}
```

### ¿Por qué usar `min()`?

- Compara el ancho y el alto de la ventana.
- Conserva el valor más pequeño.
- Permite que los elementos mantengan proporciones correctas independientemente de la orientación de la pantalla.

---

## 4. Escalar elementos usando la referencia

Una vez definida la referencia, todas las medidas pueden calcularse a partir de ella.

```javascript
let diametro = referencia * 0.2;
```

Esto facilita la adaptación automática a distintos dispositivos.

---

## 5. Evitar cálculos complejos para cada figura

En lugar de recalcular posiciones y tamaños para cada elemento geométrico, se recomienda utilizar transformaciones.

Funciones útiles:

- `translate()`
- `push()`
- `pop()`

---

## 6. Uso de `translate()`, `push()` y `pop()`

Estas funciones permiten mover el sistema de coordenadas temporalmente y dibujar figuras de manera más organizada.

```javascript
push();

translate(width / 2, height / 2);
circle(0, 0, referencia * 0.2);

pop();
```

