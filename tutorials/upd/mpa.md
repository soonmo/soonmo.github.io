---
title: MPA 솔루션 맛보기
layout: page
permalink: /tutorials/upd/mpa/
---
HP MPA (Managed Print Administration) 는 PARK (Printer Administration Resource Kit)에 포함된 솔루션의 하나로 사용자 별 출력 정책, 프린터 리스트 등을 제공한다. 이번 실습에서는 UPD와 MPA를 연동해서 프린터 리스트를 사용자에게 효과적으로 제공하는 MPL(Managed Print List) 이라고 부르는 기능을 체험해 본다.

  * &#8220;**명령 프롬프트**&#8221; 실행, (윈도우키 + R, cmd 입력 후 엔터)
  * UPD 설치 프로그램 폴더로 이동 (C:\HP Universal Print Driver\pcl6-x64-6.0.0.18849)

	![](http://soonmo.github.io/images/3-10.png)

  * 다음 명령어를 입력 후 “**엔터**” 
      * Install /empa /policy”172.16.10.40” /dm /h /n”LAB4”

	![](http://soonmo.github.io/images/4-12.png)

  * 명령어의 의미를 알고 싶으면 install /? 하면 옵션에 대한 설명이 나온다. 설치가 끝나 때까지 기다린다. /h 옵션을 주었기 때문에 설치 진행 상황이 나타나지 않고 백그라운드로 실행된다. 작업 표시줄에 UPD 설치 프로그램 아이콘이 있으면 아직 설치 중임을 알 수 있다.

	![](http://soonmo.github.io/images/6-9.png)

  * 설치가 완료되면 LAB4  “**프린터 속성**” 클릭

	![](http://soonmo.github.io/images/7-10.png)

  * **프린터 찾기** > **classroom**… 클릭

	![](http://soonmo.github.io/images/8-9.png)

  * HP MPL Printer Groups 창이 나타나면 출력을 원하는 프린터 선택 (Managed Printer List)

	![](http://soonmo.github.io/images/9-9.png)

  * “**확인**” 클릭

	![](http://soonmo.github.io/images/10-9.png)

  * “**테스트 페이지 인쇄**” 클릭, “**닫기**”, “**확인**” 클릭

	![](http://soonmo.github.io/images/11-7.png)

  * PDF 문서를 열어서 인쇄를 한다. (MPL 사용)