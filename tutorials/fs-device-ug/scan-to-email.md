---
title: Scan to email
layout: page
permalink: /tutorials/fs-device-ug/scan-to-email/
---
복합기에서 스캔한 문서를 메일 전송 서버를 통해서 전송하는 방식으로 로컬 인증, LDAP 인증 설정과 연동되면 강력해진다. 어떻게 작동하는지 이번 실습을 통해서 살펴 본다.

## <span id="__SMTP">메일 전송 서버 (SMTP) 설정</span>

  * “**스캔/디지털 전송**” &#8211; &#8220;**전자우편**&#8221; (좌측 메뉴) 클릭, 발신 **전자우편 서버(SMTP)** 하단 “**추가**” 메뉴 클릭

	![](http://soonmo.github.io/images/1.png)

  * SMTP 서버 주소 입력 후 &#8220;**다음**&#8221; 클릭

	![](http://soonmo.github.io/images/2.png)

  * &#8220;**다음**&#8221; 클릭

	![](http://soonmo.github.io/images/3.png)

  * **서버에 인증이 필요하지 않습니다**. “**다음**”

	![](http://soonmo.github.io/images/4.png)

  * &#8220;**다음**&#8220;

	![](http://soonmo.github.io/images/5.png)

  * 테스트 전자우편 보낼 주소: [s**n**@ppsdemo.net](mailto:sn@ppsdemo.net) (예) <s1@ppsdemo.net> 후 “**테스트**” 클릭

	![](http://soonmo.github.io/images/6.png)

  * &#8220;**마침**&#8221; 클릭

	![](http://soonmo.github.io/images/7.png)

## <span id="i">메일 수신 확인</span>

  * IE 주소에 [http://mail.ppsdemo.net](http://mail.ppsdemo.net/) 입력 
      * 사용자명: 이메일 주소, (예) <s1@ppsdemo.net>
      * 암호: 계정 암호, (예)S1
      * “**로그인**” 클릭

		![](http://soonmo.github.io/images/8.png)

  * 메일 확인

	![](http://soonmo.github.io/images/9.png)

	![](http://soonmo.github.io/images/9-1.png)

## <span id="i-2">세부 설정</span>

  * 주소 및 메시지 필드 제어 
      * 보내는 사람: **사용자 주소(로그인 필수)** , “**사용자 편집 가능**” 해제
      * 받는 사람: **사용자 주소(로그인 필수)**
      * 제목: 디지털 전송
      * 메시지: 안녕하세요? 첨부문서는 hp 디지털 복합기에서 200dpi PDF로 스캔한 문서입니다. 감사합니다.

		![](http://soonmo.github.io/images/11.png)

  * 스캔 설정 
      * 이미지 미리 보기: “**미리 보기 필요**”
      * **여러 장의 페이지 급지 인식**: 해제
      * ㈜ 선택이 될 때와 해제될 때의 차이점이 무엇인가?

		![](http://soonmo.github.io/images/12.png)

  * 첨부 설정 
      * 기본 해상도: **200dpi**
      * 파일 이름 접두사: “**사용자이름(%SECURITY_USERNAME%)**”
      * 기본 파일 이름: **\_문서\_**
      * 파일 이름 접미사: “**날짜(%DEVICE\_DATE\_YYYYMMDD%)**”
      * 파일 이름 미리 보기: “**업데이트 미리 보기**” 클릭해서 확인
      * 여러 파일로 스캔: 이 옵션을 선택하면 1장당 1개의 PDF 파일로 생성한다.
      * &#8220;**적용**&#8221; 클릭

		![](http://soonmo.github.io/images/13.png)

  * 보안 – 액세스 제어, 로그인 및 권한 정책의 “**전자우편 응용 프로그램**”을 아래와 같이 설정한다.

	![](http://soonmo.github.io/images/14.png)

  * &#8220;**적용**&#8221; 클릭

## <span id="i-3">복합기 테스트</span>

  * 복합기 홈화면에서 “**전자우편**” 선택

	![](http://soonmo.github.io/images/15.png)

  * 사용자 이름, 암호 입력

	![](http://soonmo.github.io/images/16.png)

  * ㈜ 보내는 사람 변경 불가능하다. 
      * ADF (문서 공급기) 에 스캔할 문서를 3~4장 정도 적재한다.\
      * 스크린 상단의 “전자 우편 전송” 선택

		![](http://soonmo.github.io/images/17.png)

  * 미리보기: 스캔된 문서가 복합기의 화면에 나타난다.

	![](http://soonmo.github.io/images/18.png)

  * 화면 하단의 “**확대(돋보기)**” 아이콘 선택하면 스캔된 문서가 확대된다.

	![](http://soonmo.github.io/images/magnifier.png)

	![](http://soonmo.github.io/images/19.png)

  * 화면 하단의 “**썸네일**” 아이콘 선택

	![](http://soonmo.github.io/images/thumbnail.png)

	![](http://soonmo.github.io/images/20.png)

  * 페이지 삭제 &#8211; 첫번째 페이지 선택 후 좌측 쓰레기통 아이콘 선택

	![](http://soonmo.github.io/images/delete.png)

  * 페이지 삭제 확인 메시지가 나타나면 “**삭제**” 버튼 선택

	![](http://soonmo.github.io/images/21.png)

  * 페이지 순서 바꾸기 – 첫번째 페이지 선택 후 좌측 페이지 순서 바꾸기 아이콘 선택

	![](http://soonmo.github.io/images/22.png)

	![](http://soonmo.github.io/images/recorder.png)

  * 마지막 페이지 위에 아이콘 선택해서 마지막 페이지로 이동

	![](http://soonmo.github.io/images/22.png)

  * 가로/세로 회전 – 첫번째 페이지 선택 후 문서 회전 아이콘 선택

	![](http://soonmo.github.io/images/rotate.png)

	![](http://soonmo.github.io/images/23.png)

  * 새로운 페이지 추가 – 페이지 추가 아이콘 선택

	![](http://soonmo.github.io/images/add_page.png)

	![](http://soonmo.github.io/images/24.png)

  * ADF 에 문서을 적재 후 “**스캔**” 선택
  * 화면 상단의 “**전자우편 전송**” 선택

	![](http://soonmo.github.io/images/email_app.png)

  * &#8220;**추가**&#8221; 선택

	![](http://soonmo.github.io/images/26.png)

  * &#8220;**확인**&#8220;

	![](http://soonmo.github.io/images/27.png)

## <span id="i-4">메일 수신 확인</span>

  * IE 주소에 [http://mail.ppsdemo.net](http://mail.ppsdemo.net/) 입력 
      * 사용자명: 이메일 주소, (예) <s1@ppsdemo.net>
      * 암호: 계정 암호, (예)S1
      * “**로그인**” 클릭
  * 메일확인

	![](http://soonmo.github.io/images/29.png)