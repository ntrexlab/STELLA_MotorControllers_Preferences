# STELLA_MotorControllers_Preferences
STELLA 구동 시 Motor 작동및 센서값이 비정상적인 경우 윈도우 환경에서 UI를 통해 설정 값을 확인하셔야 됩니다.



***
## 1. 사용 하드웨어 및 Tool
 * #### 사용 하드웨어 
    - StellaN1_Motor - [소형 유성 DC 엔코더 모터 12V 1:27 500PPR](https://smartstore.naver.com/phonepong/products/5897519502)
    - StellaN2_Motor - [소형 기어드 DC 엔코더 모터 12V 1:30 500PPR](https://smartstore.naver.com/phonepong/products/5747732463)
     - STELLAN1_MDC24D100D-v2 - [MW_MDC24D100D-v2](http://www.devicemart.co.kr/goods/view?no=1077424)
     - STELLAN2_MDC24D50D-v1 - [따로 판매하지 않는 상품]
     - STELLAN1_배터리 -[KC인증 충전식 고용량 농업용 분무기 리튬이온배터리](https://www.weled.co.kr/goods/goods_view.php?goodsNo=1000034222)
    - STELLAN2_배터리 - [따로 판매하지 않는 상품]
* #### 사용 Tool
    - Mobile_Ui [설치경로-관련자료](https://www.devicemart.co.kr/goods/view?no=1077424#goods_file)
***
## **모터와 모터드라이버 배선도**
#### 1. 100D_배선도
![100D_회로](https://user-images.githubusercontent.com/85467544/155084736-b8d0f172-a15e-4104-bf24-bd55e7e87d66.png)

#### 2. 50D_배선도
![50D_회로](https://user-images.githubusercontent.com/85467544/155084730-378111ea-2681-4fc5-9665-cb57aaf575a6.png)

***
## **환경 설정 확인 방법**
***
#### 1.  모터드라이버를 USB를 통해 PC에 연결합니다.  
#### 2. Mobile_UI를 실행 후 Scan Devices 버튼을 클릭합니다.
![md_1](https://user-images.githubusercontent.com/85467544/155093378-fb8caea4-ba94-4661-afa1-39a70140872f.png)
#### 3. Configuration(1) 버튼을 클릭 후 Expand All(2) 버튼을 클릭합니다.
![md_2](https://user-images.githubusercontent.com/85467544/155093364-d2de820f-bbf8-4531-9d04-d0e76a1396b6.png)
#### 4. Motor 1,2 Encoder 값을 확인한다. Stella N1 540000, Stella N2 60000 이면 정상 파라미터. 
![md_3](https://user-images.githubusercontent.com/85467544/155093371-2eeec8e1-e051-4307-966e-970e8029709e.png)
#### 5. 이 후 모터 컨트톨러 페이지에서 Velocity 양수 입력시  모터에 + 선이 왼쪽에 있다고 가정 시 Channel 1은 시계 방향, Channel 2은 반시계 방향으로 작동 시 정상 5,6번 정상일 경우 . 
![md_4](https://user-images.githubusercontent.com/85467544/155253666-b0f1ea8a-c427-4024-9c2c-5add3deeff0b.png)
![md9](https://user-images.githubusercontent.com/85467544/155253599-441deac9-4751-4d28-8d5c-b2874d195846.PNG)


***
## **환경 설정 하기**
#### 1.  Stella 프로파일 셋업 파일 다운로드 합니다.[설치경로-관련자료](https://github.com/ntrexlab/MOTOR_GAIN)
#### 2. Mobile_UI를 실행 후 Scan Devices 버튼을 클릭합니다.
![md_1](https://user-images.githubusercontent.com/85467544/155093378-fb8caea4-ba94-4661-afa1-39a70140872f.png)
#### 3. Configuration(1) 버튼을 클릭 후 Load From File(2) 버튼을 클릭합니다.
![md_6](https://user-images.githubusercontent.com/85467544/155097164-e31b9f28-afeb-467c-83d6-8bb5773985a1.png)
#### 4. 1번에서 다운로드 한 파일 선택합니다.
![md7](https://user-images.githubusercontent.com/85467544/155098265-26666617-030c-4b3a-bac2-8d101be4a481.png)
#### 4. Motor 1,2 Encoder(1) 값을 확인한다. Stella N1 540000, Stella N2 60000 이면 정상 파라미터 Write Configurations(2) 클릭 후 Save to Flash(3) 클릭합니다.
![md8](https://user-images.githubusercontent.com/85467544/155098273-3a764730-6c93-4ea1-b872-e092a39e71c9.png)

***
