int tempinput = A0;
float val = 0.0;
float voltageinmv ;
float centigradetemp;
int thresholdtemp = 36;
int outputpin = 13 ;

void setup()
{
  pinMode(A0, INPUT);
  pinMode(13,OUTPUT);
}

void loop()
{
  
  val = analogRead(tempinput);
  voltageinmv = val*(5000.0/1024.0);
  centigradetemp = ((voltageinmv) - 500.0) / 10.0 ;
  if (centigradetemp >= thresholdtemp)
  {
    for (int i=5 ; i>0 ; i++)
    {
      digitalWrite(outputpin , HIGH);
      delay(300);
      digitalWrite(outputpin , LOW);
      delay(300);
    }
   
  }
  else 
  {
    digitalWrite(outputpin , LOW);
  }
  
    
}
