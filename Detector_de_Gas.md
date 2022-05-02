## Copia y pega esta parte del código:

```cpp
// C++ code
//
int gas;
int piezo = 13;
void setup()
{
  pinMode(A0, INPUT);
  pinMode(piezo, OUTPUT);
}

void loop()
{
  gas = analogRead(A0);
  if (gas >=600)
  	{
    tone(piezo, 523, 200);
    delay(500);
  	}
}
```
____
[Regresar al tutorial en el micrositio](#)

[Regresar al tutorial en GitHub](https://github.com/richmf/Tutorial-Arduino-FC-UNAM)
