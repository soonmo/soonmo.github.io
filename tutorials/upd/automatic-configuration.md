---
id: 1422
title: Automatic Configuration 의 이해
date: 2016-05-07T00:40:37+00:00
author: 홍 순모
layout: page
guid: http://hpidemo.net/?page_id=1422
---
모델 드라이버, UPD 에서는 프린터 드라이버 설치시 Auto Cofiguration 이라는 기술을 통해서 장치 구성을 자동으로 한다. 특히 UPD의 경우 장치가 칼라인지 흑백인지를 드라이버 설치시 구분하는데 Auto Configuration을 사용한다. 이번 실습을 통해서 UPD에서 Auto Configuration이 어떻게 작동하는지 정확히 이해할 수 있다.

  * 바탕화면의 UPD 설치 프로그램 더블 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1424" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/2-12.png?fit=76%2C104" alt="Automatic Configuration 2" data-recalc-dims="1" />
</p>

  * Unzip 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1425" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/3-11.png?fit=351%2C218" alt="Automatic Configuration 3" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/3-11.png?w=351 351w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/3-11.png?resize=300%2C186 300w" sizes="(max-width: 351px) 100vw, 351px" data-recalc-dims="1" />
</p>

  * “**확인**” 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1426" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/4-13.png?fit=225%2C144" alt="Automatic Configuration 4" data-recalc-dims="1" />
</p>

  * 사용자 계정 콘트롤 창이 나오면 “**예**” 클릭
  * “**예**” 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1427" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/6-10.png?fit=525%2C403" alt="Automatic Configuration 6" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/6-10.png?w=525 525w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/6-10.png?resize=300%2C230 300w" sizes="(max-width: 525px) 100vw, 525px" data-recalc-dims="1" />
</p>

  * “**일반 모드**” 선택 후 “**다음**” 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1428" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-11.png?fit=525%2C399" alt="Automatic Configuration 7" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-11.png?w=525 525w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-11.png?resize=300%2C228 300w" sizes="(max-width: 525px) 100vw, 525px" data-recalc-dims="1" />
</p>

  * “**로컬 프린터 추가**” 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1429" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/8-10.png?fit=618%2C450" alt="Automatic Configuration 8" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/8-10.png?w=618 618w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/8-10.png?resize=300%2C218 300w" sizes="(max-width: 618px) 100vw, 618px" data-recalc-dims="1" />
</p>

  * “**기존 포트 사용**” 선택, 이전 LAB에서 본인의 MFP IP 주소로 생성한 포트 선택 (없으면 새포트 만들기를 선택해서 포트를 생성한다), ㈜ 실습용 복합기가 흑백 복합기이면 다른 조의 칼라 복합기의 IP주소를 확인해서 포트를 생성한다.

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1430" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/9-10.png?fit=618%2C450" alt="Automatic Configuration 9" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/9-10.png?w=618 618w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/9-10.png?resize=300%2C218 300w" sizes="(max-width: 618px) 100vw, 618px" data-recalc-dims="1" />
</p>

  * 복합기에서 LAN 케이블을 뽑니다. (연결해제)
  * HP Universal Printing PCL 6 (v6.0.0) 선택 후 “**다음**” 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1431" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/11-8.png?fit=618%2C450" alt="Automatic Configuration 11" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/11-8.png?w=618 618w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/11-8.png?resize=300%2C218 300w" sizes="(max-width: 618px) 100vw, 618px" data-recalc-dims="1" />
</p>

  * 프린터 이름 그대로 두고 “**다음**” 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1432" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/12-8.png?fit=618%2C450" alt="Automatic Configuration 12" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/12-8.png?w=618 618w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/12-8.png?resize=300%2C218 300w" sizes="(max-width: 618px) 100vw, 618px" data-recalc-dims="1" />
</p>

  * 좀 올래 걸리지만 기다린다. “**공유 안 함**” 선택 후 “**다음**” 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1433" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/13-6.png?fit=618%2C450" alt="Automatic Configuration 13" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/13-6.png?w=618 618w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/13-6.png?resize=300%2C218 300w" sizes="(max-width: 618px) 100vw, 618px" data-recalc-dims="1" />
</p>

  * 복합기에 랜케이블 다시 연결
  * “**테스트 페이지 인쇄**” 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1434" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/15-5.png?fit=618%2C450" alt="Automatic Configuration 15" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/15-5.png?w=618 618w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/15-5.png?resize=300%2C218 300w" sizes="(max-width: 618px) 100vw, 618px" data-recalc-dims="1" />
</p>

  * 테스트 페이지 확인 
      * **(질문)** 좌측상단의 Windows logo 가 칼라인가? 아니면 흑백인가?
      * **(질문)** 흑백으로 출력되었다면 이유는?
  * “**마침**” 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1435" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/16-7.png?fit=525%2C408" alt="Automatic Configuration 16" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/16-7.png?w=525 525w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/16-7.png?resize=300%2C233 300w" sizes="(max-width: 525px) 100vw, 525px" data-recalc-dims="1" />
</p>

## 문제 해결 방법

  * “**프린터 속성**” 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1437" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/18-7.png?fit=294%2C350" alt="Automatic Configuration 18" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/18-7.png?w=294 294w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/18-7.png?resize=252%2C300 252w" sizes="(max-width: 294px) 100vw, 294px" data-recalc-dims="1" />
</p>

  * “**장치 설정 탭**” 클릭, 스크롤 다운 후 “**장치 유형**” 을 “**컬러**” 로 변경 후 “**확인**” 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1438" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/19-7.png?fit=478%2C516" alt="Automatic Configuration 19" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/19-7.png?w=478 478w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/19-7.png?resize=278%2C300 278w" sizes="(max-width: 478px) 100vw, 478px" data-recalc-dims="1" />
</p>

  * 테스트 페이지 인쇄