#define BLYNK_PRINT Serial 
#define BLYNK_TEMPLATE_ID "TMPL6fXbxj6_o"
#define BLYNK_TEMPLATE_NAME "Control LED"
#define BLYNK_AUTH_TOKEN "7LlbHcJ0ghrkOA3MsQw5KcPDfCH12GQr"
#include <ESP8266WiFi.h> 
#include <BlynkSimpleEsp8266.h> 

char auth[] = BLYNK_AUTH_TOKEN;
char ssid[] = "mikhasa";
char pass[] = "bismillah";
BlynkTimer timer;
    
 
 BLYNK_WRITE (V0){ 
  digitalWrite (D0,param.asInt()); }
  BLYNK_WRITE (V1){
  digitalWrite (D1,param.asInt()); 
  }   
void setup() 
{ 
  // Debug console 
  Serial.begin(9600); 
  
  pinMode(D0, OUTPUT); 
  pinMode(D1, OUTPUT);
  
  
  Blynk.begin(auth, ssid, pass, "blynk.cloud", 80); 
  
} 
void loop() 
{ 
  Blynk.run();
  timer.run(); 

  
}
