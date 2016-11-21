---
title: AutoSend
layout: page
permalink: /tutorials/fs-device-ug/autosend/
---
AutoSend는 주기적으로 일련 번호, 이벤트 로그, 사용 페이지 수, 소모품 상태 정보 등 프린터 구성 정보 등을 HP 로 전송하거나 이메일, 웹서버 등으로 전송하는 기능이다.

사전 준비 사항

메일전송(SMTP) 서버

  * 일반 &#8211;  AutoSend
  * 다음과 같이 설정 
      * “**AutoSend 활성화**” 체크
      * 일, 주, 월, 인쇄 페이지 중에서 “**인쇄** **페이지**” 선택하고, 50 입력
      * HP로 보내기 체크 해제
      * 전자우편으로 전송 체크 후 수신자에 [s**n**@ppsdemo.net](mailto:sn@ppsdemo.net) 입력 후 “**추가**” 클릭
      * (**노트**) 전송 주기 설정에 따라서 프린터 정보를 보낸다. 예를 들어서 “일” 을 선택하고 “1” 을 입력면 하루에 한번 씩 프린터 정보를 메일로 보낸다.

	![](http://soonmo.github.io/images/2-6.png)

  * 주소 지정에 [mfp**n**@ppsdemo.net](mailto:mfpn@ppsdemo.net) 을 입력 후 “**적용**” 클릭 (보내는 사람 주소로 표시)

	![](http://soonmo.github.io/images/2-6.png)

  * &#8220;**테스트**&#8221; 클릭

	![](http://soonmo.github.io/images/4-7.png)

  * <http://mail.ppsdemo.net> 접속 후 로그인
  * 메일 확인 – “**Device Snapshot …** “ 으로 시작하는 제목의 메일임 더블 클릭

	![](http://soonmo.github.io/images/6-5.png)

  * 첨부 파일 “Device.xml” 더블 클릭

	![](http://soonmo.github.io/images/7-6.png)

  * &#8220;그래도 항상 표시&#8221; 클릭

	![](http://soonmo.github.io/images/7-1-1.png)

  * 무슨 내용인지 알아 보기 힘들다. &#8220;다운로드&#8221; 클릭 후 바탕 화면에 저장

	![](http://soonmo.github.io/images/7-2-1.png)

  * XML 파일 내에 아래와 같은 많은 정보가 포함되어 있다.

	![](http://soonmo.github.io/images/8-6.png)