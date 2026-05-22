# El peso de ser mujer
## Matias Montes, Catalina Carrasco

## Descripción y contextualización

*El peso de ser mujer* es un proyecto interactivo desarrollado en p5.js que aborda la presión social y la violencia verbal ejercida hacia la mujer. A través de imágenes, parpadeos, interacción del usuario y figuras geométricas en constante expansión, la obra busca representar visualmente la ansiedad, la saturación mental y la fragmentación emocional provocadas por las críticas y expectativas sociales impuestas sobre la identidad femenina.

La experiencia inicia con un ambiente oscuro e inestable, donde imágenes y elementos visuales parpadean constantemente, generando una sensación de tensión e incomodidad. A medida que el usuario interactúa con el proyecto, entra simbólicamente en los pensamientos de la figura femenina, activando un colapso visual representado mediante triángulos aleatorios que crecen y ocupan toda la pantalla. Estos elementos representan pensamientos intrusivos, críticas, insultos y la acumulación de presión psicológica que afecta la percepción y construcción de la identidad de la mujer.

El proyecto busca generar empatía y reflexión en el espectador, utilizando la interacción como una metáfora del acceso a la carga mental que muchas mujeres experimentan debido a la violencia verbal, las imposiciones sociales y la constante evaluación de sus cuerpos, emociones y comportamientos.

---

## Explicación técnica

El proyecto fue desarrollado utilizando p5.js y está compuesto por múltiples interacciones visuales y condicionales programadas mediante JavaScript.

El sketch utiliza imágenes cargadas mediante ⁠ preload() ⁠, función encargada de asegurar que todos los recursos visuales estén disponibles antes de iniciar la ejecución del programa. Posteriormente, ⁠ setup() ⁠ configura el canvas y define parámetros visuales como el modo de alineación de imágenes y figuras.

La lógica principal ocurre dentro de ⁠ draw() ⁠, función que se ejecuta constantemente y permite generar animaciones, parpadeos e interacciones en tiempo real.

El proyecto incorpora:

•⁠  ⁠Variables propias para controlar estados visuales e interacciones.
•⁠  ⁠Variables integradas de p5.js como ⁠ mouseX ⁠, ⁠ mouseY ⁠, ⁠ width ⁠, ⁠ height ⁠ y ⁠ frameCount ⁠.
•⁠  ⁠Uso de figuras geométricas como triángulos, rectángulos, círculos y elipses.
•⁠  ⁠Imágenes y texto interactivo.
•⁠  ⁠Funciones ⁠ random() ⁠ y ⁠ map() ⁠ para generar comportamientos dinámicos y variaciones visuales.
•⁠  ⁠Transformaciones mediante ⁠ translate() ⁠, ⁠ rotate() ⁠ y ⁠ scale() ⁠, protegidas por ⁠ push() ⁠ y ⁠ pop() ⁠.
•⁠  ⁠Condicionales ⁠ if ⁠, ⁠ else if ⁠ y ⁠ else ⁠ para controlar la progresión narrativa del proyecto.
•⁠  ⁠Bucles ⁠ for ⁠ utilizados para crear múltiples triángulos de forma repetitiva.
•⁠  ⁠Funciones propias fuera de ⁠ draw() ⁠, como ⁠ mousePressed() ⁠ y ⁠ keyPressed() ⁠.
•⁠  ⁠Interacción directa con el usuario mediante movimiento del mouse y clicks.

Visualmente, el proyecto utiliza el parpadeo y la repetición para representar ansiedad e inestabilidad emocional. Además, el crecimiento progresivo de los triángulos simboliza la expansión de pensamientos negativos y la saturación mental derivada de la presión social y la violencia verbal.

---

## Relación entre concepto y programación

Cada decisión visual dentro del código fue pensada para reforzar el concepto principal del proyecto.

El parpadeo constante representa la ansiedad, la inseguridad y la inestabilidad emocional. Las imágenes que aparecen y desaparecen generan una sensación de interferencia y saturación mental.

La interacción de hacer click sobre la cabeza de la mujer simboliza el acceso a sus pensamientos internos. A partir de esta acción, comienza una explosión visual de triángulos aleatorios que representan críticas, insultos y pensamientos fragmentados acumulados por la presión social.

El uso de posiciones aleatorias mediante ⁠ random() ⁠ permite que los triángulos nunca tengan una forma fija, reforzando visualmente el caos mental y emocional. Por otro lado, el crecimiento progresivo de estas figuras hasta ocupar toda la pantalla simboliza cómo estos pensamientos terminan consumiendo completamente el espacio mental de la persona.

