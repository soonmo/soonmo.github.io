---
title: '액세스 제어 &#8211; LDAP'
layout: page
permalink: /tutorials/fs-device-ug/access-control-ldap/
---
엔터프라이즈는 보통 사용자가 수백, 수천, 수만명이라 로컬 계정을 복합기에 등록해서 사용하는데는 여러가지 문제가 있다. 보통 엔터프라이즈에서는 네트웍 기반의 사용자 인증을 사용하는데 LDAP (Lightweight Directory Access Protocol) 이라는 방식을 많이 사용한다. HP 복합기에는 LDAP 서버와 연동해서 사용자 인증을 할 수 있는 기능을 지원하고 있는데 일일히 사용자를 등록하지 않아도 LDAP을 통해서 모든 직원들을 인증할 수 있다.

## Softera LDAP Broswer 설치

  * 윈도우 + R, \\dc\lab_sw 입력한다.
  * LDAP_Broswer 폴더에 들어가서 “**ldapbroswer-4.5.13124.0-x64-eng**” 더블클릭
  * Select Installation Type 에서 “**Typical**” 선택해서 설치
  * 설치가 끝나면 바탕화면의 “**Softera LDAP Broswer**” 아이콘 더블클릭

	![](http://soonmo.github.io/images/4-5.png)

  * “**In the future, do not show the warning**” 체크 후 **OK**

	![](http://soonmo.github.io/images/5-6.png)

  * **No** 선택

	![](http://soonmo.github.io/images/6-4.png)

  * 프로그램이 실행되면 **Ctrl + P** 를 누른다. 프로파일 이름을 적당히 입력한다. (예) HP Partner Tech U Lab

	![](http://soonmo.github.io/images/7-4.png)

  * Host: 에 dc 입력, Fetch Base DNs 클릭 후 “DC=ppsdemo, DC=net” 선택

	![](http://soonmo.github.io/images/8-5.png)

  * “**Currently logged on user (Active Directory only**)” 선택

	![](http://soonmo.github.io/images/9-2.png)

  * 마침
  * Find what 에 **계정명**을 입력 후 엔터. (예) s1, 검색 결과가 나오면 CN 을 더블 클릭

	![](http://soonmo.github.io/images/11-4.png)

  * cn, distinguishedName 의 값을 메모한다. 
      * **cn**: s1
      * **distinguishedName**: CN=s1,CN=Users,DC=ppsdemo,DC=net

	![](http://soonmo.github.io/images/12-4.png)

## 내장 웹서버 설정

  * **보안** &#8211; **액세스제어** (좌측메뉴), **로그인 방법 활성화 및 구성의** LDAP 좌측의 “**설정**” 클릭

	![](http://soonmo.github.io/images/13-3.png)

  * LDAP 로그인  사용 체크, LDAP 서버 주소: 172.16.10.10, 접두사 바인딩: cn

	![](http://soonmo.github.io/images/14-2.png)

  * 루트 바인딩 및 검색: CN=Users,DC=ppsdemo,DC=net 입력 후 “**추가**” 클릭 
      * 입력한 이름과 이 속성 일치: **cn**
      * 이 속성으로 장치 사용자 전자우편 주소 불러오기: **mail**
      * 이 속성으로 장치 사용자의 이름 불러오기: **displayName**
      * 이 속성으로 장치 사용자의 관련 단체 불러 오기: **objectClass**

	![](http://soonmo.github.io/images/15-1.png)

  * **확인** 클릭
  * 다시 LDAP 좌측 &#8220;**설정**&#8221; 클릭

	![](http://soonmo.github.io/images/16-1.png)

  * 화면 하단 “**LDAP 로그인 테스트**” 에서 사용자 이름, 암호를 입력 후 “**테스트**” 클릭 
      * 사용자 이름: sn (본인 아이디)
      * 암호: Sn (본인 아이디)

	![](http://soonmo.github.io/images/17-2.png)

  * 정상적으로 LDAP 설정이 되었으면 아래와 같은 메시지가 나온다.

	![](http://soonmo.github.io/images/18-2.png)

  * **보안** &#8211; **액세스 제어**, 로그인 및 권한 정책의 “**응용프로그램 복사**” 항목을 아래와 같이 설정한다, 화면 제일 하단의 “**적용**” 클릭

	![](http://soonmo.github.io/images/19-2.png)

## 복합기 테스트

  * 복합기 홈화면에서 &#8220;**복사**&#8221; 선택

	![](http://soonmo.github.io/images/copy_menu.png)

  * 사용자 이름, 암호 입력 (예) s1, S1

	![](http://soonmo.github.io/images/21-3.png)

  * 로그인이 정상적으로 되었는지 확인한다.

	![](http://soonmo.github.io/images/22-1.png)

  * 다른 계정으로 테스트해 본다.