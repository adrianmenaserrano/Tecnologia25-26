# SENSOR PIR.
## FOTO DEL CODIGO
<img width="1303" height="526" alt="image" src="https://github.com/user-attachments/assets/9dfa64d3-aacd-4cda-8e6d-408d17e791a7" />

## VIDEO DE REPRESAENTACION.
[![](https://img.youtube.com/vi/dypxWQvsMdU/0.jpg)](https://www.youtube.com/watch?v=dypxWQvsMdU)

## OBJETOS QUE HEMOS UTILIZADO
- 1 Sensor pir
- 3 cables
- 1 placa arduino
- 1 resistencia

## OBJETIVO
El objetivo del sensor PIR es hacer un detector de movimiento en una sala. Si alguien se esta moviendo pondra en el monitorseries que alguien se esta moviendo y si nadie esta en la sala el monitorseries pondra que nadie se esta moviendo
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
<img width="1303" height="526" alt="image" src="https://github.com/user-attachments/assets/9dfa64d3-aacd-4cda-8e6d-408d17e791a7" />

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