La transición de color desde blanco hacia amarillo representa un cambio gradual desde un estado neutral hacia uno de alerta, tensión y saturación emocional.

---

## Referentes

### Fundamentación de referentes visuales

El proyecto busca representar visualmente la presión social y la violencia verbal ejercida hacia la mujer, mostrando cómo estos discursos pueden generar ansiedad, saturación emocional y fragmentación mental. Para construir esta narrativa visual se utilizaron distintos referentes simbólicos y gráficos.

Uno de los principales referentes corresponde a imágenes de figuras humanas con distorsiones visuales en la cabeza, utilizadas para representar el colapso mental provocado por la acumulación de críticas, insultos y pensamientos negativos. Estas alteraciones visuales simbolizan cómo la presión social invade el espacio mental y afecta la identidad femenina.
<img width="1080" height="1080" alt="17794356174318004435705263220831" src="https://github.com/user-attachments/assets/e06a0882-4157-42e3-89a1-a04650591f30" />

---


También se incorporaron siluetas femeninas como recurso visual, permitiendo representar la identidad de la mujer desde una forma universal y simbólica. La ausencia de rasgos específicos refuerza la idea de pérdida de individualidad frente a las exigencias sociales y los estereotipos impuestos.
<img width="1000" height="1080" alt="17794354776561062550569783356877" src="https://github.com/user-attachments/assets/fd6ff3b4-11e0-425f-9e2b-341e19612035" />

---

La orquídea fue utilizada como referente por su relación con la feminidad, la delicadeza y la vulnerabilidad. Además de su carga simbólica, su forma orgánica establece una relación visual con el cuerpo femenino, convirtiéndose en una representación de sensibilidad frente a la violencia verbal y social.
<img width="474" height="714" alt="17794363640018728989486923282978" src="https://github.com/user-attachments/assets/5b2b2cd6-8833-4ba4-a120-d2115dbf15c2" />

---
En cuanto a la composición tipográfica, se tomaron referentes donde el texto invade visualmente el espacio, generando sensaciones de presión y saturación. El uso de tipografías pesadas y agresivas busca representar la violencia de las palabras y el impacto psicológico que estas pueden generar sobre la mujer.
<img width="540" height="756" alt="17794364985916783448613491936293" src="https://github.com/user-attachments/assets/74f61eff-0d83-4bab-b930-8e16d5cdb049" />

---

La combinación de estos referentes permite construir una experiencia visual inmersiva donde el espectador entra metafóricamente en los pensamientos de la protagonista, comprendiendo la carga emocional y mental producida por la presión social y la violencia verbal hacia las mujeres.

---

## Objetivo del proyecto

El objetivo del proyecto es representar de manera interactiva la presión psicológica y emocional que puede experimentar la mujer debido a las críticas, expectativas y violencia verbal presentes en la sociedad, utilizando herramientas de programación visual para generar una experiencia inmersiva que provoque empatía, reflexión e incomodidad en el espectador.

