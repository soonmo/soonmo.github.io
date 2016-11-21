---
id: 1446
title: UPD ADMX 정책 적용 (양면인쇄)
date: 2016-05-07T09:15:47+00:00
author: 홍 순모
layout: page
guid: http://hpidemo.net/?page_id=1446
---
AD 환경에서 사용할 수 있도록 UPD ADMX 템플릿을 제공하고 있다. 그룹 정책 관리자에서 UPD 옵션을 변경함으로써 도메일 사용자의 UPD 인쇄 옵션을 조정할 수 있다. 본 실습에서는 강사가 사전에 양면 인쇄 정책을 설정해 놓은 AD 서버에 로그인 하면 프린터 드라이버가 자동으로 설치되면서 양면인쇄 정책이 적용되는 모습을 확인 할 수 있다.

  * Windows 로그-오프
  * 강사가 AD 에 접속해서 “**그룹 정책 관리자**” 구성 설명을 한다. 서버 쪽 설정은 다음과 같은 과정으로 진행됨 
      * PARK의 “**HP-MPP-4.4.5.admx**” 파일을 서버의 “**C:\Windows\PolicyDefinitions**” 에 복사
      * PARK 의  “**HP-MPP-4.4.5.adml**” 파일을 서버의 “**C:\Windows\PolicyDefinitions\ko-KR**” 에 복사
      * “**관리도구**” > “**그룹정책관리**”
      * “**그룹 정책 관리**” > “포리스트:ppsdemo.net” > 도메인 > “ppsdemo.net” > “**그룹 정책 개체**” > “**Default Domain Policy**”
      * 마우스 오른쪽 클릭 후 “**편집**&#8220;

<p style="padding-left: 60px;">
  <img class="alignnone size-full wp-image-1558" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/2-23.png?fit=479%2C526" alt="UPD ADMX 2" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/2-23.png?w=479 479w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/2-23.png?resize=273%2C300 273w" sizes="(max-width: 479px) 100vw, 479px" data-recalc-dims="1" />
</p>

  * “**사용자 구성**” > “**정책**” > “**관리 템플릿**” > “**HP Managed Print Policy 4.4.5**”
  * Default Print Settings
  * Duplex: **Print on both sides Lock**

<p style="padding-left: 60px;">
  <img class="alignnone size-full wp-image-1553" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/2-1-2.png?fit=701%2C641" alt="UPD ADMX 2-1" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/2-1-2.png?w=701 701w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/2-1-2.png?resize=300%2C274 300w" sizes="(max-width: 701px) 100vw, 701px" data-recalc-dims="1" />
</p>

  * 로그-온 스크립트 설정 
      * 그룹 정책 관리 편집기
      *  “**사용자 구성**” > “**정책**” > “**Windows 설정**” > “**스크립트(로그온/로그오프)**”

<p style="padding-left: 60px;">
  <img class="alignnone size-full wp-image-1554" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/3-17.png?fit=654%2C376" alt="UPD ADMX 3" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/3-17.png?w=654 654w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/3-17.png?resize=300%2C172 300w" sizes="(max-width: 654px) 100vw, 654px" data-recalc-dims="1" />
</p>

  * 로그온 더블 클릭
  * 스크립트 추가

<p style="padding-left: 60px;">
  <img class="alignnone size-full wp-image-1555" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/3-1-1.png?fit=501%2C419" alt="UPD ADMX 3-1" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/3-1-1.png?w=501 501w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/3-1-1.png?resize=300%2C251 300w" sizes="(max-width: 501px) 100vw, 501px" data-recalc-dims="1" />
</p>

  * Windows 로그-온, 스크립트가 실행되도록 기다린다. 칼라 프린터 IP 를 넣으라고 나오면 본인 복합기의 IP를 입력한다.
  * **시작 > 장치 및 프린터**, “**ColorPrinter**” 마우스 포인터를 위치킨 후 오른쪽 버튼 클릭 후 “**인쇄 기본 설정**” 선택, 아래와 같이 <span style="text-decoration: underline;">양면 인쇄가 Lock 이 되어 있다</span>.

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1557" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/4-1-3.png?fit=631%2C582" alt="UPD ADMX 4-1" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/4-1-3.png?w=631 631w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/4-1-3.png?resize=300%2C277 300w" sizes="(max-width: 631px) 100vw, 631px" data-recalc-dims="1" />
</p>