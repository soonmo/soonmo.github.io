---
title: 모델 드라이버, UPD 설치 및 비교
layout: page
permalink: /tutorials/upd/discrete-vs-upd/
---
이번 실습에서는 모델 드라이버 (모델 별 전용)와 UPD (Universal Print Driver)를 각각 설치해 보고 차이점을 비교해 본다.

## <span id="i">기존에 설치되어 있는 프린트 드라이버 삭제</span>

  * 도메인 사용자 (ppsdemo\s**n**) 계정으로 로그-인
  * 윈도우키 + R, **printmanagement.ms**c 입력 후 “엔터” 키를 누른다.
  * **인쇄 서버 > 컴퓨터이름 (로컬) > 프린터** 클릭, 삭제하고자 하는 프린터 이름 위에 마우스 포인터를 위치 시킨 후 마우스 오른쪽 버튼 클릭 – **삭제** 클릭

	![](http://soonmo.github.io/images/2-9.png)

  * “**예**” 클릭

	![](http://soonmo.github.io/images/3-7.png)

  * HP Universal Printing PCL 6 프린터도 같은 방법으로 삭제 (있으면)
  * **인쇄서버 > 컴퓨터이름(로컬) > 드라이버** 클릭

	![](http://soonmo.github.io/images/printmanagement-01.png)

  * 지우고자 하는 드라이버에 마우스 포인터를 위치시킨 후 마우스 오른쪽 버튼 클릭, “**드라이버** **패키지** **제거**” 클릭

	![](http://soonmo.github.io/images/printmanagement-02.png)

## <span id="i-2">모델 드라이버 설치</span>

  * \\dc\lab_sw 열고 “drivers” 폴더 안에 본인의 복합기 기종에 맞는 드라이버를 바탕화면으로 복사한다. (또는 http://www.hp.com 에서 드라이버를 다운로드 받는다.)
  * 드라이버 파일을 더블 클릭 후 압축 해제하는 창이 뜨면 “**예**”를 클릭, ㈜ 드라이버 파일이 저장되는 경로를 기억해 둔다.

	![](http://soonmo.github.io/images/5-7.png)

  * 시작 – 장치 및 프린터 클릭, “**프린터 추가**” 클릭

	![](http://soonmo.github.io/images/add-printer.png)

  * “**로컬 프린터 추가**” 클릭

	![](http://soonmo.github.io/images/6-6.png)

  * **새 포트 만들기**, 포트 종류 “**Standard TCP/IP Port**” 선택 후 “**다음**” 클릭

	![](http://soonmo.github.io/images/7-7.png)

  * IP 주소에 본인의 복합기 IP 주소 입력 (예, 172.16.10.15n), “**프린터를 검색하고 사용할 드라이버를 자동으로 선택**” 앞에 체크 **해제** 후 “**다음**” 클릭

	![](http://soonmo.github.io/images/8-7.png)

  * “**디스크 있음**” 클릭

	![](http://soonmo.github.io/images/9-7.png)

  * “**찾아 보기**” 클릭

	![](http://soonmo.github.io/images/10-6.png)

  * 드라이버 경로 선택 후 “**열기**” – “**확인**” 클릭

	![](http://soonmo.github.io/images/11-5.png)

  * 모델이 여러 개 나오면 본인 복합기 모델을 선택 후 “**다음**” 클릭

	![](http://soonmo.github.io/images/12-6.png)

  * “**다음**” 클릭

	![](http://soonmo.github.io/images/13-4.png)

  * 드라이버 설치 진행

	![](http://soonmo.github.io/images/14-4.png)

  * “**공유 안 함**” 선택 후 “**다음**” 클릭

	![](http://soonmo.github.io/images/15-4.png)

  * “**테스트 페이지**” 인쇄 클릭, “**마침**” 클릭

	![](http://soonmo.github.io/images/16-5.png)

## <span id="UPD">UPD 설치</span>

  * \\dc\lab_sw 열고 “UPD” 폴더 안에 “upd-pcl6-x64-6.0.0.18849.exe” 파일을 바탕화면으로 복사한다. (또는 http://www.hp.com/go/upd 에서 다운로드 받는다.)
  * 바탕화면의 upd 설치 파일 더블 클릭

	![](http://soonmo.github.io/images/17-6.png)

  * “**Unzip**” 클릭, ㈜ 압축 파일이 해제되어 복사되는 폴더를 잘 기억해 둔다.

	![](http://soonmo.github.io/images/18-5.png)

  * “**확인**” 클릭

	![](http://soonmo.github.io/images/19-5.png)

  * 사용자 계정 콘트롤 창이 뜨면 “**예**” 클릭
  * “**예**” 클릭

	![](http://soonmo.github.io/images/21-4.png)

  * “**일반 모드**” 선택 후 “**다음**” 클릭

	![](http://soonmo.github.io/images/22-6.png)

  * “**로컬 프린터 추가**” 클릭

	![](http://soonmo.github.io/images/23-5.png)

  * “**기존 포트 사용**” 선택 후 모델 드라이버 설치 때 만들 었던 포트 선택 후 “**다음**” 클릭

	![](http://soonmo.github.io/images/24-5.png)

  * “HP Universal Printing PCL 6 (6.0.0)” 선택 후 “다음” 클릭; **(질문)** “HP Universal Printing PCL 6” 와 “HP Universal Printing PCL 6 (v6.0.0)” 의 차이점은?

	![](http://soonmo.github.io/images/25-4.png)

  * “**다음**” 클릭

	![](http://soonmo.github.io/images/26-5.png)

  * 드라이버가 설치될 때 까지 기다린다.
  * “**공유 안 함**” 선택 후 “**다음**” 클릭
  * “**테스트 페이지 인쇄**” 클릭, 테스트 페이지가 출력되면 “**닫기**” 클릭
  * 아래와 같은 화면이 나오면 기다린다.

	![](http://soonmo.github.io/images/30-2.png)

  * “**마침**” 클릭

	![](http://soonmo.github.io/images/31-2.png)

## <span id="_UPD">모델 드라이버와 UPD 비교</span>

  * 모델 드라이버, UPD의  **프린터 속성** &#8211; **장치 설정**  탭을 각각 클릭 해서 비교해 본다.

	![](http://soonmo.github.io/images/32-1.png)

	![](http://soonmo.github.io/images/32-2.png)

  * 모델 드라이버, UPD의  **인쇄 기본 설정** &#8211; **고급**  탭을 각각 클릭 해서 비교해 본다.

	![](http://soonmo.github.io/images/33-1-1.png)

	![](http://soonmo.github.io/images/33-2.png)

  * ㈜ 모델 드라이버와 UPD 일반 모드는 사용자 입장에서 전혀 차이가 없음