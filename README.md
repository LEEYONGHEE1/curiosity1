# curiosity

큐리오 시티 : 화성 탐사 로버를 벤치마킹한 프로젝트

Arduino(NodeMCU) -> 온습도 센서 연결 및 받아온 데이터 json으로 변환
AWS Iot core 로 MQTT 통신을 이용해 데이터 보냄

![KakaoTalk_20220519_023524197](https://user-images.githubusercontent.com/80656902/170838403-c20eaa24-31d0-4bab-acba-9463b41f76f5.jpg)

아두이노 -> AWS IotCore
![아두이노에서 값 전송](https://user-images.githubusercontent.com/80656902/170838487-858acec6-dd68-4eb0-ac21-9856603b654c.png)

AWS IotCore 에서 토픽으로 구독
![AWS에서 값 받아오기](https://user-images.githubusercontent.com/80656902/170838529-2d675fd0-504e-4575-aa5b-b8776b4fa8b0.png)

AWS Lambda를 사용하여 DynamoDB에 저장

![lambda](https://user-images.githubusercontent.com/80656902/170838549-2b295f82-9af0-4f90-9548-a9e043b67340.png)
![dynamodb 연결 성공 화면](https://user-images.githubusercontent.com/80656902/170838570-9ffecd0f-5bfc-45c1-a380-ce0cb272252d.png)

DB 값은 Lambda와 REST API의 POST를 활용해 코틀린 환경에서 구현




