# FOTO DE REPRESENTACION.
<img width="4032" height="3024" alt="image" src="https://github.com/user-attachments/assets/d1acb62d-2067-483e-88ea-f30c07a2b1e6" />

## COMO FUNCIONA ESTA PLATAFORMA ELEVADORA.
El circuito se compondra de estos elementos:
- 4 botones
- 2 posiciones
- 1 valvula de 4 disposiciones
- 1 piston
- 4 bueyes
- 5 entradas de aire y 5 salidas de aire
  ## SU EXPLICACION
Lo que se deberia de hacer es pulsar solo un boton de la izquierda uno solo de la derecha pero da igual el que pulses porque su funcion va a ser siempre la misma.

El circuito empezara con pulsar los dos botones princpales. 

La primera entrada de aire lo que hara es que suba el aire por el conducto llegue a su primera seccion que es donde esta las valvulas de selectura y despues de eso seguiran por el siguiente conducto lleggando a la seccion de dos cuatro donde hay cuatro vias y posiciones de hay llegua al vastago por el lado izquierdo que lo que haria es retraer el pisto asta el limite haciendo que suba la plataforma elevadora.

La segunda entrada seria hacer lo mismo.Ahora el aire va ha entrar por la derecha haciendo que esos dos botones principales arian que al ser pulsados el aire se mueva por todo el lado de su circuito haciendo que suba asta la plataforma elevadora.

La tercera y cuarta empezaran pulsando un boton.

La tercera entrada seria ir directamente hacia la seccion de dos cuatro que pasaria por el conducto hacia el lado dereccho del el vastago haciendo que la plataforma elevadora baje

La cuarta entrada seria con su principal entrada de aire que sube por el conducto donde habria dos disposiciones en este caso el aire pasara el por el conducto hacia la seccion de las valvulas de selectura pasa por el siguiente conducto que llega ha la seccion de dos cuatro y alfinal pasaria por el lado derecho del el vastago haciendo que la plataforma elevadora baje.

La quinta entra  empezaria entrado aire por el conducto lleguando a las dos disposiciones que luego subiria por el conducto llegando a la seccion de las valvulas de selectura.Despues pasaria por el conducto llegando a la seccion de dos cuatro que pasaria y acabaria llendo por la derecha haciendo que bajela la plataforma elevadora.

# EL SENSOR PIR.
# CODIGO DEL SENSOR PIR.
int LED6 = 6;
int PIR = 7;
int lecturaPIR;

void setup() {
Serial.begin (9600);
pinMode (LED6, OUTPUT);
pinMode (PIR, INPUT);

}

void loop() {
lecturaPIR=digitalRead(PIR);
if(lecturaPIR==HIGH){

digitalWrite(LED6, HIGH);

Serial.println("Movimiento detectado");

}

if(lecturaPIR==LOW){
digitalWrite(LED6, LOW);
Serial.println("Movimiento no detectado");

}

delay(100);

}
## EXPLICACION DEL CODIGO
Lo que hace el codigo es que al iniciarse el sensor se activara haciendo que el diodo LED se encienda. Una vez que se encienda el sensor PIR marcara que no hay nadie(si nadie esta dentro de su rango de vista) si en ese rango detecta un movimiento de alguien en la sala pondra en el monitor series "movimiento detectado" y por el contrario si no hay nadie en su rango de vista pondra que"no hay nadie en la sala".

Paara ello hemos empezado poniendo los pines respectivos que sonlos pines 6 y 7 con su respectiva lectura del pir.Una vez puesto los pines toca hacer el void setup que dentro estaria el serial.begin(9600) que es la velocidad de descarga en baudios con el pin 6 de entrada y el pir de salida. Dentro de el voidloop es la que te va ha dar la lectura constante de el sensor PIR. Dentro del el loop tambien esta el if que es una variable para hacer una cosa u otra que en este caso te va a decir que si el LED6 esta en HIGH la lecturadelpir va ha estar en HIGH haciendo que detecte movimiento y si el LED6 esta en LOW la lecturadelpir va ha estar en LOW haciendo que no detecte movimiento.
## VIDEO DE REPRESENTACION
[![](https://img.youtube.com/vi/dypxWQvsMdU/0.jpg)](https://www.youtube.com/watch?v=dypxWQvsMdU)
