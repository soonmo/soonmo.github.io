---
title: '액세스 제어 &#8211; 로컬 장치'
layout: page
permalink: /tutorials/fs-device-ug/access-control-local-device/
---
복합기의 각 기능 (복사, 인쇄, 디지털 전송, 팩스 등)의 무단 사용을 보호하기 위해서 각 사용자 식별 코드 (숫자 5자리 이상)를 설정해서 허가된 사용자만 사용하게 할 수 있다. 중소 규모 사무실에 적합한 보안 솔루션이다.

## <span id="i">사용자 추가</span>

  * **정보** &#8211; **작업 일지** 클릭, 사용자 항목을 기록해 둔다. (예) PPSDEMO\s1

	![](http://soonmo.github.io/images/1-3.png)

  * **보안** &#8211; **액세스 제어**
  * 스크롤 다운, “**장치 사용자 계정**”, “**새로 만들기**”… 클릭

	![](http://soonmo.github.io/images/3-4.png)

  * 새 장치 사용자 계정에 본인 계정 정보를 다음과 같이 입력한다. 
      * 표시이름: Studentn (n은 학생 번호) (예) Student1
      * 전자우편 주소: <sn@ppsdemo.net> (예) s1@ppsdemo.ne
      * 네트워크 이름: PPSDEMO\sn (예) PPSDEMO\s1
      * 액세스코드: 11111 (학생번호가 2이면 22222, 학생번호가 3이면 33333….)
      * 권한 집합: **장치 운영자**

	![](http://soonmo.github.io/images/4-4.png)

  * 새 장치 사용자 계정에 파트너 계정 정보를 다음과 같이 입력한다. 
      * 표시이름: Studentn (n은 학생 번호) (예) Student2
      * 전자우편 주소: <sn@ppsdemo.net> (예) <s2@ppsdemo.net>
      * 네트워크 이름: PPSDEMO\sn (예) PPSDEMO\s2
      * 액세스코드: 22222
      * 권한 집합: **장치 사용자**

	![](http://soonmo.github.io/images/5-5.png)

  * **로그인 및 권한 정책** – “**응용 프로그램 복사**”를 아래와 같이 설정 후 화면 제일 아래 “**적용**” 클릭

	![](http://soonmo.github.io/images/6-3-(1).png)

## <span id="i-2">복합기 테스트</span>

  * 복합기 홈 화면에서 &#8220;**복사**&#8221; 선택

	![](http://soonmo.github.io/images/copy_menu.png)

  * 액세스 코드에 사용자 추가시 설정한 본인의 코드를 입력한다. (예) 1111

	![](http://soonmo.github.io/images/7-3-(1).png)

  * 복사 화면이 나오면 화면 상단에 사용자 이름으로 로그인인 되었는지 확인한다.

	![](http://soonmo.github.io/images/8-4-(1).png)

  * 같은 방법은 다른 사용자 액세스 코드로 로그인 한다.

	![](http://soonmo.github.io/images/9-1-(1).png)

## <span id="i-3">복합기 테스트</span>

  * 내장 웹서버 우측 상단 &#8220;**로그아웃**&#8221; 클릭해서 로그 아웃한다

	![](http://soonmo.github.io/images/10-2.png)

  * &#8220;**로그인**&#8221; 선택

	![](http://soonmo.github.io/images/11-3-(1).png)

  * 로컬 장치 계정을 “**로컬 장치 사용자**” 로 변경 후 암호에 admin 이 아니라 본인이 설정장 액세스 코드 (예, 11111) 를 입력한다

	![](http://soonmo.github.io/images/12-3-(1).png)

  * 우측 상단에 사용자 이름을 보면 실제 사용자명이 나타난다. (예) Student

	![](http://soonmo.github.io/images/13-2-(1).png)

  * 로그 아웃 후 같은 방법으로 파트너 코드 (권한 집합이 장치 사용자)로 로그인한다. 무엇이 다른가?

## <span id="i-4">여러 사용자 한꺼번에 추가 (가져오기)</span>

  * **보안** &#8211; **액세스 제어**
  * 스크롤 다운 &#8220;**장치 사용자 계정**&#8220;, **내보내기** 클릭

	![](http://soonmo.github.io/images/16-(1).png)

  * 내보내기 클릭 후 바탕화면에 CSV 파일을 저장한다.

	![](http://soonmo.github.io/images/18-1-(1).png)

  * 파일을 열어 보면 아래와 같다. (엑셀이 없으면 노트패드로 내용을 확인)

	![](http://soonmo.github.io/images/19-1-(1).png)

  * 엑셀로 파일에 사용자 정보를 추가 후 바탕화면에 저장함 (예, “User_list.csv”)

	![](http://soonmo.github.io/images/20-2.png)

  * “**장치 사용자 계정**”, 가져오기 클릭

	![](http://soonmo.github.io/images/21-2.png)

  * “**찾아보기**” 클릭 후 바탕화면의 “User_list.csv” 선택, **가져오기** 클릭

	![](http://soonmo.github.io/images/22-(1).png)

  * 아래와 같이 사용자들이 추가됨

	![](http://soonmo.github.io/images/23-(1).png)

  * 복합기에서 “**복사**” 를 누르고 등록된 액세스 코드로 로그인이 되는지 확인한다.

	![](http://soonmo.github.io/images/copy_menu.png)