---
title: UPD 작업 저장 (Stored Job)
layout: page
permalink: /tutorials/upd/stored-job/
---
UPD 의 보안 기능인 작업 저장 기능에 대한 실습을 한다. 작업 저장의 다양한 구성과 구성별 차이점을 명확히 이해하고 실제로 어떻게 작동하는지 실습을 통해서 확인한다.

## <span id="i">실습용 큐 설치</span>

  * 이전 실습에서 설치한 UPD 프린터를 삭제한다. (시작 > 실행 “**printmanagement.msc**”)
  * \\dc\lab_sw 공유 폴더를 열고 UPD 폴더 내 “upd-pcl6-x64-6.0.0.18849.exe” 파일을 PC 바탕화면으로 복사

	![](http://soonmo.github.io/images/2-13.png)

  * \\dc\lab_sw 공유 폴더의 **“UPD\_HP\_JOB\_STORAGE\_Lab.zip”** 파일을 PC 바탕화면으로 복사

	![](http://soonmo.github.io/images/2-1-1.png)

  * “**upd-pcl6-x64-6.0.0.18849.exe**” 파일을 더블 클릭 후 “**when don unzipping open**:…” 체크 해제 후 압축 해제

	![](http://soonmo.github.io/images/3-12.png)

  * “**UPD\_HP\_JOB\_STORAGE\_Lab.zip**” 압축을 다음과 같이 “C:\HP Universal Print Driver” 폴더에 압축 해제

	![](http://soonmo.github.io/images/4-14.png)

  * “**install-upd-lab.bat**” 파일 마우스 포인터를 위치시킨 후 오른쪽 버튼 클릭 후 “**편집**” 선택

	![](http://soonmo.github.io/images/5-9.png)

  * 2번째 라인 수정: 본인 복합기 IP 주소로 변경

	![](http://soonmo.github.io/images/5-1-1.png)

	![](http://soonmo.github.io/images/5-2-1.png)

  * “**파일**” – “**저장**”

	![](http://soonmo.github.io/images/5-3-1.png)

  * “**install-upd-lab.bat**” 파일 마우스 포인터를 위치시킨 후 오른쪽 버튼 클릭 후 “관리자 권한으로 실행” 선택

	![](http://soonmo.github.io/images/6-11.png)

  * &#8220;**엔터**&#8220;

	![](http://soonmo.github.io/images/7-12.png)

  * 스크립트가 모두 실행될 때 까지 기다린다. (상당히 오랜 시간이 걸림..1A, 1B….4B 까지 8개 대기열 생성)

	![](http://soonmo.github.io/images/8-11.png)

	![](http://soonmo.github.io/images/8-1-1.png)

  * 윈도우키 + R, “**printmanagement.msc**” (엔터), ㈜ 모두 8개의 인쇄 대기열이 만들어 졌다.

	![](http://soonmo.github.io/images/9-11.png)

## <span id="1A_StoredJob-PINtoPRINT-DefaultPIN-1234">1A – StoredJob-PINtoPRINT-DefaultPIN-1234</span>

  * **드라이버 사전 구성 유틸리티** 실행
  * 파일 &#8211; 열기,  “**C:\HP Universal Print Driver\UPD_CFM\1A-StoredJob-PINtoPRINT-DefaultPIN-1234.cfm**” 
      * 작업 저장 모드를 확장해서 설정 상태 확인
      * ㈜ 기본 PIN 을 설정하지 않으면 “0000” 으로 설정 됨

	![](http://soonmo.github.io/images/2-14.png)

  * 마우스 오른쪽 클릭 > **인쇄 기본값 설정**

	![](http://soonmo.github.io/images/3-13.png)

  * “**작업 저장**” 탭 클릭 해서 드라이버 설정을 확인

	![](http://soonmo.github.io/images/4-15.png)

  * 테스트 페이지 인쇄

	![](http://soonmo.github.io/images/5-10.png)

  * 프린터에 사용자 계정으로 폴더가 생성되고 그 안에 인쇄 작업이 저장됨

	![](http://soonmo.github.io/images/6-12.png)

  * 프린터(복합기)로 이동
  * “**장치 메모리에서 불러 오기**” 선택

	![](http://soonmo.github.io/images/7-1-2.png)

  * 사용자명 폴더 터치 (예; Sn)

	![](http://soonmo.github.io/images/7-2-2.png)

  * 문서 선택 (테스트 페이지)

	![](http://soonmo.github.io/images/7-3-1.png)

  * PIN 입력 화면이 나오면 PIN 입력 (1234)

	![](http://soonmo.github.io/images/7-4-1.png)

	![](http://soonmo.github.io/images/7-5-1.png)

  * 상단의 “**장치 메모리에서 불러오기**” 터치하면 테스트 페이지가 인쇄된다.

	![](http://soonmo.github.io/images/7-6-1.png)

  * “**테스트 페이지**” 선택

	![](http://soonmo.github.io/images/7-7-1.png)

  * “**삭제**” 터치

	![](http://soonmo.github.io/images/7-8-1.png)

  * &#8220;**확인**&#8220;

## <span id="1B_StoredJob-PINtoPRINT-DefaultPIN-1234-Locked">1B – StoredJob-PINtoPRINT-DefaultPIN-1234-Locked</span>

  * **드라이버 사전 구성 유틸리티** 실행
  * 파일 &#8211; 열기, “**C:\HP Universal Print Driver\UPD_CFM\1B-StoredJob-PINtoPRINT-DefaultPIN-1234-Lock.cfm**”

	![](http://soonmo.github.io/images/2-15.png)

  * 마우스 오른쪽 클릭 > 인쇄 기본값 설정

	![](http://soonmo.github.io/images/3-13.png)

  * “**작업 저장**” 탭 클릭 해서 드라이버 설정을 확인

	![](http://soonmo.github.io/images/4-16.png)

  * “**테스트 인쇄**” 수행 (1A-StoredJob-PINtoPRINT-DefailtPIN-1234 참조)

## <span id="2A_StoredJob-PINtoPRINT-RequestPIN">2A – StoredJob-PINtoPRINT-RequestPIN</span>

  * **드라이버 사전 구성 유틸리티** 실행
  * 파일 &#8211; 열기, “**C:\HP Universal Print Driver\UPD_CFM\2A-StoredJob-PINtoPRINT-RequestPIN.cfm**”

	![](http://soonmo.github.io/images/2-16.png)

  * 마우스 오른쪽 클릭 > 인쇄 기본값 설정

	![](http://soonmo.github.io/images/3-13.png)

  * “**작업 저장**” 탭 클릭 해서 드라이버 설정을 확인

	![](http://soonmo.github.io/images/4-17.png)

  * 테스트페이지 인쇄

	![](http://soonmo.github.io/images/5-10.png)

  * PIN을 요구함, PIN 입력

	![](http://soonmo.github.io/images/6-1-2.png)

  * &#8220;**확인**&#8221; 클릭

	![](http://soonmo.github.io/images/6-2-1.png)

  * 프린터로 이동해서 인쇄를 한다 (1A-StoredJob-PINtoPRINT-DefailtPIN-1234 참조)

## <span id="2B_StoredJob-PINtoPRINT-RequestPIN-Locked">2B – StoredJob-PINtoPRINT-RequestPIN-Locked</span>

  * **드라이버 사전 구성 유틸리티** 실행
  * 파일 &#8211; 열기, “**C:\HP Universal Print Driver\UPD_CFM\2B-StoredJob-PINtoPRINT-RequestPIN-Lock.cfm**”


	![](http://soonmo.github.io/images/2-17.png)

  * 마유스 오른쪽 클릭 > 인쇄 기본값 설정

	![](http://soonmo.github.io/images/3-13.png)

  * “**작업 저장**” 탭 클릭 해서 드라이버 설정을 확인

	![](http://soonmo.github.io/images/4-18.png)

  * 테스트 페이지 인쇄
  * 프린터로 이동해서 인쇄를 한다 (1A-StoredJob-PINtoPRINT-DefailtPIN-1234 참조)

## <span id="3A_StoredJob-EncryptJob-Automatic">3A – StoredJob-EncryptJob-Automatic</span>

  * 드라이버 사전 구성 유틸리티 실행
  * 파일 &#8211; 열기, “**C:\HP Universal Print Driver\UPD_CFM\3A-StoredJob-EncryptJob-Automatic.cfm**”

	![](http://soonmo.github.io/images/2-18.png)

  * 마우스 오른쪽 클릭 > 인쇄 기본값 설정

	![](http://soonmo.github.io/images/3-13.png)

  * “**작업 저장**” 탭 클릭 해서 드라이버 설정을 확인

	![](http://soonmo.github.io/images/4-19.png)

  * 테스트 페이지 인쇄
  * 암호 입력 (문자, 숫자 모두 가능)

	![](http://soonmo.github.io/images/6-2-2.png)

  * ㈜ 기본 암호로 저장에 체크하면 암호가 저장됨

	![](http://soonmo.github.io/images/6-3-1.png)

  * “**확인**” 클릭

	![](http://soonmo.github.io/images/7-13.png)

  * 프린터(복합기)로 이동
  * “**장치 메모리에서 불러오기**” 선택

	![](http://soonmo.github.io/images/7-1-2.png)

  * 사용자명 폴더 터치 (예; Sn)

	![](http://soonmo.github.io/images/7-2-2.png)

  * 문서 선택 (테스트 페이지)

	![](http://soonmo.github.io/images/7-3-1.png)

  * 암호 입력화면 이 나오면 암호를 입력한다.

	![](http://soonmo.github.io/images/7-4-2.png)

	![](http://soonmo.github.io/images/7-5-2.png)

  * 상단의 “**장치 메모리에서 불러오기**” 녹색 버튼 터치해서 인쇄

	![](http://soonmo.github.io/images/7-8-1.png)

## <span id="3B_StoredJob-EncryptJob-Automatic-Locked">3B – StoredJob-EncryptJob-Automatic-Locked</span>

  * **드라이버 사전 구성 유틸리티** 실행
  * 파일 &#8211; 열기, “**C:\HP Universal Print Driver\UPD_CFM\3A-StoredJob-EncryptJob-Automatic-Locked.cfm**”

	![](http://soonmo.github.io/images/2-19.png)

  * 마우스 오른쪽 클릭 > 인쇄 기본값 설정

	![](http://soonmo.github.io/images/3-13.png)

  * “**작업 저장**” 탭 클릭 해서 드라이버 설정을 확인

	![](http://soonmo.github.io/images/4-20.png)

  * 시험 인쇄 출력
  * 프린터로 이동해서 인쇄를 한다 (1A-StoredJob-PINtoPRINT-DefailtPIN-1234 참조)

## <span id="4A_StoredJob-EncryptJob-Disabled">4A – StoredJob-EncryptJob-Disabled</span>

  * **드라이버 사전 구성 유틸리티** 실행
  * 파일 &#8211; 열기, “**C:\HP Universal Print Driver\UPD_CFM\4A-EncryptJob-Disabled.cfm**”

	![](http://soonmo.github.io/images/2-20.png)

  * 마우스 오른쪽 클릭 > 인쇄 기본값 설정

	![](http://soonmo.github.io/images/3-13.png)

  * “**작업 저장**” 탭 클릭 해서 드라이버 설정을 확인

	![](http://soonmo.github.io/images/3-14.png)

  * 테스트 페이지 인쇄
  * &#8220;**확인**&#8221; 클릭

	![](http://soonmo.github.io/images/6-13.png)

  * 프린터로 이동해서 인쇄를 한다 (1A-StoredJob-PINtoPRINT-DefailtPIN-1234 참조) 
      * ㈜ PIN 이나 암호를 요구하지 않음

	![](http://soonmo.github.io/images/7-6-2.png)

## <span id="4B_StoredJob-EncryptJob-Disabled-Locked">4B – StoredJob-EncryptJob-Disabled-Locked</span>

  * **드라이버 사전 구성 유틸리티** 실행
  * 파일 &#8211; 열기, “**C:\HP Universal Print Driver\UPD_CFM\4B-EncryptJob-Disabled-Locked.cfm**”

	![](http://soonmo.github.io/images/2-21.png)

  * 마우스 오른쪽 클릭 > 인쇄 기본값 설정

	![](http://soonmo.github.io/images/3-13.png)

  * “**작업 저장**” 탭 클릭 해서 드라이버 설정을 확인

	![](http://soonmo.github.io/images/3-15.png)

  * 테스트 페이지 인쇄
  * 프린터로 이동해서 인쇄를 한다 (1A-StoredJob-PINtoPRINT-DefailtPIN-1234 참조) 
      * ㈜ PIN 이나 암호를 요구하지 않음