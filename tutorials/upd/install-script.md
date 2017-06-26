---
title: 드라이버 자동 설치 스크립트
layout: page
permalink: /tutorials/upd/install-script/
---
프린터 추가 마법사나 벤더에서 제공하는 설치 프로그램을 이용해서 설치를 하게 되면 단계가 많아서 일반 사용자가 설치하기가 불편하고 시간도 많이 걸린다. 이를 자동화해서 쉽게 설치하려면 Windows 에서 제공하는 Rundll32 나 UPD의 경우 install.exe 를 이용해서 스크립트를 만들면 된다. 이번 실습에서는 스크립트를 이용해서 드라이버를 설치해 보겠다.

  * [실습용 샘플 파일 다운로드](https://soonmo.net/owncloud/index.php/s/1EOLu88ntdAs6oX)

  * “**HP\_프린터\_드라이버팩_Beta.exe**” 를 바탕화면으로 복사 후 더블 클릭
  * **2** 입력 후 (엔터)

  ![](http://soonmo.github.io/images/install_script_01.png)

  * **복합기 IP** 를 입력 후 엔터 (예, 172,16,10.15n)

  ![](http://soonmo.github.io/images/install_script_02.png)

  * **4** 입력 후 엔터

  ![](http://soonmo.github.io/images/install_script_03.png)

  * 스크립트가 실행되면서 포트를 만들고 프린터 드라이버를 자동으로 설치한다.

  ![](http://soonmo.github.io/images/install_script_04.png)

  * **2** 를 입력 후 엔터 (설치 종료)

  ![](http://soonmo.github.io/images/install_script_05.png)

  * **시작** – **장치 및 프린터**, 드라이버가 설치가 되었는지 확인

  ![](http://soonmo.github.io/images/install_script_06.png)

  * 설치 스크립트의 내용을 확인한다. c:\HP\_Print\_Drivers  에 “**printer_install.bat**” 파일을  메모장으로 열어서 내용을 확인할 수 있음

  ![](http://soonmo.github.io/images/install_script_07.png)