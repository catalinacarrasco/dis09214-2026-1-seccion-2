# sesión 04 - 10/4
# Variables

Son datos constantes o que van cambiando (valores, números, etc)

## Variables integradas en p5

* MouseX, MouseY
  Variables de sistema numérico que determinan la posición del mouse en las coordenadas
  X e Y.
  * Sintaxis: (mouseX, mouseY);
  * Ejemplo: ellipse(mouseX, mouseY, 100, 100);

<img width="867" height="396" alt="Captura de pantalla 2026-05-21 124727" src="https://github.com/user-attachments/assets/61599d83-7d4b-4b12-9952-a4a5c7a0bfd1" />
<img width="863" height="443" alt="Captura de pantalla 2026-05-21 124747" src="https://github.com/user-attachments/assets/5dbc2a37-9edb-48f8-9712-ff6fdfbbf3b9" />

 
## Variables creadas en p5

 Se usa let (dinámicas), const (constantes)

* La variable puede tener el nombre que quieran pero la primera palabra va en minúscula y después la otra palabra lleva la primera letra en mayúscula.

<img width="653" height="407" alt="Captura de pantalla 2026-05-21 130518" src="https://github.com/user-attachments/assets/1bd6bc9f-7b3e-47a4-b63d-b4e71e7f9e2d" />

1. Javascript objects: Variables agrupadas
 * Después se pone . x (le dices que vaya a esa variable)
 * En lugar de tener muchas variables sueltas, los objetos funcionan como un "contenedor"   que organiza la información mediante pares de clave y valor.

<img width="467" height="348" alt="Captura de pantalla 2026-05-21 131215" src="https://github.com/user-attachments/assets/89dc0ae2-a686-4738-bf83-a2e7db111edf" />

2. Random()fuction: Devolver numero aleatorio dentro de un rango.
 * Hay 3 tipos:
   * random(): Si no pones nada, devuelve un número decimal entre 0 y 1
   * random(máximo): Devuelve un número decimal entre 0 y el máximo que elijas.
   * random(mínimo, máximo): Devuelve un número decimal entre esos dos valores.
     
3. Width y height: (Ancho y alto) Integradas, corresponden a los valores definidos en el createCanvas.

4. windowWidth, windowHeight: Permite ajustar el tamaño del lienzo al tamaño de la ventana del navegador, se pone en el setup.
   * se pone random(width) y asi solo es random dentro del lienzo.

5. map()fuction: Convierte el valor de un rango a otro(mapear)
 * Sintaxis: map(valor, min original, max original, min_nuevo, max nuevo)
    * valor: La variable que quieres "mapear" (por ejemplo, mouseX).
    * min original y max original: El rango en el que se encuentra ese valor actualmente
    * min nuevo y max nuevo: El rango al que lo quieres transformar.
