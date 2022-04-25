## Copia y pega esta parte del código:

```cpp
// C++ code
//
int rojo=12;
int amarillo=11;
int verde=10;
void setup()
{
  pinMode(rojo, OUTPUT);
  pinMode(amarillo, OUTPUT);
  pinMode(verde, OUTPUT);
}
void loop()
{
  digitalWrite(rojo, HIGH);
  digitalWrite(amarillo, LOW);
  digitalWrite(verde, LOW);
  delay(6000); 
  digitalWrite(verde, HIGH);
  digitalWrite(rojo, LOW);
  digitalWrite(amarillo, LOW);
  delay(4000); 
  digitalWrite(amarillo, HIGH);
  digitalWrite(verde, LOW);
  digitalWrite(rojo, LOW);
  delay(2000); 
}
```
____
[Regresar al tutorial en el micrositio](#)

[Regresar al tutorial en GitHub](https://github.com/richmf/Tutorial-Arduino-FC-UNAM)
