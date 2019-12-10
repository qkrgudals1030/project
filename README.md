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

> ## 아두이노 작품

![KakaoTalk_20191209_212102532](https://user-images.githubusercontent.com/50895124/70435469-4285c380-1aca-11ea-83ea-2337010aed96.jpg)

![KakaoTalk_20191209_212144639](https://user-images.githubusercontent.com/50895124/70435478-47e30e00-1aca-11ea-9805-82e9aa9e2c87.jpg)

> ## 유튜브링크

https://github.com/qkrgudals1030/project

> ## 리플릿

![캡처](https://user-images.githubusercontent.com/51018392/70547148-bea80600-1bb3-11ea-9a03-b59715515681.PNG)

> ## 소감 

저희가 생각한 아이디어를 저희가 배웠던 내용들을 가지고 만들어 보면서 제가 생각한 아이디어에 대한 자신감을 가질 수 있었습니다. 또한 배웠던 내용을 작품을 만들어보면서 막히는 부분들은 인터넷과 카페를 통해 해결해보면서 조금더 기술을 익힐 수 있었습니다. 이런 작품을 만드는 과정이 쉽지만은 않았지만 만들고 나니 더욱더 다양한 작품들을 만들어 보고 싶다고 생각하게 되었습니다. 이런 기회를 주셔서 감사합니다 심재창 교수님. 창의공학 파이팅!!!


