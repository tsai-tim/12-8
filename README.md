# 12-8
void setup() {
  // put your setup code here, to run once:
  pinMode(2,OUTPUT);//IN3
  pinMode(5,OUTPUT);//IN1
  pinMode(6,OUTPUT);//IN2
}

void loop() {
  // put your main code here, to run repeatedly:

 forw(200);
 delay(600);
 brake();
 delay(2500);
 rev(200);
 delay(600);
 
}
void forw(int f){
  analogWrite(9,f);
analogWrite(10,0);
}
void rev(int f){
  analogWrite(9,0);
analogWrite(10,f);
}
void brake(){
  analogWrite(9,255);
analogWrite(10,255);}
