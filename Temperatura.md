## Copia y pega esta parte del código:

```cpp
const int sensortemp=A0;
const float tempref=24.71;
void setup()
{
Serial.begin(9600);
  for(int numeropin=2;numeropin<5;numeropin++){
    pinMode(numeropin,OUTPUT);
    digitalWrite(numeropin,LOW);
  }
}
void loop()
{
int ValorSensor=analogRead(sensortemp);
Serial.print("Valor del sensor: ");
Serial.print(ValorSensor);
float Tension=(ValorSensor/1024.0)*5.0;
Serial.print(", Voltios: ");
Serial.print(Tension);
float Temperatura=(Tension-0.5)*100;
Serial.print(", Grados C: ");
Serial.println(Temperatura);
  if(Temperatura<tempref){
    digitalWrite(4,LOW);
    digitalWrite(3,LOW);
    digitalWrite(2,LOW);
  }
  else if(Temperatura>=tempref+2&&Temperatura<tempref+4){
    digitalWrite(4,HIGH);
    digitalWrite(3,LOW);
    digitalWrite(2,LOW);
  }
    else if(Temperatura>=tempref+4&&Temperatura<tempref+6){
    digitalWrite(4,HIGH);
    digitalWrite(3,HIGH);
    digitalWrite(2,LOW);
  }
  else if(Temperatura>=tempref+6){
    digitalWrite(4,HIGH);
    digitalWrite(3,HIGH);
    digitalWrite(2,HIGH);
  }
  delay(100);
}

```
____
[Regresar al tutorial en el micrositio](#)

[Regresar al tutorial en GitHub](https://github.com/richmf/Tutorial-Arduino-FC-UNAM)
