## Copia y pega esta parte del código:

```cpp
#include <LiquidCrystal.h>

int segundos = 0;

LiquidCrystal lcd_1(12, 11, 5, 4, 3, 2);

void setup()
{
  lcd_1.begin(16, 2); 
  lcd_1.print("!Hola mundo! :)");
}

void loop()
{
  lcd_1.setCursor(0, 1);
  lcd_1.print(segundos);
  delay(1000);
  segundos += 1;
}

```
____
[Regresar al tutorial en el micrositio](#)

[Regresar al tutorial en GitHub](https://github.com/richmf/Tutorial-Arduino-FC-UNAM)
