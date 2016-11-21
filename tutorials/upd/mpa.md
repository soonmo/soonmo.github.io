---
id: 1410
title: MPA 솔루션 맛보기
date: 2016-05-06T23:53:11+00:00
author: 홍 순모
layout: page
guid: http://hpidemo.net/?page_id=1410
---
HP MPA (Managed Print Administration) 는 PARK (Printer Administration Resource Kit)에 포함된 솔루션의 하나로 사용자 별 출력 정책, 프린터 리스트 등을 제공한다. 이번 실습에서는 UPD와 MPA를 연동해서 프린터 리스트를 사용자에게 효과적으로 제공하는 MPL(Managed Print List) 이라고 부르는 기능을 체험해 본다.

  * &#8220;**명령 프롬프트**&#8221; 실행, (윈도우키 + R, cmd 입력 후 엔터)
  * UPD 설치 프로그램 폴더로 이동 (C:\HP Universal Print Driver\pcl6-x64-6.0.0.18849)

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1418" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/3-10.png?fit=677%2C442" alt="MPA 3" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/3-10.png?w=677 677w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/3-10.png?resize=300%2C196 300w" sizes="(max-width: 677px) 100vw, 677px" data-recalc-dims="1" />
</p>

  * 다음 명령어를 입력 후 “**엔터**” 
      * Install /empa /policy”172.16.10.40” /dm /h /n”LAB4”

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1419" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/4-12.png?fit=677%2C442" alt="MPA 4" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/4-12.png?w=677 677w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/4-12.png?resize=300%2C196 300w" sizes="(max-width: 677px) 100vw, 677px" data-recalc-dims="1" />
</p>

  * 명령어의 의미를 알고 싶으면 install /? 하면 옵션에 대한 설명이 나온다. 설치가 끝나 때까지 기다린다. /h 옵션을 주었기 때문에 설치 진행 상황이 나타나지 않고 백그라운드로 실행된다. 작업 표시줄에 UPD 설치 프로그램 아이콘이 있으면 아직 설치 중임을 알 수 있다.

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1412" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/6-9.png?fit=513%2C38" alt="MPA 6" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/6-9.png?w=513 513w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/6-9.png?resize=300%2C22 300w" sizes="(max-width: 513px) 100vw, 513px" data-recalc-dims="1" />
</p>

  * 설치가 완료되면 LAB4  “**프린터 속성**” 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1413" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-10.png?fit=327%2C353" alt="MPA 7" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-10.png?w=327 327w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-10.png?resize=278%2C300 278w" sizes="(max-width: 327px) 100vw, 327px" data-recalc-dims="1" />
</p>

  * **프린터 찾기** > **classroom**… 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1414" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/8-9.png?fit=690%2C477" alt="MPA 8" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/8-9.png?w=690 690w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/8-9.png?resize=300%2C207 300w" sizes="(max-width: 690px) 100vw, 690px" data-recalc-dims="1" />
</p>

  * HP MPL Printer Groups 창이 나타나면 출력을 원하는 프린터 선택 (Managed Printer List)

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1415" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/9-9.png?fit=735%2C845" alt="MPA 9" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/9-9.png?w=735 735w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/9-9.png?resize=261%2C300 261w" sizes="(max-width: 735px) 100vw, 735px" data-recalc-dims="1" />
</p>

  * “**확인**” 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1416" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/10-9.png?fit=690%2C477" alt="MPA 10" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/10-9.png?w=690 690w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/10-9.png?resize=300%2C207 300w" sizes="(max-width: 690px) 100vw, 690px" data-recalc-dims="1" />
</p>

  * “**테스트 페이지 인쇄**” 클릭, “**닫기**”, “**확인**” 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1417" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/11-7.png?fit=479%2C512" alt="MPA 11" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/11-7.png?w=479 479w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/11-7.png?resize=281%2C300 281w" sizes="(max-width: 479px) 100vw, 479px" data-recalc-dims="1" />
</p>

  * PDF 문서를 열어서 인쇄를 한다. (MPL 사용)