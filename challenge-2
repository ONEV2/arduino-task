void setup()
{
  pinMode(13, OUTPUT);//set pin13 as output
}

void loop()
{
  digitalWrite(13, LOW);
  // temperature sensor input
  if (analogRead(A3) > 300) {
    digitalWrite(13, HIGH);
  } else 
  {
    digitalWrite(13, LOW);
  }
  if (analogRead(A3) < 310) {
    digitalWrite(13, LOW);
  }
  delay(10); // Delay a little bit to improve simulation performance
}
