---
layout: post
title: ScanJet Pro 4500fn1 리뷰
tags: ScanJet 스캔젯 리뷰
---



제품의 주요 사양은 다음과 같습니다.



![hp-scanjet-pro-4500-fn1-network-scanner](..\images\hp-scanjet-pro-4500-fn1-network-scanner.jpg)



* 모델명 (제품번호): HP ScanJet Pro 4500fn1 (L2749A)
* 스캐너 타입: ADF & 플랫베드
* 스캔 속도: 30ppm (단면 칼라/흑백, 300dpi), 60ipm (양면 칼라/흑백, 300dpi)
* 싱글 패스 양면 스캔 지원
* ADF 용량: 50 매
* 광학 해상도: 600dpi (ADF), 1200dpi (플랫베드)
* 권장 사용량: 4,000매/일
* 롤러 기대 수명: 100,000 매 (L2742A)
* 광원: LED
* 센서 기술: CMOS CIS
* 권장 용지 무게: 45 - 120 (gsm)
* 연결: USB 3.0, Ethernet, Wi-Fi
* 드라이버: TWAIN, ISIS, WIA



이제품의 가장 큰 특징은 다양한 연결을 지원하는 것입니다. 일반적으로 스캐너는 USB로 연결해서 1대의 PC에서 사용하지만 이제품은 유선랜이나 무선랜에 연결해서 여러대의 PC에서 스캔을 할 수 있습니다. 또한 스캐너 자체에 작지만 터치 스크린이 있어서 스캐너를 직접 조작도 할 수 있습니다. 

![hp-scanjet-pro-4500-fn1-network-scanner-back](..\images\hp-scanjet-pro-4500-fn1-network-scanner-back.jpg)



USB 연결 방식은 다른 스캐너 제품과 동일하기 때문에 특별히 설명할 것이 없습니다. 네트웍에 스캐너를 연결해서 여러 사람들이 공유해서 사용하는 방식에 대해서 알아 보겠습니다.



# 네트웍 설정

인터넷 공유기를 사용하거나 **유동 IP (DHCP)** 환경에서는 스캐너를 연결하면 바로 IP 주소가 자동으로 설정됩니다. 따로 작업할 것이 없습니다.

만약에 **고정 IP** 환경이라고 하면 스캐너에서 직접 IP 설정이 불가능하기 때문에 PC 또는 노트북과 랜케이블로 직접 연결해서 아래와 같은 과정으로 IP 설정을 해야 합니다.

![SJ4500-Static-IP](..\images\SJ4500-Static-IP.PNG)



# 소프트웨어 설치

hp.com 에서 스캔 소프트웨어 (HP Scan) 를 다운로드 후 설치합니다.

http://h30438.www3.hp.com/pub/softlib/software13/printers/Full_Webpack-41.4.2220-SJ4500f1_Full_Webpack.exe



# 스캔 시나리오 A

HP Scan 소프트웨어를 사용해서 스캔하는 방식으로 아래 2가지 방식 (방법1, 방법2)이 있습니다.

![SJ4500-Usage-01](..\images\SJ4500-Usage-01.PNG)



## 방법 1

예약 스캔이라는 방식으로 먼저 HP Scan 을 실행 후 해상도, 스캔 파일 포맷 (PDF, JPG...) 을 설정 후에 스캔을 진행합니다. 그러면 스캔이 진행되는 것이 아니라 아래와 같은 안내 메시지가 나타납니다.

![sj4500 002](..\images\sj4500 002.png)



스캔할 문서를 가지고 스캐너로 이동합니다.

![SJ4500-HPSCAN 001](..\images\SJ4500-HPSCAN 001.png)

* 문서를 적재 후에 스캐너의 터치 스크린의 **"예약된 작업"** 선택합니다.
* 컴퓨터 선택에서 본인의 컴퓨터 이름을 선택합니다. 
* **"스캔"** 선택하면 문서가 스캔되고 PC로 스캔 이미지가 전송됩니다.



## 방법 2

