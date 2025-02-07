int led11=11;
int led12=12;
int led13=13;
int button=2;
int greentime=1000;
int yellowtime=1000;
int redtime=1000;
long time=0;
long ct=0;
void setup()
{
  pinMode(led11, OUTPUT);
  pinMode(led12, OUTPUT);
  pinMode(led13, OUTPUT);
  pinMode(button,OUTPUT);
  Serial.begin(9600);
}

void loop()
{
  int signal=digitalRead(button);
  if(signal==HIGH){
    Serial.println("Pedestrian crossing the road!!");
    digitalWrite(led13,HIGH);
    digitalWrite(led12,LOW);
    digitalWrite(led11,LOW);
    delay(3000);
    
  }
  else if(signal==LOW){
    //for green light
    time+=greentime;
    while(ct<time){
    digitalWrite(led11,HIGH);
    digitalWrite(led12,LOW);
    digitalWrite(led13,LOW);
    ct=millis();
    }
    
    //for yellow light
    time+=yellowtime;
    while(ct<time){
    digitalWrite(led11,LOW);
    digitalWrite(led12,HIGH);
    digitalWrite(led13,LOW);
    ct=millis();
    }
    
    //for red light
    time+=redtime;
    while(ct<time){
    digitalWrite(led11,LOW);
    digitalWrite(led12,LOW);
    digitalWrite(led13,HIGH);
    ct=millis();
    }
  }
}
