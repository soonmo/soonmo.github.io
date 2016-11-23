---
title: PC Send Fax 소프트웨어
layout: page
permalink: /tutorials/fs-device-ug/pc-send-fax/
---
PC Send Fax 소프트웨어는 PC 에서 전자 문서를 복합기의 아날로그 팩스를 통해서 보낼 때 사용하는 소프트웨어 입니다.

## 팩스 테스트 환경 만들기

아날로그 팩스 회선이 없기 때문에 LAN Fax 설정을 한 후 팩스 테스트를 진행하고 추후 아날로그 회선이 가능한 환경에서 본 가이드를 사용해서 직접 기능을 확인해 보세요.

  * 팩스 탭 
      * “**팩스 발신 활성화**” 체크
      * 팩스 발신 방법: “**LAN 팩스 서비스**”
      * “**LAN 팩스 설정**” 탭 클릭

		![](http://soonmo.github.io/images/1-2-(1).png)

  * 다음 화면과 같이 설정 
      * 타사 LAN 팩스 제품: “**통지 기능이 없는 일반 LAN 팩스 제품**”
      * UNC 폴더 경로: \\dc\lanfax
      * Windows 도메인: ppsdemo
      * 사용자 이름: sn (본인 아이디: s1, …)
      * 암호: Sn (본인 암호: S1, …)
      * “**폴더 이용 권한 확인**” 클릭
      * 화면 제일 하단 “**적용**” 클릭

		![](http://soonmo.github.io/images/2-1-(1).png)

  * 보안-액세스 제어, 로그인 및 권한 정책의 &#8220;**팩스 응용 프로그램**&#8220;을 아래와 같이 설정 후 **&#8220;적용**&#8221; 클릭

	![](http://soonmo.github.io/images/4-2-(1).png)

## 복합기 테스트

  * ADF 에 용지 적재 후 복합기 홈화면 &#8220;**팩스**&#8221; 선택

	![](http://soonmo.github.io/images/5-2-(1).png)

  * 인증

	![](http://soonmo.github.io/images/MFP-Auth.png)

  * 팩스 번호를 입력 하거나 주소록에서 이름 선택

	![](http://soonmo.github.io/images/7-2-(2).png)

  * 화면 상단 &#8220;**팩스 발신**&#8221; 선택

	![](http://soonmo.github.io/images/Send-Fax-Button.png)

  * 확인

	![](http://soonmo.github.io/images/8-2-(1).png)

  * “윈도우키+R” \\dc\lanfax

	![](http://soonmo.github.io/images/9-3.png)

  * TIFF 이미지 파일, hpf 파일 한쌍이 있다. 
      * TIFF 이미지 열어서 확인
      * 메모장으로 hpf 파일 열어서 내용 확인

		![](http://soonmo.github.io/images/10-2-(1).png)

## PC Send Fax 소프트웨어 설치

  * \\dc\lab_sw “PC-Send-Fax-Driver” 폴더

	![](http://soonmo.github.io/images/11-2-(1).png)

  * “HP\_MFP\_SendFax300_64bit” 더블 클릭 후 압푹 해제한다

	![](http://soonmo.github.io/images/12-2-(1).png)

  * 시작 – 장치 및 프린터, 프린터 추가
  * 로컬 프린터 추가

	![](http://soonmo.github.io/images/14-1-(1).png)

  * 새포트 만들기, “Standard TCP/IP port”

	![](http://soonmo.github.io/images/15-2.png)

  * 본인의 프린터 IP 주소 입력 (예) 172.16.10.151

	![](http://soonmo.github.io/images/16-2.png)

  * 디스크 있음

	![](http://soonmo.github.io/images/17-2-(1).png)

  * 찾아보기 “c:\HP PC Send Fax 64bit Driver”

	![](http://soonmo.github.io/images/18-2-(1).png)

  * 다음

	![](http://soonmo.github.io/images/19-2-(1).png)

  * 다음

	![](http://soonmo.github.io/images/20-2-(2).png)

  * &#8220;**공유안함**&#8220;, 다음

	![](http://soonmo.github.io/images/21-2-(1).png)

  * 테스트 페이지 인쇄

	![](http://soonmo.github.io/images/22-3.png)

  * LAN Fax 구성으로는 지원이 안된다는 경고 메시지…, 무시하고 &#8220;**확인**&#8220;

	![](http://soonmo.github.io/images/23-2.png)

  * 설정 탭 
      * 발신자 이름: 홍길동
      * 팩스번호: 02-2199-1111
      * 회사이름: hp
      * 음성전화번호: 02-2199-2222
      * 미리보기 체크

		![](http://soonmo.github.io/images/24-2.png)

  * 팩스 작업 탭 
      * 수신자 이름: 김유신
      * 팩스 번호: 02-1234-5678
      * &#8220;**미리보기 후 전송**&#8221; 클릭

		![](http://soonmo.github.io/images/25-2.png)

  * 미리보기 화면을 본 후 &#8220;**팩스 취소**&#8221; 클릭

	![](http://soonmo.github.io/images/26-2.png)