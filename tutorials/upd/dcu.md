---
title: 드라이버 사전 구성
layout: page
permalink: /tutorials/upd/dcu/
---
친환경을 위해서 불필요한 칼라 출력을 줄이기 위해서 프린터 드라이버 기본 설정을 그레이스케일로 인쇄로 변경하고 싶다면 **PARK (Printer Administration Resource Kit)** 에 **Driver Configuration Utility**  솔루션으로 구현할 수 있다. 이번 실습에서는 드라이버 구성 유틸리티를 가지고 다양한 사전 구성을 연습해 본다.

  * 윈도우 + R, \\dc\lab_sw “확인” 클릭 후 UPD 폴더 안에 “**park-v1.7.8.zip**” 파일을 본인의 PC 바탕화면으로 복사 후 압축을 해제한다.

	![](http://soonmo.github.io/images/1-8.png)

  * “**driver configuration utility**”폴더로 이동

	![](http://soonmo.github.io/images/2-22.png)

  * “**hpbcfgap**” 더블 클릭

	![](http://soonmo.github.io/images/3-16.png)

  * “**앞으로 이 경고를 표시하지 않음**” 체크 후 “**확인**” 클릭

	![](http://soonmo.github.io/images/4-21.png)

  * **파일** – **열기**, **C:\HP Universal Print Driver\pcl6-x64-6.0.0.18849** 로 이동
  * “hpcpu175.cfg” 파일 선택 후 “**열기**” 클릭

	![](http://soonmo.github.io/images/6-14.png)

  * **양면 인쇄**: **참**, **용지 크기**: **A4**

	![](http://soonmo.github.io/images/7-14.png)

  * 파일 – 다른 이름으로 저장, 파일 이름: **Duplex.cfm** 입력 후 “**저장**” 클릭

	![](http://soonmo.github.io/images/8-12.png)

  * **양면 인쇄**: **참**, **잠금**에 체크, **용지 크기**: **A4**

	![](http://soonmo.github.io/images/9-12.png)

  * 파일 – 다른 이름으로 저장, 파일 이름: **Duplex_lock.cfm** 입력 후 “**저장**” 클릭

	![](http://soonmo.github.io/images/10-10.png)

  * “**제조시 기본값으로 돌리기**” 클릭

	![](http://soonmo.github.io/images/11-9.png)

  * “**그레이스케일로 인쇄**”: 사용 설정, **용지 크기**:  **A4**

	![](http://soonmo.github.io/images/12-9.png)

  * 파일 – 다른 이름으로 저장, 파일 이름: **Grayscale.cfm** 입력 후 “**저장**”  클릭

	![](http://soonmo.github.io/images/13-7.png)

  * **그레이스케일로** 인쇄: **사용 설정**, **잠금** 체크, 용지 크기: **A4**

	![](http://soonmo.github.io/images/14-5.png)

  * 파일 – 다른 이름으로 저장, 파일 이름: **Grayscale_lock.cfm** 입력 후 “**저장**” 클릭
  * 구성 편집기 창 닫음
  * 명령 프롬프트 실행, C:\HP Universal Print Driver\pcl6-x64-6.0.0.18849 로 이동

	![](http://soonmo.github.io/images/17-9.png)

  * **Install /gcfm”Duplex.cfm” /n”Duplex” /sm172.16.10.15n /h /q (엔터)**

	![](http://soonmo.github.io/images/18-8.png)

  * “**예**” 클릭 후 기다린다. (백그라운드로 드라이버가 설치 됨)
  * **시작 > 장치 및 프린터**, Duplex 마우스 오른쪽 클릭, **인쇄 기본 설정 > Duplex 클릭**

	![](http://soonmo.github.io/images/19-8.png)

  * “**완료**” 탭 클릭, ㈜ 양면 인쇄가 디폴트로 사전 구성 됨

	![](http://soonmo.github.io/images/20-5.png)

  * 명령 프롬프트 에서 차례로 다음 명령을 수행한다. 각 명령 후 드라이버가 설치가 끝나면 다름 명령을 수행 
      * **Install /gcfm”Duplex\_lock.cfm” /n”Duplex\_lock” /sm172.16.10.15n /h /q (엔터)**
      * **Install /gcfm”Grayscale.cfm” /n”Grayscale” /sm172.16.10.15n /h /q (엔터)**
      * **Install /gcfm”Grayscale\_lock.cfm” /n”Grayscale\_lock” /sm172.16.10.15n /h /q (엔터)**
  * 새로 설치된 드라이버의 인쇄 기본 설정값을 확인한다.

	![](http://soonmo.github.io/images/22-1-1.png)

	![](http://soonmo.github.io/images/22-2-1.png)

	![](http://soonmo.github.io/images/22-3-1.png)

	![](http://soonmo.github.io/images/22-4-1.png)