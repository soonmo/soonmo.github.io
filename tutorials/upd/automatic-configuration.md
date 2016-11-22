---
title: Automatic Configuration 의 이해
layout: page
permalink: /tutorials/upd/automatic-configuration
---
모델 드라이버, UPD 에서는 프린터 드라이버 설치시 Auto Cofiguration 이라는 기술을 통해서 장치 구성을 자동으로 한다. 특히 UPD의 경우 장치가 칼라인지 흑백인지를 드라이버 설치시 구분하는데 Auto Configuration을 사용한다. 이번 실습을 통해서 UPD에서 Auto Configuration이 어떻게 작동하는지 정확히 이해할 수 있다.

  * 바탕화면의 UPD 설치 프로그램 더블 클릭

	![](http://soonmo.github.io/images/2-12.png)

  * Unzip 클릭

	![](http://soonmo.github.io/images/3-11.png)

  * “**확인**” 클릭

	![](http://soonmo.github.io/images/4-13.png)

  * 사용자 계정 콘트롤 창이 나오면 “**예**” 클릭
  * “**예**” 클릭

	![](http://soonmo.github.io/images/6-10.png)

  * “**일반 모드**” 선택 후 “**다음**” 클릭

	![](http://soonmo.github.io/images/7-11.png)

  * “**로컬 프린터 추가**” 클릭

	![](http://soonmo.github.io/images/8-10.png)

  * “**기존 포트 사용**” 선택, 이전 LAB에서 본인의 MFP IP 주소로 생성한 포트 선택 (없으면 새포트 만들기를 선택해서 포트를 생성한다), ㈜ 실습용 복합기가 흑백 복합기이면 다른 조의 칼라 복합기의 IP주소를 확인해서 포트를 생성한다.

	![](http://soonmo.github.io/images/9-10.png)

  * 복합기에서 LAN 케이블을 뽑니다. (연결해제)
  * HP Universal Printing PCL 6 (v6.0.0) 선택 후 “**다음**” 클릭

	![](http://soonmo.github.io/images/11-8.png)

  * 프린터 이름 그대로 두고 “**다음**” 클릭

	![](http://soonmo.github.io/images/12-8.png)

  * 좀 올래 걸리지만 기다린다. “**공유 안 함**” 선택 후 “**다음**” 클릭

	![](http://soonmo.github.io/images/13-6.png)

  * 복합기에 랜케이블 다시 연결
  * “**테스트 페이지 인쇄**” 클릭

	![](http://soonmo.github.io/images/15-5.png)

  * 테스트 페이지 확인 
      * **(질문)** 좌측상단의 Windows logo 가 칼라인가? 아니면 흑백인가?
      * **(질문)** 흑백으로 출력되었다면 이유는?
  * “**마침**” 클릭

	![](http://soonmo.github.io/images/16-7.png)

</p>

## 문제 해결 방법

  * “**프린터 속성**” 클릭

	![](http://soonmo.github.io/images/18-7.png)

  * “**장치 설정 탭**” 클릭, 스크롤 다운 후 “**장치 유형**” 을 “**컬러**” 로 변경 후 “**확인**” 클릭

	![](http://soonmo.github.io/images/19-7.png)

  * 테스트 페이지 인쇄