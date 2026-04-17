# clase 02

## apuntes de la clase 

podemos hacer que el tamaño del lienzo se ajuste al tamaño de la ventana
//createCanvas(windowWidth , windowHeight)

con 3 argumentos va a ser RGB
para cambiar modo de color se usa colormode
//(HSB, 360,100,100,100)
//(modo,maxsaturacion,maxbrillo,maxopacidad)
si el brillo está en 0 se ve negro

hay 2 parametros que son nativos widht y height
widht es el ancho del canvas (sirve por si cambio el ancho del lienzo)
height es el alto del canvas (por si cambio el alto del lienzo)
si quiero que esté a la mitad height/2 o widght/2 en los puntos x e y 
  
puedo volver parametro del ancho o largo cualquier variable
para el tamaño tambien lo puedo ocupar

puedo agregarle el - para que se mueva esa cantidad de puntos

funcion de vertives:vertex
necesita estar encerrada entre beginShape (), y endShape()

siquiero que la figura quede bien cerrada debo incluir el inicio
tambien puedo agregar CLOSE como argumento en endShape
  
text ("palabras en comillas dobles",pos X, pos Y)

  fill da relleno, noFill es relleno transparente
  
  textAlign(alineacionhorizontal,alineacionvertical)
  
  textFont(´tipo de fuente´)con comilla simple no doble
  existen ´monoespaciado´, ´serif´ y ´sans serif´

  tambien se pueden cambiar los estilos con textStyle

  las rotaciones trabajan en radiantes, en grados de 0 a 360
  al rotar, roto desde el eje de cordenada
  se usa angloMode(DEGREES)

  puch y pop sirven para asignar colores,rellenos o contorno y que no afecte a lo que está fuera de eso
