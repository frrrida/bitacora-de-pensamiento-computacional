# Apuntes clase 5

## primera parte
le ponemos "let" a variables fuera del setup 
ej: let saldo= 100 para q al agregarlas en el setup solo con poner "saldo" sepa cual es el valor de ese 

print para que la info salga en la consola 

print ("el precio del pasaje es"+ preciopasaje)


if para cuando el caso si ocurre

else if o else para caundo el caso no ocurra

ej: if( saldo > precioPasaje){
textSize(50)
text("BIP", width/2, heigth/2)
} 
else{
textSize(50)
text("NO BIP", width/2,heigth/2)
} 

frameRate () para decidir la velocidad en q van a pasar las cosas 


podemos cambiar tdo al draw en vez del setup para que ocurra todo el rato y no solo al precionar 


podemos ponerle random a un dato entre las cantidades qeu queremos 
ej: saldo= random (0, 1000)

frameCount es el valor de los frames que han pasado


para trabajar con colores en variables se declaran fuera del setup los nombres de los colores
ej: 
let rojo
let verde

luego dentro del setup le pongo el mismo nombre y asigno el color incluyendo la palabra "color"
ej:
rojo = color(240,0,0)
verde= color(0,255,0)

si queremos q los colores varien segun nuestras condiciones (if o else) las agregamos en esa parte 

## segunda parte

line(x1, y1, x2, y2)

para hacer una linea en el tercio del lienzo
line(width/3, 0, width/3, height) van haciendose de arriba hacia abajo

liena a los 2/3
line(width*2/3, 0, width *2/3, height)

puedo generar una figura en dondde pasa mi mouse por el lienzo 
ej: ellipse(mouseX, mouseY, 20, 20) 

ponemos mouseX y mouseY en dnde deberian ir las cordenadas para q estas dependan de la ubicación del mouse 

para esconder el mouse usamos noCursor en el setup

para cambiar el color de fondo creamos una variable(fuera del setup) para eso llamada 

let colorFondo 

y tambien agregamos colores 

let color 1

let color 2

let color 3

luego dentro del setup vamos a llenar de esos colores 
colorFondo= color(0,0,0)
color1= color(123,200,30)
color2= color(90,123,50)
color3= color(20,20,180) 

en el draw ponemos en el background(colorFondo)
siempre vamos a pintar el fondo con el color de fondo


(posMouseX) la posicion del mouse en x 

podemos poner condiciones q se deben cumplir de las q va a depender el color q se vea 
por ejemplo en los tercios q separamos en el lienzo

if(posMouseX < width/3){
colorFondo= color1
}

if(posMouseX > width/3){
colorFondo= color2 
}

if(posMouseX > width*2/3){
colorFondo= color3 
}

operador AND 
se debe cumplir mas de una cosa para que funcione

operador OR
basta con q se cumpla una para q funcione

con el operador OR integramos dos condiciones en una y ocurrirá siempre q se gatille cualquiera de las dos q yo meta dentro
ej: if(posMouseX < width/3 || posMouseX > width*2/3) 


## parte tres

podemos hacer margenes en el lienzo 
fuera del setup ponemos
let margenIzq= 10
let margenDer= 100

dentro del draw le ponemos los valores a estos margenes 
margenIzq= width/5
margenDer= width* 4/5

para poder visualizar eso dibujamos lineas en esos margenes
con 
line(margenIzq, 0, margenIzq, height)
line(margenDer, 0, margenDer, height)

asi es mas facil para cambiar los margenes desde los valores q le dimos


para agregar una imagen agegamos primero una variable fuera del setup q diga
let + un nombre para luego agregar la imagen
ej: let don

luego dentro del setup ponemos
don= loadImagen("./nombredelarchivo.jpg")
don= loadImagen("./donFrancis.jpg")

dentro del draw vamos a poner la imagen como tal incluyendo la variable q hicimos en el setup

image(don, 0,0,100,100)
le agregamos parametros por ejemplo para el ancho y alto de la imagen 
image(img, x, y, [width], [height])

para hacer q la imagen se mueva con el mouse en vez de poner 0,0 ponemos
image(don, mouseX, mouseY, 100,100)

funciones: 
mousePressed ocurre cuando preciono el mouse
mouseReleased ocurre cuando suelto el mouse 
ambos deben  ir antes con la palabra funcion como el setup o draw y llevar () y {}

ej:

function mousePressed() {

}


ek background en draw constantemente se regenera en cambio en setup solo se genera una vez y todo lo q pase encima va a verse 


para cambiar la posicion de la imagen podemos crear variables (fuera del setup) y le ponemos ahi los valores
esto remplazaria las cordenadas 
ej:
let posX=0
let posY=0 

actualizamos la posicion de la imagen para q se mueva poniendo dentro del draw

posX = posX + numero para la velocidad q queremos q se mueva
posX = posX + 2

podemos crear una variable para guardar la direccion llamada 
let dirX = 

dir es hacia la derecha si es 1 y hacia la izq si es -1

con esto podemos hacer por ejemplo q la imagen se devuelva desde un punto exacto invirtiendo su dirección




























































