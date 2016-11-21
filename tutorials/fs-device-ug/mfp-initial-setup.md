---
layout: page
title: 복합기 기본 설정
permalink: /tutorials/fs-device-ug/mfp-initial-setup/
---
이번 섹션에서는 복합기 설치 단계에서 가장 기본이 되는 설정을 수행한다.

## 복합기 최초 부팅 후 작업

  * 언어 설정 &#8211; 언어:**한글**, 기보드 레이아웃: **한글**

	![](http://soonmo.github.io/images/1-2.png)

  * 날짜/시간 형식 &#8211; 날짜 형식: YYYY/MMM/DD, 시간 형식: 12시간(오전/오후)

	![](http://soonmo.github.io/images/2-2.png)

  * 시간대- **(GMT+9:00) 서울**, 날짜/시간을 맞춘다.

	![](http://soonmo.github.io/images/3-2.png)

  * 확인을 선택하면 홈스크린이 나온다.

	![](http://soonmo.github.io/images/4-2.png)

  * &#8220;**초기 설정**&#8221; 메뉴 선택

	![](http://soonmo.github.io/images/5-2.png)

  * 좌측 상단 홈(집모양) 아이콘 선택

	![](http://soonmo.github.io/images/6-1.png)

  * 시작화면에 &#8220;**초기 설정**&#8221; 표시 체크 해제 후 확인

	![](http://soonmo.github.io/images/7-2.png)

## 복합기 네트웍 설정

  * IE 실행 후 주소에 프린터 IP 를 입력한다. ㈜ 프린터 IP 는 홈스크린 우측 상단의 네트웍 아이콘을 선택해서 확인한다.

	![](http://soonmo.github.io/images/network_icon.png)

  * **네트워킹** 탭
  * **TCP/IP 설정** &#8211; **네트워크 ID** 탭 선택
  * 호스트 이름에 영문으로 이름 입력, 확인

	![](http://soonmo.github.io/images/11-2.png)

  * TCP/IP(v4) 탭 선택 후 아래와 같이 설정 후 적용, 확인 
      * IP 구성 방법: 수동
      * IP 주소: 172.16.10.15x
      * 서브넷마스크, 기본게이트웨이 설정

		![](http://soonmo.github.io/images/12-2.png)

## UPD (Universal Print Driver) 설치

  * 이곳에서 UPD PCL 6 드라이버를 다운받는다. (32bit, 64bit 맞는 것 선택)
  * &#8220;upd-pcl6-x64-6.0.0.1.18849&#8221; 더블 클릭 (32bit OS면 upd-pcl6-x32-6.0.0.1.18849)
  * 설치 모드 선택 화면이 나오면 &#8220;**동적모드**&#8221; 선택

	![](http://soonmo.github.io/images/20-1.png)

  * 설치가 끝나면 &#8220;**마침**&#8221; 클릭

	![](http://soonmo.github.io/images/21-1.png)

  * [시작]-[장치 및 프린터], HP Universal Printing PCL 6 마우스 오른쪽 클릭 후 프린터 속성 선택
  * 프린터 주소 입력: 172.16.10.15x
  * &#8220;**내 프린터 및 팩스 폴더에 이 프린터 추가**&#8221; 선택 후 확인

	![](http://soonmo.github.io/images/26.png)

  * 새로 추가된 프린터 &#8220;HP LaserJet color flow MFP M575 (xxx.xxx.xxx.xxx)&#8221; 기본 프린터로 설정 후 시험 인쇄를 한다.