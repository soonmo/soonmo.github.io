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

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1011" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/04/4-5.png?fit=78%2C89" alt="액세스 제어 - LDAP" data-recalc-dims="1" />
</p>

  * “**In the future, do not show the warning**” 체크 후 **OK**

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1012" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/04/5-6.png?fit=630%2C151" alt="액세스 제어 - LDAP" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/04/5-6.png?w=630 630w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/04/5-6.png?resize=300%2C72 300w" sizes="(max-width: 630px) 100vw, 630px" data-recalc-dims="1" />
</p>

  * **No** 선택

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1013" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/04/6-4.png?fit=339%2C138" alt="액세스 제어 - LDAP" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/04/6-4.png?w=339 339w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/04/6-4.png?resize=300%2C122 300w" sizes="(max-width: 339px) 100vw, 339px" data-recalc-dims="1" />
</p>

  * 프로그램이 실행되면 **Ctrl + P** 를 누른다. 프로파일 이름을 적당히 입력한다. (예) HP Partner Tech U Lab

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-996" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/04/7-4.png?fit=652%2C440" alt="액세스 제어 - LDAP" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/04/7-4.png?w=652 652w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/04/7-4.png?resize=300%2C202 300w" sizes="(max-width: 652px) 100vw, 652px" data-recalc-dims="1" />
</p>

  * Host: 에 dc 입력, Fetch Base DNs 클릭 후 “DC=ppsdemo, DC=net” 선택

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-997" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/04/8-5.png?fit=655%2C441" alt="액세스 제어 - LDAP" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/04/8-5.png?w=655 655w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/04/8-5.png?resize=300%2C202 300w" sizes="(max-width: 655px) 100vw, 655px" data-recalc-dims="1" />
</p>

  * “**Currently logged on user (Active Directory only**)” 선택

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-998" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/04/9-2.png?fit=652%2C440" alt="액세스 제어 - LDAP" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/04/9-2.png?w=652 652w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/04/9-2.png?resize=300%2C202 300w" sizes="(max-width: 652px) 100vw, 652px" data-recalc-dims="1" />
</p>

  * 마침
  * Find what 에 **계정명**을 입력 후 엔터. (예) s1, 검색 결과가 나오면 CN 을 더블 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-999" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/04/11-4.png?fit=803%2C371" alt="액세스 제어 - LDAP" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/04/11-4.png?w=803 803w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/04/11-4.png?resize=300%2C139 300w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/04/11-4.png?resize=768%2C355 768w" sizes="(max-width: 803px) 100vw, 803px" data-recalc-dims="1" />
</p>

  * cn, distinguishedName 의 값을 메모한다. 
      * **cn**: s1
      * **distinguishedName**: CN=s1,CN=Users,DC=ppsdemo,DC=net

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1000" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/04/12-4.png?fit=806%2C405" alt="액세스 제어 - LDAP" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/04/12-4.png?w=806 806w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/04/12-4.png?resize=300%2C151 300w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/04/12-4.png?resize=768%2C386 768w" sizes="(max-width: 806px) 100vw, 806px" data-recalc-dims="1" />
</p>

## 내장 웹서버 설정

  * **보안** &#8211; **액세스제어** (좌측메뉴), **로그인 방법 활성화 및 구성의** LDAP 좌측의 “**설정**” 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1001" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/04/13-3.png?fit=634%2C337" alt="액세스 제어 - LDAP" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/04/13-3.png?w=634 634w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/04/13-3.png?resize=300%2C159 300w" sizes="(max-width: 634px) 100vw, 634px" data-recalc-dims="1" />
</p>

  * LDAP 로그인  사용 체크, LDAP 서버 주소: 172.16.10.10, 접두사 바인딩: cn

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1002" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/04/14-2.png?fit=542%2C382" alt="액세스 제어 - LDAP" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/04/14-2.png?w=542 542w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/04/14-2.png?resize=300%2C211 300w" sizes="(max-width: 542px) 100vw, 542px" data-recalc-dims="1" />
</p>

  * 루트 바인딩 및 검색: CN=Users,DC=ppsdemo,DC=net 입력 후 “**추가**” 클릭 
      * 입력한 이름과 이 속성 일치: **cn**
      * 이 속성으로 장치 사용자 전자우편 주소 불러오기: **mail**
      * 이 속성으로 장치 사용자의 이름 불러오기: **displayName**
      * 이 속성으로 장치 사용자의 관련 단체 불러 오기: **objectClass**

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1003" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/04/15-1.png?fit=985%2C317" alt="액세스 제어 - LDAP" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/04/15-1.png?w=985 985w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/04/15-1.png?resize=300%2C97 300w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/04/15-1.png?resize=768%2C247 768w" sizes="(max-width: 985px) 100vw, 985px" data-recalc-dims="1" />
</p>

  * **확인** 클릭
  * 다시 LDAP 좌측 &#8220;**설정**&#8221; 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1004" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/04/16-1.png?fit=651%2C415" alt="액세스 제어 - LDAP" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/04/16-1.png?w=651 651w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/04/16-1.png?resize=300%2C191 300w" sizes="(max-width: 651px) 100vw, 651px" data-recalc-dims="1" />
</p>

  * 화면 하단 “**LDAP 로그인 테스트**” 에서 사용자 이름, 암호를 입력 후 “**테스트**” 클릭 
      * 사용자 이름: sn (본인 아이디)
      * 암호: Sn (본인 아이디)

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1005" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/04/17-2.png?fit=497%2C133" alt="액세스 제어 - LDAP" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/04/17-2.png?w=497 497w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/04/17-2.png?resize=300%2C80 300w" sizes="(max-width: 497px) 100vw, 497px" data-recalc-dims="1" />
</p>

  * 정상적으로 LDAP 설정이 되었으면 아래와 같은 메시지가 나온다.

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1006" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/04/18-2.png?fit=273%2C114" alt="액세스 제어 - LDAP" data-recalc-dims="1" />
</p>

  * **보안** &#8211; **액세스 제어**, 로그인 및 권한 정책의 “**응용프로그램 복사**” 항목을 아래와 같이 설정한다, 화면 제일 하단의 “**적용**” 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1007" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/04/19-2.png?fit=1104%2C270" alt="액세스 제어 - LDAP" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/04/19-2.png?w=1104 1104w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/04/19-2.png?resize=300%2C73 300w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/04/19-2.png?resize=768%2C188 768w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/04/19-2.png?resize=1024%2C250 1024w" sizes="(max-width: 1000px) 100vw, 1000px" data-recalc-dims="1" />
</p>

## 복합기 테스트

  * 복합기 홈화면에서 &#8220;**복사**&#8221; 선택

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-991" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/04/copy_menu.png?fit=298%2C115" alt="copy_menu" data-recalc-dims="1" />
</p>

  * 사용자 이름, 암호 입력 (예) s1, S1

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1009" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/04/21-3.png?fit=800%2C600" alt="액세스 제어 - LDAP" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/04/21-3.png?w=800 800w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/04/21-3.png?resize=300%2C225 300w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/04/21-3.png?resize=768%2C576 768w" sizes="(max-width: 800px) 100vw, 800px" data-recalc-dims="1" />
</p>

  * 로그인이 정상적으로 되었는지 확인한다.

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1010" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/04/22-1.png?fit=800%2C600" alt="액세스 제어 - LDAP" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/04/22-1.png?w=800 800w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/04/22-1.png?resize=300%2C225 300w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/04/22-1.png?resize=768%2C576 768w" sizes="(max-width: 800px) 100vw, 800px" data-recalc-dims="1" />
</p>

  * 다른 계정으로 테스트해 본다.