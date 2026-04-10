# SOLEMNE-1

### LINK PROYECTO p5.js
https://editor.p5js.org/tomas1000000/sketches/xr7dZxcj7

## PROCESO
Primero trasladé el dibujo a Adobe Illustrator, en un lienzo de 500 x 500, donde lo vectoricé para limpiar las formas y obtener una versión digital más clara y precisa. Este paso fue clave para simplificar la imagen en figuras geométricas bien definidas. Luego, a partir de ese archivo vectorial, identifiqué y extraje las coordenadas de cada elemento, considerando sus posiciones, tamaños y proporciones dentro del lienzo. Con esa información, pude reconstruir el diseño en p5.js utilizando únicamente comandos básicos de dibujo, trasladando fielmente la composición original al entorno digital mediante coordenadas exactas.


## DIFICULTADES
Una de las principales dificultades fue adaptarme al uso de coordenadas dentro del programa, ya que habia que pensar el dibujo de forma de coordenadas como las daba Illustrator. Tuve que aprender cómo se posicionan los elementos en el lienzo con sistema de ejes y cada valor y tamaño de las figuras. Además, también fue un desafío conocer con los comandos de p5.js, ya que no tenía experiencia con JavaScript ni ningún otro lenguaje de programación. Esto significo un proceso de prueba y error, probando distintas instrucciones y corrigiendo errores constantemente hasta lograr que las formas se ubicaran correctamente y el resultado final se asemejara al diseño original.




## CODIGO
function setup() {
  createCanvas(500, 500); // TAMAÑO LIENZO
  angleMode(DEGREES); 
  background(240); // COLOR FONDO
  noStroke(); // SIN BORDES EN FIGURAS

  // RECTÁNGULO ROJO
  fill(150, 30, 30); // COLOR ROJO
  rect(70, 0, 60, 120); // DIBUJA UN RECTANGULO

  // BLOQUE DIAGONAL AZUL
  fill(35, 45, 90); // COLOR AZUL
  quad(70, 130, 130, 130, 250, 270, 190, 270); // DIBUJA UN ROMBO

  // RECTANGULOS IZQUIERDA
  fill(35, 45, 90); // COLOR AZUL
  rect(0, 280, 50, 130); // DIBUJA UN RECTANGULO
  fill(0); // COLOR NEGRO
  rect(50, 280, 50, 130); // DIBUJA UN RECTANGULO

  // CUADRICULA
  fill(35, 45, 90); //COLOR AZUL
  square(100, 340, 20); // DIBUJA UN CUADRADO
  square(120, 320, 20); // DIBUJA UN CUADRADO
  square(140, 300, 20); // DIBUJA UN CUADRADO
  square(160, 280, 20); // DIBUJA UN CUADRADO
  square(160, 340, 20); // DIBUJA UN CUADRADO

  fill(0); //COLOR NEGRO
  square(140, 280, 20); // DIBUJA UN CUADRADO
  square(140, 340, 20); // DIBUJA UN CUADRADO
  square(140, 360, 20); // DIBUJA UN CUADRADO
  square(140, 380, 20); // DIBUJA UN CUADRADO
  square(140, 390, 20); // DIBUJA UN CUADRADO
  square(160, 320, 20); // DIBUJA UN CUADRADO

  // CUADRADOS CENTRO
  fill(0); // COLOR NEGRO
  rect(260, 320, 70, 100); // DIBUJA UN RECTANGULO
  rect(330, 270, 20, 150); // DIBUJA UN RECTANGULO

  fill(150, 30, 30); // COLOR ROJO
  rect(290, 320, 30, 100); // DIBUJA UN RECTANGULO

  // LÍNEA
  fill(0); // COLOR NEGRO
  rect(350, 270, 150, 4); // DIBUJA UN RECTANGULO

  // TRIÁNGULOS
  fill(150, 30, 30); // COLOR ROJO
  triangle(350, 270, 410, 270, 380, 300); // DIBUJA UN TRIANGULO
  triangle(350, 300, 410, 300, 380, 330); // DIBUJA UN TRIANGULO
  triangle(350, 330, 410, 330, 380, 360); // DIBUJA UN TRIANGULO

  // TRIÁNGULO GRANDE ROJO
  fill(150, 30, 30); // COLOR ROJO
  triangle(440, 170, 500, 500, 370, 500); // DIBUJA UN TRIANGULO

  // CIRCULOS GRILLA
  fill(0); // COLOR NEGRO
  circle(320, 80, 40); // DIBUJA UN CIRCULO
  circle(380, 110, 40); // DIBUJA UN CIRCULO
  circle(340, 150, 40); // DIBUJA UN CIRCULO
  circle(380, 150, 40); // DIBUJA UN CIRCULO
  circle(340, 190, 40); // DIBUJA UN CIRCULO
  circle(380, 190, 40); // DIBUJA UN CIRCULO
  
  // CIRCUNFERENCIA
  fill (0) // COLOR NEGRO
  arc(100,100 , 150, 150, 0 ,270) // DIBUJA UN MEDIO CIRCULO


  // RECTÁNGULO INFERIOR NEGRO
  fill(0); // COLOR NEGRO
  rect(150, 430, 50, 80); // DIBUJA UN RECTANGULO

  // RECGTANGULO HORIZONTAL NEGRO
  fill(0); // COLOR NEGRO
  rect(180, 320, 110, 20); // DIBUJA UN RECTANGULO
}
