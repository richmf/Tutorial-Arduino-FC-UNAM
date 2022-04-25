## Copia y pega esta parte del código:

// C++ code
//
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
  distancia = tiempo / 58.2;  //Convertir el tiempo en centimetros
  
  if (distancia < 50)
  {
    digitalWrite(led, HIGH);
  }
  else
  {
    digitalWrite(led, LOW);
    {
    }
  digitalWrite(led, HIGH);
  delay(2000); 
  digitalWrite(led, LOW);
  delay(1000);
  }
}

[Regresar al tutorial en el micrositio](#)

[Regresar al tutorial en GitHub](https://github.com/richmf/Tutorial-Arduino-FC-UNAM)