HP Scan 소프트웨어를 구동하지 않고 바로 스캐너에서 스캔하는 방식입니다. HP Scan 소프트웨어를 설치하면 스캐너와 통신하는 서비스가 실행됩니다. 스캐너에 HP Scan 이 설치된 PC 가 등록되는데 최대 10대의 PC가 등록 가능합니다.

![SJ4500-HPSCAN 002](..\images\SJ4500-HPSCAN 002.png)

 

세번째 화면의 단축키는 HP Scan 에서 설정한 단축키입니다. 



# 스캔 시나리오 B

**시나리오 B** 는 HP 복합기의 디지털 전송 기능과 유사한 기능으로 스캐너에서 스캔 후 바로 메일 전송 서버(SMTP)를 통해서 스캔파일을 첨부해서 **이메일로 전송**하거나 PC의 **공유 폴더로 전송**하는 기능입니다.

![SJ4500-Usage-02](..\images\SJ4500-Usage-02.PNG)



이 방식을 사용하려면 HP Scan 이 필요없고 스캐너의 내장 웹서버 (EWS)에 웹브라우저로 접속 후 필요한 설정을 해야합니다. 



## Scan to Folder

PC 의 공유 폴더를 설정 후 스캐너에 웹브라우저로 접속 후 상단 **"스캔"** 메뉴에 들어갑니다. 좌측의 **"네트워크 폴더 설정"** 클릭 후  하단의 **"새로 추가"**를 클릭합니다.

![SJ4500-SCAN2Folder 001](..\images\SJ4500-SCAN2Folder 001.png)



공유 폴더 설정값을 입력해 줍니다. **"저장 & 테스트"** 클릭해서 정상적으로 설정되었는지 확인합니다.

![SJ4500-SCAN2Folder 002](..\images\SJ4500-SCAN2Folder 002.png)



**"스캔 설정"** 에서 스캔 후 네트웍 폴더로 전송에 대한 기본 설정을 한 후에 상단에 **"스캔 후 네트워크 폴더로 전송 활성화"** 를 체크 후 **"적용"** 을 클릭합니다.

![SJ4500-SCAN2Folder 003](..\images\SJ4500-SCAN2Folder 003.png)



스캐너로 이동 후 문서를 적재합니다. **"네트워크 폴더로 전송"**  선택하면 표시 이름에 이전에 설정했던 이름 (영수증...)이 나타납니다. 폴더를 선택후 스캔 옵션을 변경하거나 **"스캔"** 을 선택하면 스캔이 진행됩니다.

 ![SJ4500-SCAN2Folder-Usage](..\images\SJ4500-SCAN2Folder-Usage.png) 





## Scan to Email

우선 이메일 전송을 위해서 메일전송서버 (SMTP) 가 필요합니다. SMTP 서버가 없다면 본 기능을 사용할 수 없습니다.  대부부분의 SMTP 서버는 보안 조치가 되어 있어서 전산실에  우선 확인해서 스캐너에서 보내는 이메일을 전달할 수 있는지 확인하고 보안 정책에 의해서 사용할 수 없다면 본 기능을 사용할 수 없습니다.



스캐너에 웹브라우저로 접속 후 상단 **"스캔"** 메뉴에 들어갑니다. 좌측의 **"스캔 후 이메일 설정"** 클릭 후  필요한 설정값을 입력해 줍니다.

![SJ4500-Scan2Email-Config 001](..\images\SJ4500-Scan2Email-Config 001.png)

 

**"스캔 설정"** 에서 스캔 후 이메일 설정에 대한 기본 설정을 한 후에 상단에 **"스캔 후 이메일로 전송 설정 활성화"** 를 체크 후 **"적용"** 을 클릭합니다.

![SJ4500-Scan2Email-Config 002](..\images\SJ4500-Scan2Email-Config 002.png)

 

스캐너로 이동 후 문서를 적재합니다. **"이메일로 전송"**  선택하면 **이메일 주소 선택**이 나타납니다. 이메일 주소를 선택하거나 이메일 주소 입력을 선택 후 직접 입력합니다.  스캔 옵션을 변경하거나 **"스캔"** 을 선택하면 스캔이 진행됩니다.![SJ4500-SCAN2Email-Usage](..\images\SJ4500-SCAN2Email-Usage.png)
