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

int PIR = 7; // el pin 7, por donde entra los datos de el sensor PIR

int lecturaPIR; // variable donde se guardan los datos de la lectura del PIR

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
Para ello lo que hemos echo a sido hacer un suelo de 150 cm x 150cm. Luego colocamos unas viseras de 5cm,hacia arriba y a la derecha del suelo para que quepan con las otras piezas de otros suelos.Tambien emos echo otra viseras transparentes para luego unirlas y hacer un hueco para unirlas con otros suelos como si fuese un puzzle.

## RESUELTADO FINAL DEL PROYECTO DEL INVERNADERO EN TINKERKCAD
<img width="813" height="379" alt="image" src="https://github.com/user-attachments/assets/44d31f94-eb76-4cda-b6eb-67ba0ee87fea" />

El proyecto final del invernadero seria que quede más o menos asi pero con la diferencia de que en este caso hay que hacerlo funcional para que pueda detectar:humeda,calor,cuando necesitan agua,etc pero lo más importante e que sea funcional y si las cosas salen bien trasladarlo a la vida real haciendolo igual al prototipo de tinkerkad con sus mismo sensores,con su misma forma y de la misma manera en la que nos repartimos el trabajo. Si lo llegamos ha hacer para ello pondremos en practica todo lo que hicimos con los sensores de humeda,gas,ultravioleta,etc.

## FOTOGRAFIA DE COMO SE VA IMPRIMIENDO UNA FIGURA
<img width="1139" height="641" alt="image" src="https://github.com/user-attachments/assets/3af7ca7a-2bf2-44f7-ba7c-c2555d104b80" />

Por lo que se puede ver en esta imagen lo que se esta haciendo es la impresion 3D de la planta(suelo) de el invernadero en miniatura que estamos haciendo tanto en tinkercad como con ayuda de la impresora lo estamos haciendo tambien ha mano
