## Copia y pega esta parte del código:

```cpp
int led = 13;
int pir = 12;
int pirdato;

void setup()
{
  pinMode(led, OUTPUT);
  pinMode(pir,INPUT);
}

void loop()
{
  pirdato = digitalRead(pir);
  if (pirdato == HIGH)
  {
    digitalWrite(led,HIGH);
  }
  else
  {
    digitalWrite(led,LOW);
  }
  delay(10);
}
```
____
[Regresar al tutorial en el micrositio](#)

[Regresar al tutorial en GitHub](https://github.com/richmf/Tutorial-Arduino-FC-UNAM)
