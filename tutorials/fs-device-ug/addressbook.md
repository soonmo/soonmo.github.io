---
title: 주소록 (Addressbook)
layout: page
permalink: /tutorials/fs-device-ug/addressbook/
---
주소록은 사용자 이름, 전화번호, 팩스번호, 이메일 주소, 공유폴더 등의 정보를 가지고 있다. HP 복합기에서는 복합기 자체에 저장되는 로컬 주소록과 네트웍 주소록(LDAP)을 지원하는데 주소록 기능을 잘 활용하면 scan to email 과 scan to network folder 기능을 좀 더 편리하게 사용할 수 있도록 도움을 줍니다.

## <span id="i">로컬 주소록</span>

  * 스캔/디지털 전송 &#8211; 주소록

	![](http://soonmo.github.io/images/1-3-(1).png)

  * 장치에 저장된 연락처에서 본인 연락처 (Studentn) 을 체크 후 “**편집**” 클릭

	![](http://soonmo.github.io/images/2-2.png)

  * 하기 정보 입력 후 “**확인**” 
      * 이름, 성, 전화 번호, 팩스 번호 등을 입력
      * “**네트웍 폴더**” 체크
      * UNC 폴더 경로: “**\\dc\scan\본인계정**” (예) **\\dc\scan\s1**
      * 소속조직, 부서, 구/군/시, 국가/지역 입력

	![](http://soonmo.github.io/images/3-1.png)

  * 위에서 입력한 정보가 업데이트 되었는지 확인

	![](http://soonmo.github.io/images/4-3.png)

## <span id="i-2">복합기 테스트</span>

  * ADF에 문서를 적재 후 홈화면의 “**네트워크 폴더에 저장**” 선택

	![](http://soonmo.github.io/images/5-3.png)

  * 인증

	![](http://soonmo.github.io/images/6-2.png)

  * 우측 중간에 책모양의 주소록 아이콘 선택

	![](http://soonmo.github.io/images/7-3.png)

  * 이름 선택 (Studentn) 후 화살표 선택, 확인

	![](http://soonmo.github.io/images/9-4.png)

  * &#8220;**네트워크 폴더에 저장**&#8220;

	![](http://soonmo.github.io/images/scan-to-network-folder-app.png)

  * &#8220;**확인**&#8220;

	![](http://soonmo.github.io/images/10-3.png)

  * “**윈도우키 + R**” 후 **\\dc\scan\sn** (예) **\\dc\scan\s1** 후 문서 확인

	![](http://soonmo.github.io/images/11-3.png)

## <span id="i-3">로컬 주소록 가져오기</span>

CSV 파일로 한번에 여러명의 주소를 복합기에 저장

  * 스캔/디지털 전송 – 주소록, 장치에 저장된 연럭처 아래 “**추가**” 클릭

	![](http://soonmo.github.io/images/12-3.png)

  * 이름: TechU 입력 후 “**확인**”

	![](http://soonmo.github.io/images/13-2.png)

  * “Lab7\_User\_list.csv” 파일을 바탕화면에 복사, “윈도우키+R” \\dc\lab_sw
  * &#8220;**가져오기&#8221;** 클릭

	![](http://soonmo.github.io/images/14-2.png)

  * “**찾아보기**” 클릭 후 바탕화면의 “**csv**” 선택 후 “**가져오기**” 클릭

	![](http://soonmo.github.io/images/15-3.png)

  * 추가된 사용자 확인

	![](http://soonmo.github.io/images/18-3.png)

## <span id="i-4">복합기 테스트</span>

  * 홈화면에서 “**네트워크 폴더에 저장**” 선택

	![](http://soonmo.github.io/images/19-3.png)

  * 인증

	![](http://soonmo.github.io/images/6-2.png)

  * 우측 중간에 책모양의 주소록 아이콘 선택

	![](http://soonmo.github.io/images/addressbook.png)

  * 모든 연락처를 누르면 메뉴가 나오는데 “TechU” 를 선택

	![](http://soonmo.github.io/images/22-4.png)

  * 이름들을 확인 후 좌측 상단의 홈 아이콘을 눌러서 복합기 홈화면으로 이동

	![](http://soonmo.github.io/images/23-3.png)

  * 문서 적재 후 홈화면의 “**전자우편**” 선택

	![](http://soonmo.github.io/images/35.png)

  * 받는 사람 우측의 주소록 아이콘 선택

	![](http://soonmo.github.io/images/addressbook2.png)

  * 연락처를 “TechU” 로 변경후 User1 을 받는 사람에 추가 후 확인

	![](http://soonmo.github.io/images/28-1.png)

  * &#8220;**전자우편 전송**” 선택

	![](http://soonmo.github.io/images/email_app.png)

## <span id="i-5">네트워크 주소록 설정</span>

  * 스캔/디지털 전송 – 주소록, **네트웍크 연락처 활성화(LDAP 서버 사용)** 아래 “**추가**” 아이콘 클릭

	![](http://soonmo.github.io/images/31.png)

  * LDAP 서버 주소: 172.16.10.10, 서버에 인증 필요 선택 
      * Windows 협상 (SPENGO)
      * Window 도메인: ppsdemo
      * 사용자 이름: sn (본인 계정)
      * 암호: Sn (본인 암호)
      * 검색 시작 경로: DC=ppsdemo, DC=net

		![](http://soonmo.github.io/images/32.png)

  * 테스트에 user6 를 입력 후 “**테스트**” 클릭

	![](http://soonmo.github.io/images/33.png)

	![](http://soonmo.github.io/images/33-1.png)

  * “**네트워크 연락처 활성화 (LDAP 서버 사용)**” 체크 후 화면 하단 “**적용**” 클릭

	![](http://soonmo.github.io/images/34.png)

## <span id="i-6">복합기 테스트</span>

  * 홈화면 &#8220;**전자우편**&#8221; 선택

	![](http://soonmo.github.io/images/35.png)

  * 인증

	![](http://soonmo.github.io/images/6-2.png)

  * 우측 중간에 책모양의 주소록 아이콘 선택

	![](http://soonmo.github.io/images/addressbook2.png)

  * 모든 연락처 선택, ㈜ 어떤 차이가 있는가?

	![](http://soonmo.github.io/images/38.png)