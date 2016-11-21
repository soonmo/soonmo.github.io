---
id: 1398
title: Microsoft Point and Print
date: 2016-05-06T23:30:29+00:00
author: 홍 순모
layout: page
guid: http://hpidemo.net/?page_id=1398
---
Microsoft Point and Print 의 작동 원리를 실습을 통해서 실제 경험한다.

  * 이전 실습에서 설치했던 프린터 드라이버를 삭제한다.
  * 윈도우키 + R, **\\dc\mfp1** 입력 후 “**확인**” 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1405" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/2-11.png?fit=441%2C203" alt="MS Point and Print 2" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/2-11.png?w=441 441w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/2-11.png?resize=300%2C138 300w" sizes="(max-width: 441px) 100vw, 441px" data-recalc-dims="1" />
</p>

  * 잠시 기다리면 서버와 연결되면서 프린터가 자동으로 설치됨 – 이것이 **Microsoft Point and Print** 기술임
  * **시작** > **장치 및 프린터**, dc의 mfp1 마우스 포인터 위치시킨 후 마우스 오른쪽 버튼 클릭 후 “**인쇄 기본 설정**” 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1406" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/3-9.png?fit=304%2C299" alt="MS Point and Print 3" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/3-9.png?w=304 304w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/3-9.png?resize=300%2C295 300w" sizes="(max-width: 304px) 100vw, 304px" data-recalc-dims="1" />
</p>

  * “**완료**” 탭 클릭, “**양면 인쇄**” 가 기본으로 선택되어 있음

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1407" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/4-11.png?fit=631%2C582" alt="MS Point and Print 4" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/4-11.png?w=631 631w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/4-11.png?resize=300%2C277 300w" sizes="(max-width: 631px) 100vw, 631px" data-recalc-dims="1" />
</p>

  * “**양면 인쇄**” 체크 해제 후 “**적용**” 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1401" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/5-8.png?fit=631%2C582" alt="MS Point and Print 5" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/5-8.png?w=631 631w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/5-8.png?resize=300%2C277 300w" sizes="(max-width: 631px) 100vw, 631px" data-recalc-dims="1" />
</p>

  * 색상탭 클릭해 보면 “**그레이스케일로 인쇄**” 에 체크가 되어 있는데 이를 해제 후 “**확인**” 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1402" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/6-8.png?fit=631%2C582" alt="MS Point and Print 6" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/6-8.png?w=631 631w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/6-8.png?resize=300%2C277 300w" sizes="(max-width: 631px) 100vw, 631px" data-recalc-dims="1" />
</p>

  * 테스트용 칼라PDF 문서를 열어서 인쇄해 본다, ㈜ 문서가 바로 프린터로 전송되는 것이 아니라 프린트 서버를 거쳐서 프린터로 전송된다.

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1403" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-9.png?fit=746%2C654" alt="MS Point and Print 7" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-9.png?w=746 746w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-9.png?resize=300%2C263 300w" sizes="(max-width: 746px) 100vw, 746px" data-recalc-dims="1" />
</p>

  * 로그아웃 했다 도메인 계정으로 재로그인한다. (또는 재부팅)
  * **시작** > **장치 및 프린터**, dc의 mfp1 마우스 포인터 위치시킨 후 마우스 오른쪽 버튼 클릭 후 “**인쇄 기본 설정**” 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1404" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/10-8.png?fit=304%2C299" alt="MS Point and Print 10" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/10-8.png?w=304 304w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/10-8.png?resize=300%2C295 300w" sizes="(max-width: 304px) 100vw, 304px" data-recalc-dims="1" />
</p>

  * 완료와 색상탭에서 각각 “**양면 인쇄**”, “**그레이스케일로 인쇄**” 설정을 확인해라.