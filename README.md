
int reading=0;
void setup()
{Serial.begin(9600);
  pinMode(10,OUTPUT);
  pinMode(5,INPUT);
}

void loop()
{reading=digitalRead(5);
 Serial.println(reading);
 if(reading==HIGH)
   digitalWrite(10,1);
 else
   digitalWrite(10,0);
  
}
