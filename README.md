# Arduino-press-button-led-on
Arduino press button led on

User ThinkerCard.

#define LED 7
#define BTN 2

int btnEstado;

void setup()
{
  pinMode(LED, OUTPUT);
  pinMode(BTN, INPUT);
}

void loop(){
  btnEstado = digitalRead(BTN);
  
  if(btnEstado == 1){
    digitalWrite(LED, HIGH);
  }else {
  	digitalWrite(LED, LOW);
  }
  
}


