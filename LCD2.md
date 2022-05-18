## Copia y pega esta parte del código:

```cpp
#include <LiquidCrystal.h>

int temp = 0;
float tempC = 0;
int sensortemp = A0;

LiquidCrystal lcd_1(12, 11, 5, 4, 3, 2);

void setup()
{
  lcd_1.begin(16, 2);
  lcd_1.print("Temperatura");
  pinMode(sensortemp, INPUT);
}

void loop()
{
  lcd_1.setCursor(0, 1);
  temp = analogRead(sensortemp);
  tempC = (temp*0.48828125)-50;
  lcd_1.print(tempC);
}
```
____
[Regresar al tutorial en el micrositio](#)

[Regresar al tutorial en GitHub](https://github.com/richmf/Tutorial-Arduino-FC-UNAM)
