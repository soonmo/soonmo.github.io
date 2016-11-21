---
title: Port 변경
layout: page
permalink: /tutorials/wja-ug/port/
---
웹젯어드민은 기본적으로 http 통신은 8000 번 포트를 사용하고, https 는 8443 포트를 사용하도록 구성되어 있다. 이유는 일반 웹 서버와 포트 충돌을 막기 위해서이다. 만약 8000, 8443 포트를 다른 프로그램에서 사용하고 있다면 웹젯어드민 서비스의 포트 변경을 해야 한다.

  * C:\Windows\ServiceProfiles\NetworkService\AppData\Local\Hewlett-Packard\HPWebJetAdmin\WjaService\config 폴더로 이동 후 “HP.Imaging.Wja.Core.WebServer.config.xml” 파일을 노트 패드로 연다.

	![](http://soonmo.github.io/images/wja-ug-226.jpg)

  * 8443을 9443 으로 변경, 8000 을 9000 으로 변경 (원하는 임의의 포트 번호로 변경) 후 저장

	![](http://soonmo.github.io/images/wja-ug-227.jpg)

  * 윈도우키 + R, services.msc 입력 후 엔터
  * HPWJA 서비스 선택, &#8220;다시 시작&#8221;을 클릭해서 서비스를 재시작 한다.

	![](http://soonmo.github.io/images/wja-ug-228.jpg)

  * IE 실행 후 주소에 [http://localhost:9000](http://localhost:9000/) 엔터