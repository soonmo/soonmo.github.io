---
title: Scan to network folder
layout: page
permalink: /tutorials/fs-device-ug/scan-to-network-folder/
---
메일서버를 사용할 수 없는 환경이거나 스캔량이 많아서 메일서버에 부담을 주는 경우에는 파일서버로 스캔한 문서를 바로 전송할 수 있다. 본 실습은 액세스 제어와 연동해서 좀 더 쉽고 효율적으로 공유 폴더로 문서를 전송하는 방법에 대해서 알아 본다.

## <span id="i">네트웍 폴더에 저장-기본</span>

  * 스캔/디지털 전송 – 네트워크 폴더 설정에 저장, “**네트워크 폴더에 저장 활성화**” 체크 후 화면 하단 “**적용**” 클릭

	![](http://soonmo.github.io/images/1-1.png)

  * 노트북에 c:\scan 폴더 생성
  * c:\scan 폴더 마우스 오른쪽 클릭 후 “**공유대상**” – “**특정사용자**”

	![](http://soonmo.github.io/images/4-1.png)

  * 파트너 계정 추가 (예) s2, 사용자 권한 수준을 “**읽기/쓰기**” 로 변경, &#8220;**공유**&#8221; 클릭

	![](http://soonmo.github.io/images/5-1.png)

  * &#8220;**완료**&#8221; 클릭

	![](http://soonmo.github.io/images/6-1.png)

  * 파트너 PC 에서 “**원도우키+R**” 누른 후 \\본인PC이름\SCAN, 아무 파일이나 복사 및 삭제 테스트가 잘되는지 확인

	![](http://soonmo.github.io/images/7-1.png)

  * 복합기 홈화면에서 “**네트워크 폴더에 저장**” 선택, ADF에 스캔할 문서 적재

	![](http://soonmo.github.io/images/8-1.png)

  * 빠른 설정의 “**흑백 PDF**” 선택, 폴더경로 아래 부분의 연두색 **+** 기호 선택

	![](http://soonmo.github.io/images/9-2.png)

  * 앞서 설정한 본인 PC의 네트웍 공유 폴더 입력, (예) \\Student-1\SCAN, ㈜ 공유 폴더 입력시 영어로 키보드 레이아웃을 변경해야 하는데 무척 불편함. 해결 방법은 ? Tip 1 참조

	![](http://soonmo.github.io/images/10-1.png)

  * 계정 정보 입력 
      * 사용자 이름: s**<u>n</u>**
      * 암호: S**<u>n</u>**
      * 도메인: ppsdemo

		![](http://soonmo.github.io/images/11-1.png)

  * “**네트워크 폴더에 저장**” 선택 후 “**확인**”

	![](http://soonmo.github.io/images/12-1.png)

	![](http://soonmo.github.io/images/12-1-1.png)

  * 공유 폴더 (c:\scan) 에 스캔된 문서가 저장되었는지 확인한다.

	![](http://soonmo.github.io/images/13-1.png)

## <span id="Tip">Tip 키보드 레이아웃 설정 변경</span>

  * 일반 &#8211; 제어판 사용자 정의
  * 키보드 레이아웃: 한국어(한글), 영어(미국식) 만 선택하고 나머지는 선택 해제

	![](http://soonmo.github.io/images/Keyboard_layout.png)

## <span id="i-2">네트웍 폴더에 저장-고급</span>

스캔한 문서를 네트웍 공유 폴더에 사용자 별 서브 디렉토리에 저장하려면 다음과 같이 설정한다.

  * 스캔/디지털 전송 – 네트웍크 폴더 설정에 저장, 빠른 설정 아래 “**추가**” 버튼 클릭

	![](http://soonmo.github.io/images/15-1.png)

  * 다음과 같이 설정 후 “**다음**” 클릭 
      * 고속 설정 제목: 문서 스캔
      * 버튼 위치: 시작 화면
      * 고속 설정 설명: 문서를 스캔 후 파일 서버의 개인 폴더로 전송합니다.
      * 고속 설정 시작 옵션: “**선택하자마자 시작됩니다**”
      * 원본 면 개수 메시지 창: “**원본 면 개수 메시지 창**”

	![](http://soonmo.github.io/images/16-1.png)

  * 폴더 설정, 공유 폴더 또는 FTP 폴더에 저장 아래 “**추가**” 버튼 클릭

	![](http://soonmo.github.io/images/17-1.png)

  * 네트워크 폴더 경로 추가 
      * UNC 폴더 경로: \\dc\scan
      * 사용자 정의 하위폴더: “**%SECURITY_USERNAME%**”, 사용자의 하위폴더 액세스 제안
      * 인증 설정: “**제어판에서 로그인한후 사용자의 인증서를 사용하여 연결합니다**”
      * Windows 도메인: ppsdemo
      * &#8220;**확인**&#8221; 클릭

	![](http://soonmo.github.io/images/18-1.png)

  * “**작업을 시작하기 전 폴더 이용 권한을 확인하십시오**” 해제 후 “**다음**” 클릭

	![](http://soonmo.github.io/images/19-1.png)

  * &#8220;**다음**&#8220;

	![](http://soonmo.github.io/images/20-1.png)

  * &#8220;**다음**&#8220;

	![](http://soonmo.github.io/images/21-1.png)

  * 첨부 설정 
      * 파일 이름 접두사: “**사용자이름(%SECURITY_USERNAME%)**”
      * 기본 파일 이름: **\_문서\_**
      * 파일 이름 접미사: “**날짜(%DEVICE\_DATE\_YYYYMMDD%)**”
      * 파일 이름 미리 보기: “**업데이트 미리 보기**” 클릭해서 확인
      * 기본 해상도: **200dpi**

		![](http://soonmo.github.io/images/22-2.png)

  * &#8220;**마침**&#8220;

	![](http://soonmo.github.io/images/23-1.png)

  * 다음과 같은 충돌 메시지가 나타난다. (네트워크 로그온 인증 필요)

	![](http://soonmo.github.io/images/24-1.png)

  * 보안 – 액세스 제어, 로그인 및 권한 정책의 “**네트워크 폴더 응용 프로그램**”을 아래와 같이 설정한다. &#8220;**적용**&#8221; 클릭

	![](http://soonmo.github.io/images/25-1.png)

## <span id="i-3">복합기 테스트</span>

  * ADF에 스캔할 문서 적재 후 복합기 홈화면에서 “**문서 스캔**” 선택

	![](http://soonmo.github.io/images/26-1.png)

  * 인증

	![](http://soonmo.github.io/images/27-1.png)

  * 양면, 단면 스캔 선택 후 &#8220;**스캔**&#8220;

	![](http://soonmo.github.io/images/28.png)

  * 확인

	![](http://soonmo.github.io/images/29-1.png)

  * 노트북에서 “**윈도우키 + R**” 후 \\dc\scan\사용자명 , (예) \\dc\scan\s1

	![](http://soonmo.github.io/images/30.png)