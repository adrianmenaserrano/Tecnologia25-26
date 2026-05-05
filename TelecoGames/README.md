# SENSOR PIR.
## FOTO DEL CODIGO
<img width="1303" height="526" alt="image" src="https://github.com/user-attachments/assets/9dfa64d3-aacd-4cda-8e6d-408d17e791a7" />

## VIDEO DE REPRESENTACION.
[![](https://img.youtube.com/vi/dypxWQvsMdU/0.jpg)](https://www.youtube.com/watch?v=dypxWQvsMdU)

## OBJETOS QUE HEMOS UTILIZADO
- 1 Sensor pir
- 3 cables
- 1 placa arduino
- 1 resistencia

## OBJETIVO
El objetivo del sensor PIR es hacer un detector de movimiento en una sala. Si alguien se esta moviendo pondra en el monitor series que alguien se esta moviendo y si nadie esta en la sala el monitorseries pondra que nadie se esta moviendo
  - --------------------------------------------------------------------------------------------------------------------------------------

# SENSOR DE LUZ
## CANTIDAD DE LUZ CON LA LDR
## CODIGO DEL LDR
int LED6 = 6; // el pin 6

int LDR = 7; // el pin 7, por donde entra los datos de el sensor LDR

int lecturaLDR; // variable donde se guardan los datos de la lectura del LDR

void setup() { // se encarga de la configuracion inicial, se ejecuta solo una vez al inicio

Serial.begin (9600); // velocidad de descarga de información baudios

pinMode (LED6, OUTPUT); // pin 6 de salida

pinMode (PIR, INPUT); // pin 7 de entrada

}

void loop() { // hace que lo que se halle dentro se ejecuta infinitamente mientras la placa este encendida

lecturaPIR=digitalRead(PIR); /* se hace una lectura del PIR y se le da el valor a la variable 'lecturaPIR'; HIGH(detectado) y 
                                LOW(no detectado) */

if(lecturaPIR==HIGH){ // "si la lectura de PIR = HIGH(detectado) entonces..."

digitalWrite(LED6, HIGH); // da corriente al pin 6 para encender el led

Serial.println("Movimiento detectado"); // mostrar en el monitor serie "movimiento detectado"
}
if(lecturaPIR==LOW){ // "si la lectura de PIR = LOW(no detectado) entonces..."

digitalWrite(LED6, LOW); // le quita la corriente al pin 6 para apagsr el led

Serial.println("Movimiento no detectado"); // mostrar en el monitor serie "movimiento no detectado"
}
delay(100); // esperar 0.1 segundos antes de repetir el void loop
}
 


## EXPLICACION DEL CODIGO
Lo que hace el codigo es que gracias al Monitor series el ldr sube o baja la intensidad a medida que haya más luz o menos luz para ello deberiamos de usar sus respectivas variables y su bucle que l oque hace es que marque constantemente la intensidad de iluminacion que tiene el ldr.
Su montaje fue bastante complicado porque tuvimos unos problemas con el montaje por que no supimos por donde empezar pero alfinal con la cordinacion del grupo acabamos encontrando solucionnes a los problemas que teniamos anteriormente

## VIDEO REPRESENTATIVO
[![](https://img.youtube.com/vi/m-Ui3pkOT5Y/0.jpg)](https://www.youtube.com/watch?v=m-Ui3pkOT5Y)

## OBJETOS QUE HEMOS UTILIZADO

- 1 LDR

- 2 CABLES

- 1 RESISTENCIA

## FOTO DEL CODIGO DEL SENSOR DE LUZ.
![ldr_real](https://github.com/user-attachments/assets/b03714f8-2e7d-49d8-94d0-2f3f1d1623c0)

## EL OBJETIVO
La idea hera coger una ldr y con su respectivo codigo hacerle que si tapabas la ldr con tus manos o con un objeto para que no le pase luz los núeros que va marcando en el MonitorSeries bajen y por el contrario si no tapas la ldr con nada como la luz llega los valores que hay en el MonitorSeries suban.


-----------------------------------------------------------------------------------------------------------------------------------------

# SENSOR DE PRESION
## EXPLICACION DEL CODIGO
Lo que hace este sensor es que con el monitorseries va ha marcar la cantidad de rayos ultravioleta que hay de pendiendo si detecta más rayos ultravioleta el monitorseries detectara más o si no detecta tantos rayos ultravioleta como antes el monitorseries detectara menos.

## CODIGO DEL SENSOR DE PRESION
<img width="1303" height="526" alt="Screenshot 2026-02-12 111343" src="https://github.com/user-attachments/assets/bbb4e979-e21c-4bbb-b20e-d415fdb87100" />

## VIDEO DEL SENSOR DE PRESION
[![](https://img.youtube.com/vi/nafKf1urKBM/0.jpg)](https://www.youtube.com/watch?v=nafKf1urKBM).

## OBJETOS QUE HEMOS UTILIZADO
- 5 CABLES
- 1 RESISTENCIA
- 1 PLACA ARDUINO
- 1 DETECTOR DE PRESION

## EL OBJETIVO
El sensor de presion como su nombre indica habia que hacer que si con tu dedo o con un objeto presionas en senor marcara un número elevado en el MonitorSeries haciendo referencia a la presion que lleva y por el contrario si no lo pulsas el número bajara.

-----------------------------------------------------------------------------------------------------------------------------------------

# SENSOR DE SONIDO
## CODIGO DEL SENSOR DE SONIDO
<img width="1303" height="526" alt="image" src="https://github.com/user-attachments/assets/2202bdc4-20f1-4288-8af7-ca7dc6c5bda5" />

## VIDEO DEL SENSOR DE SONIDO
[![](https://img.youtube.com/vi/E7mlcuRCIkQ/0.jpg)](https://www.youtube.com/watch?v=E7mlcuRCIkQ).

## OBJETOS QUE HEMOS UTILIZADO
- 4 cables
- 1 placa arduino
- 1 sensor de sonido

## EL OBJETIVO
Lo que quisimos hacer y lo que hace este sensor es que si le ponemos un sonido fuerte al sensor lo que hara es que sus número suban mucho en el MonitorSeries y por el contrario si no hay ningun sonido a su alrededor sus números bajaran.

----------------------------------------------------------------------------------------------------------------------------------------

# SENSOR DE GAS
## CODIGO DEL SENSOR DE GAS
<img width="1303" height="526" alt="image" src="https://github.com/user-attachments/assets/9412272a-ee16-42e0-b967-00c9b6d7192c" />

## VIDEO DEL SENSOR DE GAS
[![](https://img.youtube.com/vi/xSIciQBGbRE/0.jpg)](https://www.youtube.com/watch?v=xSIciQBGbRE)

## OBJETOS QUE HEMOS UTILIZADO
- 4 cables
- 1 placa arduino
- 1 sensor de gas

  ## EL OBJETIVO
  El objetivo con sensor de gas es que si ponemos algun tipo de gas en el sensor los valores en el MonitorSeries subiran pero por el contrario si no hay ningun tipo de gas en el sensor el los valores bajaran
-----------------------------------------------------------------------------------------------------------------------------------------

 # SENSOR DE HUMEDAD
 ## CODIGO DEL SENSOR DE HUMEDAD
<img width="1303" height="526" alt="image" src="https://github.com/user-attachments/assets/2202bdc4-20f1-4288-8af7-ca7dc6c5bda5" />

## VIDEO DEL SENSOR DE HUMEDAD
[![](https://img.youtube.com/vi/yI6TIqMYskk/0.jpg)](https://www.youtube.com/watch?v=yI6TIqMYskk).

##  OBJETOS QUE HEMOS UTILIZADO
- 4 cables
- 1 placa arduino
- 1 sensor de humedad

## EL OBJETIVO
Este ultimo sensor lo que hace es ponerlo en la tierra y dependiendo si tiene más humedad o menos los numeros apereceran en el MonitorSeries.Si tienen más humedad subirian los números y si tienen menos bajarian.

-----------------------------------------------------------------------------------------------------------------------

# PROYECTO FINAL: EL INVERNADERO
En este projecto hemos echo un invernadero con piezas echas en tinkercad con el objetivo de hacer como en un puzzle hacer que las piezas se puedan unir entre si. Para ello nos tuvimos que repartirnos que figura hiba ha hacer cada uno pero que todos tengan la misma medida. El suelo que hemos escogido es un suelo normal para que no afecte a la hora de poner las vigas. Mi parte fue hacer unas vigas que tengan 2 entradas para poder meter los salientes y en el otro extremo de la pieza hacer un saliente para que al unirlas con otras figuras de mis compañeros se puedan unir sin problemas.Una vez que el profe imprimio las figuras las tubimos que limar para que puedan entrar.Y cuando ya terinamos de limar comprobamos si se podian meter sin problemas y alfinal si se podia. Lo ultimo que queda es unir todas las piezas para hacer la forma de un invernadero funcional.

## FOTO DE REPRESENTACION DE MI FIGURA
<img width="605" height="232" alt="image" src="https://github.com/user-attachments/assets/b19b064a-1b18-47ca-b9ff-94f9d0459f05" />

## MEDIDAS DE LAS FIGURAS
Las figuras ue hemos echo son tanto de largo como de hancho de 15 cm y de alto unos 5 cm.

## FOTOS DEL SUELO DEL 
<img width="1273" height="463" alt="image" src="https://github.com/user-attachments/assets/613d4618-2466-4e4e-91fb-01521b507ae5" />

## EXPLICACION DE COMO FUNCIONA EL SUELO
Para ello lo que hemos echo a sido hacer un suelo de 150 cm x 150cm. Luego colocamos unas viseras de 5cm,hacia arriba y a la derecha del suelo para que quepan con las otras piezas de otros suelos.Tambien emos hecho otra viseras transparentes para luego unirlas y hacer un hueco para unirlas con otros suelos como si fuese un puzzle.

## RESUELTADO FINAL DEL PROYECTO DEL INVERNADERO EN TINKERKCAD
<img width="813" height="379" alt="image" src="https://github.com/user-attachments/assets/44d31f94-eb76-4cda-b6eb-67ba0ee87fea" />

El proyecto final del invernadero seria que quede más o menos asi pero con la diferencia de que en este caso hay que hacerlo funcional para que pueda detectar:humeda,calor,cuando necesitan agua,etc pero lo más importante e que sea funcional y si las cosas salen bien trasladarlo a la vida real haciendolo igual al prototipo de tinkerkad con sus mismo sensores,con su misma forma y de la misma manera en la que nos repartimos el trabajo. Si lo llegamos ha hacer para ello pondremos en practica todo lo que hicimos con los sensores de humeda,gas,ultravioleta,etc.

## FOTOGRAFIA DE COMO SE VA IMPRIMIENDO UNA FIGURA
<img width="1139" height="641" alt="image" src="https://github.com/user-attachments/assets/3af7ca7a-2bf2-44f7-ba7c-c2555d104b80" />

Por lo que se puede ver en esta imagen lo que se esta haciendo es la impresion 3D de la planta(suelo) de el invernadero en miniatura que estamos haciendo tanto en tinkercad como con ayuda de la impresora lo estamos haciendo tambien ha mano

# FOTO  DEL INVERNADERO CON LAS BASES Y LOS PILARES PUESTOS
<img width="646" height="358" alt="image" src="https://github.com/user-attachments/assets/779e0c20-7a51-4e6a-a2f4-43dc647b62cc" />

# PARTES QUE HEMOS USADO PARA HACER EL INVERNADERO FUNCIONAL
## LA BATERIA
<img width="633" height="318" alt="image" src="https://github.com/user-attachments/assets/546fee1c-3659-46a9-930d-9efda0405f4c" />

## LA BOMBA DE AGUA
<img width="662" height="374" alt="image" src="https://github.com/user-attachments/assets/7d293728-6812-4748-889d-767c5e7832f8" />

## EL CÓDIGO
<img width="1218" height="896" alt="Captura de pantalla 2026-04-09 103125" src="https://github.com/user-attachments/assets/04a1eacd-2abe-49a3-89b2-1ccdd8ca94d9" />

Lo que hace el codigo va a ser lo siguiente: mediante el codigo te va a decir que la planta necesita agua porque va ha ver un diodo azul que se va ha encender una ve que se encienda la planta te pedira agua entoces con la ayuda de la bomba de agua le va ha bombear agua ha la planta asta que ya este llena entonces la bomba parara de bombear.

Para todo esto hemos tenido que usar un relé para que nos ayude con el tiempo que tiene la bomba de agua en bombear antes de que la planta se ahogue.Luego también emos usado el sensor de humedad que lo que hara es detectar si la planta tiene en la tierra mucha agua o poca agua si tiene mucha agua no bombeara agua y si tiene poca agua bombeara más agua y asi asta que la bomba de agua se quede sin agua.

## EL INVERNADERO DESDE DISTINTOS LADOS
<img width="646" height="357" alt="image" src="https://github.com/user-attachments/assets/d9d51dfe-0508-4a1a-a5af-22012bca69cf" />

# FOTO DE LOS SENSORES.
<img width="637" height="352" alt="image" src="https://github.com/user-attachments/assets/8807636a-87a1-4896-a0fc-dd4a37902b7d" /> <img width="650" height="346" alt="image" src="https://github.com/user-attachments/assets/b76bc348-94ea-4f22-b21c-3328089551a9" />



# VIDEO DE REPRESENTACION DE COMO QUEDARIA.
[![](https://img.youtube.com/vi/rl1b3eS5mnE/0.jpg)](https://www.youtube.com/watch?v=rl1b3eS5mnE)
## CODIGOS DEL MAESTRO Y EL ESCLAVO.
## MAESTRO:
<img width="430" height="307" alt="image" src="https://github.com/user-attachments/assets/0d7709f9-2b5e-4ed7-bb4b-5badb9c47602" />

# ESCLAVO:
<img width="264" height="325" alt="image" src="https://github.com/user-attachments/assets/ff1c6387-89c6-484b-9f1b-184bbf328b23" />

# EXPLICACION DEL CODIGO
## ¿QUE HACE EL MAESTRO?
Para empezar cogemos el softwere serial.h de la libreria una vez hecho le poneos el nombre miBt( asi nos referimos al bluetooth) cuando hallamos echo eso empezamos con las variables del sensor de temperatura,humedad y de nivel de agua.Luego colocareos los pines de entrada que son el led 5, el rele 2 y el leddeagua que es el 6.

Ahora tenemos el voidSetup es una cosa que cada vez que iniciemos la placa se activara solo una vez es lo que por asi decirlo da vida al codigo entonces una vez que sabes esto lo que hace este voidsetup es lo siguiente. Con el serialbegin es marcarte la velocidad en la que el bluetooth le llegan los datos que tu quieres enviarle (más en expecifico son 9600 baudios). Luego dentro de ahi tenemos los pinMode que lo que te dice como deberian en este caso los dos leds y el rele que lo que te dicen es que estan de salida.

Ahora nos metemos en el voidloop que lo que hace es que todo lo que metamos de codigo en esa parti se va ha repetir constantemente.Entonces vamos a poner el entradadeagua en una analogread para que este leyendo constante mente el ledagua. Luego pondremos que agua=map eso lo que hace es que este mapeando el nivel de agua que haya pero con la idea de que en vez de que te marque con números muy grades te marcara con el porcentaje de agua que tenga la planta.

Luego tenemos lo mismo pero con el de temperatura que lo que hace es decirte a cuantos grados esta la planta o si hae temperaturas muy altas muy bajas o esta normal. Y ya por ultimo esta el de humedad que hace lo mismo que los anterires que con porcentajes que luegon aparecen en el monitorSeries te mmarcara el porcentaje de humedad que tiene la planta.

Despues de contar que hace los distintos sensores le daremos un delay a miBT.print (agua) que es lo que manda en base de codigo o texto el bluetooth.(Hay que tener en cuent de que el relé esta funcionando al reves para hacer que funcione correctamente).
Ahora toca la parte de los if el if es la parte que te dice si pasa una cosa hace esto pero si pasa otra cosa hace lo otro es una estructura que controla las opciones que tiene.
Una vez explicado eso lo que hace este if es que si el nivel de agua es menor que 30 se para todo y el led azul se encendera diciendo que necesita agua.
pero por el contrario si el nivel de agua es bueno paramos el led azul y vemos si necesita más agua o menos todo esto se hace mediante digitalWrite que como he explicado antes la funcion es decir si estan encendidos o apagados.Asi va a ser lo mismo tanto con el de temperatura como con el de humedad si es mayor de lo debido se para todo y se enciende el led azul  y si esta todo sobresaturado activamos el led rojo como advertencia y se enciende el relé y ya todo esto ponemos un delay de 20 milisegundos.

## ¿COMO FUNCIONA EL ESCLAVO?
El exclavo es lo mismo solo con la diferencia de que el al ser el esclavo es el que recibe las señales del maestro por lo tanto es el que menos codigo tiene entonces una vez sabido eso lo que hace el esclavo es. 


ponemos en la libreria el SoftwareSreial.h al igual que en el maestro y ponemos el int del ledagua en el 5 y el int en el led de temperatura en el 6 estos dos led vayan al 5 y al 6 el led agua es el diodo led azul y el de temperatura es el diodo led rojo.

Despues esta el void setup que empieza con el serialbeging que esta en (9600) baudios que es la velocidad de descarga,luego esta el miBT.begin que hace lo mismo que el seril.beging solo que va para los modulos bluetooth y por ultimo los pinmodes hacen que los leds de temperatura y agua se activen y ademas controlen el voltaje que puedan llegar a soportar eso leds.

Luego esta el voidloop que lo que hay dentro son ifs que lo que te explican es que si esto pasa hara esta cosa y sino pasa hara la segunda opcion. Una vez dicho para que sirven te explico que hay en los ifs. En el primer if lo que hay es un miBT.avaliable que lo que hace es enviarle señales al serial.write(miBT) para que el serial.write pueda escribirlo y pasarlo al monitorSeries pero si el dato es 1 escribira que el led agua esta encendido y por el contrario si dato es 2 el ledagua estara apagado. Tambien pasa con el ledtemperatura si el dato es 4 el ledtemperatura estara encndido y por el contrario si dato es 5 el ledtemperatura estara apagado
