## Copia y pega esta parte del código:

```cpp
int trig = 7;
int echo = 4;
int led = 10;
int tiempo;
int distancia;

void setup()
{
  pinMode(led, OUTPUT);
  pinMode(trig, OUTPUT);
  pinMode(echo, INPUT);
}

void loop()
{
  digitalWrite(trig, HIGH);
  delay(1);
  digitalWrite(trig, LOW);
  tiempo= pulseIn(echo, HIGH);
  distancia = tiempo / 58.2;  
  
  if (distancia < 50)
  {
    digitalWrite(led, HIGH);
  }
  else
  {
    digitalWrite(led, LOW);
    {
    }
  }
}
```
____
[Regresar al tutorial en el micrositio](#)

[Regresar al tutorial en GitHub](https://github.com/richmf/Tutorial-Arduino-FC-UNAM)
