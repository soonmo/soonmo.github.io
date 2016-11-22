---
title: Microsoft Point and Print
layout: page
permalink: /tutorials/upd/microsoft-point-and-print/
---
Microsoft Point and Print 의 작동 원리를 실습을 통해서 실제 경험한다.

  * 이전 실습에서 설치했던 프린터 드라이버를 삭제한다.
  * 윈도우키 + R, **\\dc\mfp1** 입력 후 “**확인**” 클릭

	![](http://soonmo.github.io/images/2-11.png)

  * 잠시 기다리면 서버와 연결되면서 프린터가 자동으로 설치됨 – 이것이 **Microsoft Point and Print** 기술임
  * **시작** > **장치 및 프린터**, dc의 mfp1 마우스 포인터 위치시킨 후 마우스 오른쪽 버튼 클릭 후 “**인쇄 기본 설정**” 클릭

	![](http://soonmo.github.io/images/3-9.png)

  * “**완료**” 탭 클릭, “**양면 인쇄**” 가 기본으로 선택되어 있음

	![](http://soonmo.github.io/images/4-11.png)

  * “**양면 인쇄**” 체크 해제 후 “**적용**” 클릭

	![](http://soonmo.github.io/images/5-8.png)

  * 색상탭 클릭해 보면 “**그레이스케일로 인쇄**” 에 체크가 되어 있는데 이를 해제 후 “**확인**” 클릭

	![](http://soonmo.github.io/images/6-8.png)

  * 테스트용 칼라PDF 문서를 열어서 인쇄해 본다, ㈜ 문서가 바로 프린터로 전송되는 것이 아니라 프린트 서버를 거쳐서 프린터로 전송된다.

	![](http://soonmo.github.io/images/7-9.png)

  * 로그아웃 했다 도메인 계정으로 재로그인한다. (또는 재부팅)
  * **시작** > **장치 및 프린터**, dc의 mfp1 마우스 포인터 위치시킨 후 마우스 오른쪽 버튼 클릭 후 “**인쇄 기본 설정**” 클릭

	![](http://soonmo.github.io/images/10-8.png)

  * 완료와 색상탭에서 각각 “**양면 인쇄**”, “**그레이스케일로 인쇄**” 설정을 확인해라.