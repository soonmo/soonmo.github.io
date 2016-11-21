---
id: 1441
title: 드라이버 사전 구성
date: 2016-05-07T08:58:40+00:00
author: 홍 순모
layout: page
guid: http://hpidemo.net/?page_id=1441
---
친환경을 위해서 불필요한 칼라 출력을 줄이기 위해서 프린터 드라이버 기본 설정을 그레이스케일로 인쇄로 변경하고 싶다면 **PARK (Printer Administration Resource Kit)** 에 **Driver Configuration Utility**  솔루션으로 구현할 수 있다. 이번 실습에서는 드라이버 구성 유틸리티를 가지고 다양한 사전 구성을 연습해 본다.

  * 윈도우 + R, \\dc\lab_sw “확인” 클릭 후 UPD 폴더 안에 “**park-v1.7.8.zip**” 파일을 본인의 PC 바탕화면으로 복사 후 압축을 해제한다.

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1534" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/1-8.png?fit=912%2C557" alt="DCU 1" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/1-8.png?w=912 912w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/1-8.png?resize=300%2C183 300w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/1-8.png?resize=768%2C469 768w" sizes="(max-width: 912px) 100vw, 912px" data-recalc-dims="1" />
</p>

  * “**driver configuration utility**”폴더로 이동

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1535" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/2-22.png?fit=913%2C556" alt="DCU 2" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/2-22.png?w=913 913w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/2-22.png?resize=300%2C183 300w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/2-22.png?resize=768%2C468 768w" sizes="(max-width: 913px) 100vw, 913px" data-recalc-dims="1" />
</p>

  * “**hpbcfgap**” 더블 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1536" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/3-16.png?fit=914%2C289" alt="DCU 3" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/3-16.png?w=914 914w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/3-16.png?resize=300%2C95 300w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/3-16.png?resize=768%2C243 768w" sizes="(max-width: 914px) 100vw, 914px" data-recalc-dims="1" />
</p>

  * “**앞으로 이 경고를 표시하지 않음**” 체크 후 “**확인**” 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1537" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/4-21.png?fit=449%2C285" alt="DCU 4" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/4-21.png?w=449 449w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/4-21.png?resize=300%2C190 300w" sizes="(max-width: 449px) 100vw, 449px" data-recalc-dims="1" />
</p>

  * **파일** – **열기**, **C:\HP Universal Print Driver\pcl6-x64-6.0.0.18849** 로 이동
  * “hpcpu175.cfg” 파일 선택 후 “**열기**” 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1538" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/6-14.png?fit=833%2C540" alt="DCU 6" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/6-14.png?w=833 833w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/6-14.png?resize=300%2C194 300w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/6-14.png?resize=768%2C498 768w" sizes="(max-width: 833px) 100vw, 833px" data-recalc-dims="1" />
</p>

  * **양면 인쇄**: **참**, **용지 크기**: **A4**

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1539" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-14.png?fit=732%2C510" alt="DCU 7" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-14.png?w=732 732w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-14.png?resize=300%2C209 300w" sizes="(max-width: 732px) 100vw, 732px" data-recalc-dims="1" />
</p>

  * 파일 – 다른 이름으로 저장, 파일 이름: **Duplex.cfm** 입력 후 “**저장**” 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1540" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/8-12.png?fit=833%2C540" alt="DCU 8" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/8-12.png?w=833 833w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/8-12.png?resize=300%2C194 300w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/8-12.png?resize=768%2C498 768w" sizes="(max-width: 833px) 100vw, 833px" data-recalc-dims="1" />
</p>

  * **양면 인쇄**: **참**, **잠금**에 체크, **용지 크기**: **A4**

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1520" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/9-12.png?fit=732%2C510" alt="DCU 9" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/9-12.png?w=732 732w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/9-12.png?resize=300%2C209 300w" sizes="(max-width: 732px) 100vw, 732px" data-recalc-dims="1" />
</p>

  * 파일 – 다른 이름으로 저장, 파일 이름: **Duplex_lock.cfm** 입력 후 “**저장**” 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1521" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/10-10.png?fit=833%2C540" alt="DCU 10" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/10-10.png?w=833 833w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/10-10.png?resize=300%2C194 300w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/10-10.png?resize=768%2C498 768w" sizes="(max-width: 833px) 100vw, 833px" data-recalc-dims="1" />
</p>

  * “**제조시 기본값으로 돌리기**” 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1522" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/11-9.png?fit=732%2C510" alt="DCU 11" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/11-9.png?w=732 732w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/11-9.png?resize=300%2C209 300w" sizes="(max-width: 732px) 100vw, 732px" data-recalc-dims="1" />