p5*js: [Aqui dentro](https://editor.p5js.org/catalinacarrasco/sketches/RixkEBgWQ)  

## MAPA DE FLUJO
![mapa](https://cdn.phototourl.com/free/2026-05-22-c355b069-f7a7-4950-bae7-f36dabf7ea7b.jpg)
#CÓDIGO
//IMÁGENES

let textoImg; // guarda imagen del texto
let mujer; // guarda imagen mujer
let fondoParpadeo; // guarda fondo que parpadea
let imagenInferior; // guarda imagen inferior

//VARIABLES 
let textoActivo = true; // controla si texto aparece
let mujerVisible = false; // controla aparición mujer
let cuadradoVisible = false; // controla cuadrado
let mensajeVisible = false; // controla mensaje

//EXPLOSIÓN 
let explotar = false; // activa triángulos

//PARPADEO 
let parpadeoTexto = true; // controla parpadeo texto

//TRIÁNGULOS 
let triangulos = []; // arreglo donde se guardan triángulo

//PRELOAD 
function preload() {
  textoImg = loadImage("texto.png"); // carga imagen texto
  mujer = loadImage("mujer.png"); // carga imagen mujer
  fondoParpadeo = loadImage("fondo.png"); // carga imagen fondo
  imagenInferior = loadImage("inferior.png"); // carga imagen inferior
}

//SETUP 
function setup() {
  createCanvas(500,800); // crea canvas
  imageMode(CENTER); // centra imágenes
  rectMode(CENTER); // centra rectángulos
  noStroke(); // elimina bordes
}

//DRAW 
function draw() {
  background(0); // fondo negro

  //DETECTAR MOUSE
  let mouseDentro = // detecta si mouse está dentro
    mouseX > 0 && // mouse mayor a 0 en x
    mouseX < width && // mouse menor al ancho
    mouseY > 0 && // mouse mayor a 0 en y
    mouseY < height; // mouse menor al alto

  //FONDO PARPADEANTE
  let mostrarFondo = true; // controla fondo
  if (!mouseDentro) { // si mouse está fuera
    if (frameCount % 4 < 2) { // crea parpadeo
      mostrarFondo = true; // muestra fondo
    } else {
      mostrarFondo = false; // oculta fondo
    }
  }
  else {
    mostrarFondo = true; // deja fondo fijo
  }
  if (mostrarFondo && textoActivo) { // dibuja fondo
    push(); // guarda configuración
    let ratioFondo = fondoParpadeo.width / fondoParpadeo.height; // calcula proporción
    let fondoW = width; // ancho fondo
    let fondoH = fondoW / ratioFondo; // alto proporcional
    if (fondoH < height) { // si altura es pequeña
      fondoH = height; // ajusta altura
      fondoW = fondoH * ratioFondo; // recalcula ancho
    }
 image(
      fondoParpadeo, // imagen
      width / 2, // posición x
      height / 2, // posición y
      fondoW, // ancho
      fondoH // alto
    );
    pop(); // restaura configuración
  }

  //CÍRCULO CENTRAL
  if (!mouseDentro) { // si mouse está fuera
    noFill(); // sin relleno
    stroke(251,224,23); // color amarillo
    strokeWeight(20); // grosor borde
    ellipse(
      width / 2, // posición x
      height / 2, // posición y
      10, // ancho
      10 // alto
    );
  }

  //IMAGEN INFERIOR
  if (!mouseDentro) { // si mouse está fuera
    push(); // guarda configuración
    let ratioInferior = imagenInferior.width / imagenInferior.height; // calcula proporción
    let inferiorW = 250; // ancho imagen
    let inferiorH = inferiorW / ratioInferior; // alto proporcional
     image(
      imagenInferior, // imagen
      width / 2, // posición x
      height - inferiorH / 2 - 100, // posición y
      inferiorW, // ancho
      inferiorH // alto
    );
    pop(); // restaura configuración
  }

  //TEXTO PARPADEANTE
  if (textoActivo) { // si texto activo
    if (frameCount % 4 < 2) { // genera parpadeo
      parpadeoTexto = true; // muestra texto
    } else {
      parpadeoTexto = false; // oculta texto
    }
    if (mouseDentro) { // si mouse entra
      if (parpadeoTexto) { // si texto visible
        push(); // guarda configuración
        translate(width / 2,height / 2); // mueve origen centro
        rotate(sin(frameCount * 0.25) * 0.04); // rotación suave
        let escalaTexto = map(
          mouseY, // valor original
          0, // mínimo original
          height, // máximo original
          0.92, // mínimo nuevo
          1.08 // máximo nuevo
        );
        scale(escalaTexto); // aplica escala
        let ratioTexto = textoImg.width / textoImg.height; // calcula proporción
        let textoW = 340; // ancho texto
        let textoH = textoW / ratioTexto; // alto proporcional
        image(
          textoImg, // imagen
          0, // posición x
          0, // posición y
          textoW, // ancho
          textoH // alto
        );
        pop(); // restaura configuración
      }
    }
  }
  
  //CUADRADO DERECHO
  if (cuadradoVisible && !mujerVisible) { // si cuadrado visible
    fill(251,224,23); // color amarillo
    rect(
      width - 40, // posición x
      height / 2, // posición y
      20, // ancho
      20 // alto
    );

    let dCuadrado = dist(
      mouseX, // mouse x
      mouseY, // mouse y
      width - 40, // x cuadrado
      height / 2 // y cuadrado
    );

    if (dCuadrado < 80) { // si mouse se acerca
      mujerVisible = true; // muestra mujer
      cuadradoVisible = false; // oculta cuadrado
      mensajeVisible = true; // muestra mensaje
    }
  }

  //MUJER
  if (mujerVisible) { // si mujer visible
    let escalaMujer = map(
      mouseY, // valor original
      0, // mínimo original
      height, // máximo original
      0.95, // mínimo nuevo
      1.15 // máximo nuevo
    );
    
    push(); // guarda configuración
    translate(width / 2,height / 2 + 80); // mueve origen
    scale(escalaMujer); // aplica escala
    rotate(sin(frameCount * 0.25) * 0.04); // rotación suave
    let ratioMujer = mujer.width / mujer.height; // calcula proporción
    let mujerH = 760; // altura mujer
    let mujerW = mujerH * ratioMujer; // ancho proporcional

    image(
      mujer, // imagen
      0, // posición x
      0, // posición y
      mujerW, // ancho
      mujerH // alto
    );
    pop(); // restaura configuración
    noFill(); // sin relleno
    stroke(255,100); // borde transparente
    strokeWeight(2); // grosor borde
    ellipse(
      width / 2, // posición x
      height / 2 - 110, // posición y
      100, // ancho
      100 // alto
    );
  }

  //TRIÁNGULOS RANDOM
  if (explotar) { // si explosión activa
    for (let i = 0; i < 5; i++) { // crea 5 triángulos
      triangulos.push({
        x: width / 2 + random(-20,20), // posición x
        y: height / 2 - 110 + random(-20,20), // posición y
        tam: random(5,20), // tamaño
        rot: random(TWO_PI), // rotación,variable que guarda el angulo de giro del triangulo
        vel: random(12,25), // velocidad
      });
    }

    for (let t of triangulos) { // revisa triángulos
      t.tam += t.vel; // aumenta tamaño
      let progreso = map(t.tam,0,width * 2,0,1); // crea progreso
      progreso = constrain(progreso,0,1); // limita valor
      let r = 255; // rojo fijo
      let g = lerp(255,220,progreso); // verde cambia
      let b = lerp(255,0,progreso); // azul desaparece
      let visible = random() > 0.35; // genera parpadeo

      if (visible) { // si triángulo visible
        push(); // guarda configuración
        translate(t.x,t.y); // mueve origen
        rotate(t.rot); // rota triángulo
        fill(r,g,b); // aplica color
        noStroke(); // elimina borde
        triangle(
          random(-t.tam,t.tam),//cambia la posición del triangulo, random
          random(-t.tam,t.tam),//cambia la posición del triangulo, random
          random(-t.tam,t.tam),//cambia la posición del triangulo, random
          random(-t.tam,t.tam),//cambia la posición del triangulo, random
          random(-t.tam,t.tam),//cambia la posición del triangulo, random
          random(-t.tam,t.tam)//cambia la posición del triangulo, random
        );
 pop(); // restaura configuración
      }
    }
  }

  //TEXTOS
  textSize(12); // tamaño texto
  textAlign(CENTER); // centra texto
  fill(255); // color blanco
  noStroke(); // elimina borde

  if (textoActivo && mouseDentro) { // texto inicial
    text("CLICK EN LA IMAGEN",width / 2,740); // dibuja texto
  }
  if (cuadradoVisible && !mujerVisible) { // texto cuadrado
    text("ACÉRCATE AL CUADRADO",width / 2,740); // dibuja texto
  }
  if (mujerVisible && !explotar) { // texto cabeza
    text("CLICK EN LA CABEZA",width / 2,740); // dibuja texto
  }
  if (mensajeVisible && !explotar) { // mensaje final
    fill(0); // color negro
    text(
      "ENTRA EN MIS PENSAMIENTOS Y HAZ CLICK",
      width / 2, //dibuja texto
      750
    );
  }
}

//CLICK 
function mousePressed() {
  if (textoActivo) { // si texto activo
    textoActivo = false; // oculta texto
    cuadradoVisible = true; // muestra cuadrado
  }
  else if (mujerVisible) { // si mujer visible
    let d = dist(
      mouseX, // mouse x
      mouseY, // mouse y
      width / 2, // cabeza x
      height / 2 - 110 // cabeza y
    );
    if (d < 120) { // si click cerca cabeza
      explotar = true; // activa explosión
      mensajeVisible = false; // oculta mensaje
    }
  }
}
//TECLADO 
function keyPressed() {
  if (key == "r" || key == "R") { // si tecla es r
    textoActivo = true; // reinicia texto
    mujerVisible = false; // oculta mujer
    cuadradoVisible = false; // oculta cuadrado
    mensajeVisible = false; // oculta mensaje
    explotar = false; // desactiva explosión
    triangulos = []; // vacía triángulos
  }
}
