---
title: ACL (Access Control List)
layout: page
permalink: /tutorials/fs-device-ug/access-control-list/
---
ACL을 구성하면 특정 PC 나 Server 에서만 복합기로 인쇄를 하거나 접속을 할 수 있다. 즉 네트웍 단에서 접근 제어를 할 수 있다. 예를 들어서 프린트 서버를 통해서 출력이 되도록하고 개별 PC에서의 출력을 막고 싶다면 ACL을 설정하면 된다.

## ACL 설정

  * **네트워킹** 탭 클릭
  * 사용자: admin, 암호:admin 입력 후 확인

	![](http://soonmo.github.io/images/2-4.png)

  * 좌측 메뉴 중 &#8220;**승인**&#8221; 클릭 후 메인 화면의 &#8220;**액세스 제어**&#8221; 탭 클릭
  * 우측 테이블에 아래와 같이 IPv4 주소에 본인 PC의 IP 주소를 입력하고 저장에 체크, 화면 하단의 “**적용**” 클릭

	![](http://soonmo.github.io/images/5-4.png)

## 테스트

  * ACL에 입력된 PC 에서 시험 인쇄 수행, 인쇄가 되는가?
  * 파트너 PC에서 시험 인쇄 수행, 인쇄가 되는가? IE를 실행 후 주소에 복합기 IP를 입력한다. 내장 웹서버가 나오는가?
  * 다시 액세스 제어 설정 화면에 와서 “**웹 서버(HTTP) 액세스 허용**” 체크 박스에 체크를 해제 후 “**적용**” 클릭

	![](http://soonmo.github.io/images/8-3.png)

  * 파트너 PC에서 복합기의 내장 웹서버에 접속해 본다. 내장 웹서버가 나오는가?
  * 다시 액세스 제어 설정 화면에 와서 원상 복구 한다. 
      * IP 주소 좌측의 저장 체크 마크 해제
      * &#8220;**웹 서버 (HTTP) 액세스 허용**&#8221; 체크

		![](http://soonmo.github.io/images/10-1.png)