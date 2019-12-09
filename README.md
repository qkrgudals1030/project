> ## 팀원
20191122 김준영

20191125 박형민

20191126 손정우 

20191130 이진욱

20191135 천준영

> ## 작품제목 

지키미

> ## 목적 

1인가구가 늘어 남에 따라 1인가구를 노리는 범죄가 늘어나고 있기 때문에 이를 방지하고자 만들게 되었습니다.

> ## 작품설명

ir센서와 송수신기에서 감지한 내용을 앱인벤터를 통해 휴대폰으로 알림이 올 수 있도록 하는 지키미를 만들어 보았습니다. 

> ## 아두이노 코드

```c
void setup()
{   
  pinMode(3, INPUT); 
  pinMode(2, OUTPUT);
  Serial.begin(9600);
}
int irDetect(int irLedPin, int irReceiverPin, long frequency)
{
  tone(irLedPin, frequency, 8);
  delay(1);
  int ir = digitalRead(irReceiverPin);
  delay(1);
  return ir;
}
void loop()
{
  int wr = irDetect(2, 3, 42000);
  Serial.print("  ");
  Serial.println(wr);
  delay(100);
}
```
> ## 앱인벤터 블럭코딩 

![앱인벤터](https://user-images.githubusercontent.com/50895124/70435126-5a107c80-1ac9-11ea-89da-fe2f45d53932.PNG)

![팀과제 앱인벤터 블록코딩](https://user-images.githubusercontent.com/50895124/70435130-5c72d680-1ac9-11ea-8c82-1afb033dda57.PNG)