</p>

  * “**그레이스케일로 인쇄**”: 사용 설정, **용지 크기**:  **A4**

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1523" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/12-9.png?fit=732%2C510" alt="DCU 12" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/12-9.png?w=732 732w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/12-9.png?resize=300%2C209 300w" sizes="(max-width: 732px) 100vw, 732px" data-recalc-dims="1" />
</p>

  * 파일 – 다른 이름으로 저장, 파일 이름: **Grayscale.cfm** 입력 후 “**저장**”  클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1524" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/13-7.png?fit=833%2C540" alt="DCU 13" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/13-7.png?w=833 833w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/13-7.png?resize=300%2C194 300w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/13-7.png?resize=768%2C498 768w" sizes="(max-width: 833px) 100vw, 833px" data-recalc-dims="1" />
</p>

  * **그레이스케일로** 인쇄: **사용 설정**, **잠금** 체크, 용지 크기: **A4**

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1525" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/14-5.png?fit=732%2C510" alt="DCU 14" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/14-5.png?w=732 732w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/14-5.png?resize=300%2C209 300w" sizes="(max-width: 732px) 100vw, 732px" data-recalc-dims="1" />
</p>

  * 파일 – 다른 이름으로 저장, 파일 이름: **Grayscale_lock.cfm** 입력 후 “**저장**” 클릭
  * 구성 편집기 창 닫음
  * 명령 프롬프트 실행, C:\HP Universal Print Driver\pcl6-x64-6.0.0.18849 로 이동

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1526" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/17-9.png?fit=677%2C442" alt="DCU 17" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/17-9.png?w=677 677w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/17-9.png?resize=300%2C196 300w" sizes="(max-width: 677px) 100vw, 677px" data-recalc-dims="1" />
</p>

  * **Install /gcfm”Duplex.cfm” /n”Duplex” /sm172.16.10.15n /h /q (엔터)**

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1527" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/18-8.png?fit=677%2C314" alt="DCU 18" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/18-8.png?w=677 677w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/18-8.png?resize=300%2C139 300w" sizes="(max-width: 677px) 100vw, 677px" data-recalc-dims="1" />
</p>

  * “**예**” 클릭 후 기다린다. (백그라운드로 드라이버가 설치 됨)
  * **시작 > 장치 및 프린터**, Duplex 마우스 오른쪽 클릭, **인쇄 기본 설정 > Duplex 클릭**

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1528" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/19-8.png?fit=420%2C399" alt="DCU 19" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/19-8.png?w=420 420w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/19-8.png?resize=300%2C285 300w" sizes="(max-width: 420px) 100vw, 420px" data-recalc-dims="1" />
</p>

  * “**완료**” 탭 클릭, ㈜ 양면 인쇄가 디폴트로 사전 구성 됨

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1529" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/20-5.png?fit=631%2C582" alt="DCU 20" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/20-5.png?w=631 631w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/20-5.png?resize=300%2C277 300w" sizes="(max-width: 631px) 100vw, 631px" data-recalc-dims="1" />
</p>

  * 명령 프롬프트 에서 차례로 다음 명령을 수행한다. 각 명령 후 드라이버가 설치가 끝나면 다름 명령을 수행 
      * **Install /gcfm”Duplex\_lock.cfm” /n”Duplex\_lock” /sm172.16.10.15n /h /q (엔터)**
      * **Install /gcfm”Grayscale.cfm” /n”Grayscale” /sm172.16.10.15n /h /q (엔터)**
      * **Install /gcfm”Grayscale\_lock.cfm” /n”Grayscale\_lock” /sm172.16.10.15n /h /q (엔터)**
  * 새로 설치된 드라이버의 인쇄 기본 설정값을 확인한다.

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1530" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/22-1-1.png?fit=631%2C582" alt="DCU 22-1" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/22-1-1.png?w=631 631w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/22-1-1.png?resize=300%2C277 300w" sizes="(max-width: 631px) 100vw, 631px" data-recalc-dims="1" />
</p>

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1531" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/22-2-1.png?fit=631%2C582" alt="DCU 22-2" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/22-2-1.png?w=631 631w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/22-2-1.png?resize=300%2C277 300w" sizes="(max-width: 631px) 100vw, 631px" data-recalc-dims="1" />
</p>

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1532" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/22-3-1.png?fit=631%2C582" alt="DCU 22-3" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/22-3-1.png?w=631 631w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/22-3-1.png?resize=300%2C277 300w" sizes="(max-width: 631px) 100vw, 631px" data-recalc-dims="1" />
</p>

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1533" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/22-4-1.png?fit=631%2C582" alt="DCU 22-4" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/22-4-1.png?w=631 631w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/22-4-1.png?resize=300%2C277 300w" sizes="(max-width: 631px) 100vw, 631px" data-recalc-dims="1" />
</p>