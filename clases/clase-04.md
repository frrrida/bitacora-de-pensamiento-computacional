# clase 4 
## viernes 17 de abril

  let posx
  let posy 
  son variables que se agregan fuera de setup y draw (puede ser arriba de todo)
  las variables de pueden actualizar por ejemplo agregarle 1 

  puedo alterar la velocidad de reproduccion que por defecto es 60

  **framerate** define que tan rapido van a pasar los frames

  con **frameCount** accedo a la cantidad de frames que han ocurrido desde que se ejecuto el codigo

  al utilizar framecount en donde deberia ir por ejemplo las medidas de una figura esta ira creciendo al ritmo de los frames 

  con  \n creo una nueva linea en el mismo comando
  ej: text("desde que se ejecuto" +  "\n han pasado" +  "\n" + frameCount + " \n frames", width/2, height/2)

  cuando se le agrega el \n antes de una frase esta se irá poniendo abajo (como apretar enter al escribir)

  usamos la variable tinte (fuera del setup y draw)
  let tinte = 0

   
  //actualizamos el valor de tinte
  
  tinte = tinte + 1;
  
  //para reiniciar
  
  if(tinte> 360){
  
    tinte = 0
  }

  //para que el fondo sea un color complementario
  
  if(tinte < 180){
  
    tinteComplementario = tinte + 180
