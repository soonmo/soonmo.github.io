---
id: 1450
title: UPD 작업 저장 (Stored Job)
date: 2016-05-07T08:23:05+00:00
author: 홍 순모
layout: page
guid: http://hpidemo.net/?page_id=1450
---
<div id="toc_container" class="no_bullets">
  <p class="toc_title">
    목차
  </p>
  
  <ul class="toc_list">
    <li>
      <a href="#i"><span class="toc_number toc_depth_1">1</span> 실습용 큐 설치</a>
    </li>
    <li>
      <a href="#1A_StoredJob-PINtoPRINT-DefaultPIN-1234"><span class="toc_number toc_depth_1">2</span> 1A – StoredJob-PINtoPRINT-DefaultPIN-1234</a>
    </li>
    <li>
      <a href="#1B_StoredJob-PINtoPRINT-DefaultPIN-1234-Locked"><span class="toc_number toc_depth_1">3</span> 1B – StoredJob-PINtoPRINT-DefaultPIN-1234-Locked</a>
    </li>
    <li>
      <a href="#2A_StoredJob-PINtoPRINT-RequestPIN"><span class="toc_number toc_depth_1">4</span> 2A – StoredJob-PINtoPRINT-RequestPIN</a>
    </li>
    <li>
      <a href="#2B_StoredJob-PINtoPRINT-RequestPIN-Locked"><span class="toc_number toc_depth_1">5</span> 2B – StoredJob-PINtoPRINT-RequestPIN-Locked</a>
    </li>
    <li>
      <a href="#3A_StoredJob-EncryptJob-Automatic"><span class="toc_number toc_depth_1">6</span> 3A – StoredJob-EncryptJob-Automatic</a>
    </li>
    <li>
      <a href="#3B_StoredJob-EncryptJob-Automatic-Locked"><span class="toc_number toc_depth_1">7</span> 3B – StoredJob-EncryptJob-Automatic-Locked</a>
    </li>
    <li>
      <a href="#4A_StoredJob-EncryptJob-Disabled"><span class="toc_number toc_depth_1">8</span> 4A – StoredJob-EncryptJob-Disabled</a>
    </li>
    <li>
      <a href="#4B_StoredJob-EncryptJob-Disabled-Locked"><span class="toc_number toc_depth_1">9</span> 4B – StoredJob-EncryptJob-Disabled-Locked</a>
    </li>
  </ul>
</div>

UPD 의 보안 기능인 작업 저장 기능에 대한 실습을 한다. 작업 저장의 다양한 구성과 구성별 차이점을 명확히 이해하고 실제로 어떻게 작동하는지 실습을 통해서 확인한다.

## <span id="i">실습용 큐 설치</span>

  * 이전 실습에서 설치한 UPD 프린터를 삭제한다. (시작 > 실행 “**printmanagement.msc**”)
  * \\dc\lab_sw 공유 폴더를 열고 UPD 폴더 내 “upd-pcl6-x64-6.0.0.18849.exe” 파일을 PC 바탕화면으로 복사

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1453" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/2-13.png?fit=856%2C582" alt="UPD Stored Job 2" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/2-13.png?w=856 856w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/2-13.png?resize=300%2C204 300w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/2-13.png?resize=768%2C522 768w" sizes="(max-width: 856px) 100vw, 856px" data-recalc-dims="1" />
</p>

  * \\dc\lab_sw 공유 폴더의 **“UPD\_HP\_JOB\_STORAGE\_Lab.zip”** 파일을 PC 바탕화면으로 복사

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1454" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/2-1-1.png?fit=856%2C582" alt="UPD Stored Job 2-1" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/2-1-1.png?w=856 856w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/2-1-1.png?resize=300%2C204 300w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/2-1-1.png?resize=768%2C522 768w" sizes="(max-width: 856px) 100vw, 856px" data-recalc-dims="1" />
</p>

  * “**upd-pcl6-x64-6.0.0.18849.exe**” 파일을 더블 클릭 후 “**when don unzipping open**:…” 체크 해제 후 압축 해제

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1455" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/3-12.png?fit=351%2C218" alt="UPD Stored Job 3" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/3-12.png?w=351 351w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/3-12.png?resize=300%2C186 300w" sizes="(max-width: 351px) 100vw, 351px" data-recalc-dims="1" />
</p>

  * “**UPD\_HP\_JOB\_STORAGE\_Lab.zip**” 압축을 다음과 같이 “C:\HP Universal Print Driver” 폴더에 압축 해제

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1456" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/4-14.png?fit=824%2C346" alt="UPD Stored Job 4" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/4-14.png?w=824 824w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/4-14.png?resize=300%2C126 300w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/4-14.png?resize=768%2C322 768w" sizes="(max-width: 824px) 100vw, 824px" data-recalc-dims="1" />
</p>

  * “**install-upd-lab.bat**” 파일 마우스 포인터를 위치시킨 후 오른쪽 버튼 클릭 후 “**편집**” 선택

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1457" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/5-9.png?fit=772%2C292" alt="UPD Stored Job 5" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/5-9.png?w=772 772w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/5-9.png?resize=300%2C113 300w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/5-9.png?resize=768%2C290 768w" sizes="(max-width: 772px) 100vw, 772px" data-recalc-dims="1" />
</p>

  * 2번째 라인 수정: 본인 복합기 IP 주소로 변경

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1458" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/5-1-1.png?fit=693%2C506" alt="UPD Stored Job 5-1" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/5-1-1.png?w=693 693w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/5-1-1.png?resize=300%2C219 300w" sizes="(max-width: 693px) 100vw, 693px" data-recalc-dims="1" />
</p>

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1459" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/5-2-1.png?fit=693%2C506" alt="UPD Stored Job 5-2" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/5-2-1.png?w=693 693w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/5-2-1.png?resize=300%2C219 300w" sizes="(max-width: 693px) 100vw, 693px" data-recalc-dims="1" />
</p>

  * “**파일**” – “**저장**”

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1460" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/5-3-1.png?fit=694%2C505" alt="UPD Stored Job 5-3" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/5-3-1.png?w=694 694w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/5-3-1.png?resize=300%2C218 300w" sizes="(max-width: 694px) 100vw, 694px" data-recalc-dims="1" />
</p>

  * “**install-upd-lab.bat**” 파일 마우스 포인터를 위치시킨 후 오른쪽 버튼 클릭 후 “관리자 권한으로 실행” 선택

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1461" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/6-11.png?fit=759%2C290" alt="UPD Stored Job 6" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/6-11.png?w=759 759w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/6-11.png?resize=300%2C115 300w" sizes="(max-width: 759px) 100vw, 759px" data-recalc-dims="1" />
</p>

  * &#8220;**엔터**&#8220;

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1462" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-12.png?fit=677%2C442" alt="UPD Stored Job 7" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-12.png?w=677 677w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-12.png?resize=300%2C196 300w" sizes="(max-width: 677px) 100vw, 677px" data-recalc-dims="1" />
</p>

  * 스크립트가 모두 실행될 때 까지 기다린다. (상당히 오랜 시간이 걸림..1A, 1B….4B 까지 8개 대기열 생성)

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1463" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/8-11.png?fit=677%2C442" alt="UPD Stored Job 8" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/8-11.png?w=677 677w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/8-11.png?resize=300%2C196 300w" sizes="(max-width: 677px) 100vw, 677px" data-recalc-dims="1" />
</p>

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1464" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/8-1-1.png?fit=677%2C442" alt="UPD Stored Job 8-1" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/8-1-1.png?w=677 677w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/8-1-1.png?resize=300%2C196 300w" sizes="(max-width: 677px) 100vw, 677px" data-recalc-dims="1" />
</p>

  * 윈도우키 + R, “**printmanagement.msc**” (엔터), ㈜ 모두 8개의 인쇄 대기열이 만들어 졌다.

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1465" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/9-11.png?fit=595%2C181" alt="UPD Stored Job 9" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/9-11.png?w=595 595w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/9-11.png?resize=300%2C91 300w" sizes="(max-width: 595px) 100vw, 595px" data-recalc-dims="1" />
</p>

## <span id="1A_StoredJob-PINtoPRINT-DefaultPIN-1234">1A – StoredJob-PINtoPRINT-DefaultPIN-1234</span>

  * **드라이버 사전 구성 유틸리티** 실행
  * 파일 &#8211; 열기,  “**C:\HP Universal Print Driver\UPD_CFM\1A-StoredJob-PINtoPRINT-DefaultPIN-1234.cfm**” 
      * 작업 저장 모드를 확장해서 설정 상태 확인
      * ㈜ 기본 PIN 을 설정하지 않으면 “0000” 으로 설정 됨

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1481" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/2-14.png?fit=246%2C87" alt="Stored Job 1A 2" data-recalc-dims="1" />
</p>

  * 마우스 오른쪽 클릭 > **인쇄 기본값 설정**

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1469" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/3-13.png?fit=721%2C217" alt="Stored Job 1A 3" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/3-13.png?w=721 721w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/3-13.png?resize=300%2C90 300w" sizes="(max-width: 721px) 100vw, 721px" data-recalc-dims="1" />
</p>

  * “**작업 저장**” 탭 클릭 해서 드라이버 설정을 확인

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1470" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/4-15.png?fit=631%2C582" alt="Stored Job 1A 4" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/4-15.png?w=631 631w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/4-15.png?resize=300%2C277 300w" sizes="(max-width: 631px) 100vw, 631px" data-recalc-dims="1" />
</p>

  * 테스트 페이지 인쇄

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1471" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/5-10.png?fit=717%2C266" alt="Stored Job 1A 5" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/5-10.png?w=717 717w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/5-10.png?resize=300%2C111 300w" sizes="(max-width: 717px) 100vw, 717px" data-recalc-dims="1" />
</p>

  * 프린터에 사용자 계정으로 폴더가 생성되고 그 안에 인쇄 작업이 저장됨

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1472" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/6-12.png?fit=316%2C249" alt="Stored Job 1A 6" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/6-12.png?w=316 316w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/6-12.png?resize=300%2C236 300w" sizes="(max-width: 316px) 100vw, 316px" data-recalc-dims="1" />
</p>

  * 프린터(복합기)로 이동
  * “**장치 메모리에서 불러 오기**” 선택

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1473" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-1-2.png?fit=437%2C82" alt="Stored Job 1A 7-1" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-1-2.png?w=437 437w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-1-2.png?resize=300%2C56 300w" sizes="(max-width: 437px) 100vw, 437px" data-recalc-dims="1" />
</p>

  * 사용자명 폴더 터치 (예; Sn)

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1474" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-2-2.png?fit=480%2C272" alt="Stored Job 1A 7-2" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-2-2.png?w=480 480w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-2-2.png?resize=300%2C170 300w" sizes="(max-width: 480px) 100vw, 480px" data-recalc-dims="1" />
</p>

  * 문서 선택 (테스트 페이지)

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1475" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-3-1.png?fit=480%2C272" alt="Stored Job 1A 7-3" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-3-1.png?w=480 480w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-3-1.png?resize=300%2C170 300w" sizes="(max-width: 480px) 100vw, 480px" data-recalc-dims="1" />
</p>

  * PIN 입력 화면이 나오면 PIN 입력 (1234)

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1476" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-4-1.png?fit=480%2C272" alt="Stored Job 1A 7-4" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-4-1.png?w=480 480w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-4-1.png?resize=300%2C170 300w" sizes="(max-width: 480px) 100vw, 480px" data-recalc-dims="1" />
</p>

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1477" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-5-1.png?fit=480%2C272" alt="Stored Job 1A 7-5" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-5-1.png?w=480 480w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-5-1.png?resize=300%2C170 300w" sizes="(max-width: 480px) 100vw, 480px" data-recalc-dims="1" />
</p>

  * 상단의 “**장치 메모리에서 불러오기**” 터치하면 테스트 페이지가 인쇄된다.

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1478" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-6-1.png?fit=480%2C272" alt="Stored Job 1A 7-6" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-6-1.png?w=480 480w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-6-1.png?resize=300%2C170 300w" sizes="(max-width: 480px) 100vw, 480px" data-recalc-dims="1" />
</p>

  * “**테스트 페이지**” 선택

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1479" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-7-1.png?fit=480%2C272" alt="Stored Job 1A 7-7" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-7-1.png?w=480 480w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-7-1.png?resize=300%2C170 300w" sizes="(max-width: 480px) 100vw, 480px" data-recalc-dims="1" />
</p>

  * “**삭제**” 터치

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1480" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-8-1.png?fit=480%2C272" alt="Stored Job 1A 7-8" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-8-1.png?w=480 480w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-8-1.png?resize=300%2C170 300w" sizes="(max-width: 480px) 100vw, 480px" data-recalc-dims="1" />
</p>

  * &#8220;**확인**&#8220;

## <span id="1B_StoredJob-PINtoPRINT-DefaultPIN-1234-Locked">1B – StoredJob-PINtoPRINT-DefaultPIN-1234-Locked</span>

  * **드라이버 사전 구성 유틸리티** 실행
  * 파일 &#8211; 열기, “**C:\HP Universal Print Driver\UPD_CFM\1B-StoredJob-PINtoPRINT-DefaultPIN-1234-Lock.cfm**”

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1484" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/2-15.png?fit=301%2C75" alt="Stored Job 1B 2" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/2-15.png?w=301 301w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/2-15.png?resize=300%2C75 300w" sizes="(max-width: 301px) 100vw, 301px" data-recalc-dims="1" />
</p>

  * 마우스 오른쪽 클릭 > 인쇄 기본값 설정

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1469" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/3-13.png?fit=721%2C217" alt="Stored Job 1A 3" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/3-13.png?w=721 721w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/3-13.png?resize=300%2C90 300w" sizes="(max-width: 721px) 100vw, 721px" data-recalc-dims="1" />
</p>

  * “**작업 저장**” 탭 클릭 해서 드라이버 설정을 확인

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1483" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/4-16.png?fit=631%2C582" alt="Stored Job 1B 4" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/4-16.png?w=631 631w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/4-16.png?resize=300%2C277 300w" sizes="(max-width: 631px) 100vw, 631px" data-recalc-dims="1" />
</p>

  * “**테스트 인쇄**” 수행 (1A-StoredJob-PINtoPRINT-DefailtPIN-1234 참조)

## <span id="2A_StoredJob-PINtoPRINT-RequestPIN">2A – StoredJob-PINtoPRINT-RequestPIN</span>

  * **드라이버 사전 구성 유틸리티** 실행
  * 파일 &#8211; 열기, “**C:\HP Universal Print Driver\UPD_CFM\2A-StoredJob-PINtoPRINT-RequestPIN.cfm**”

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1488" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/2-16.png?fit=343%2C61" alt="Stored Job 1A 3 2" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/2-16.png?w=343 343w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/2-16.png?resize=300%2C53 300w" sizes="(max-width: 343px) 100vw, 343px" data-recalc-dims="1" />
</p>

  * 마우스 오른쪽 클릭 > 인쇄 기본값 설정

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1469" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/3-13.png?fit=721%2C217" alt="Stored Job 1A 3" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/3-13.png?w=721 721w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/3-13.png?resize=300%2C90 300w" sizes="(max-width: 721px) 100vw, 721px" data-recalc-dims="1" />
</p>

  * “**작업 저장**” 탭 클릭 해서 드라이버 설정을 확인

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1489" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/4-17.png?fit=631%2C582" alt="Sored Job 2A 4" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/4-17.png?w=631 631w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/4-17.png?resize=300%2C277 300w" sizes="(max-width: 631px) 100vw, 631px" data-recalc-dims="1" />
</p>

  * 테스트페이지 인쇄

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1471" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/5-10.png?fit=717%2C266" alt="Stored Job 1A 5" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/5-10.png?w=717 717w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/5-10.png?resize=300%2C111 300w" sizes="(max-width: 717px) 100vw, 717px" data-recalc-dims="1" />
</p>

  * PIN을 요구함, PIN 입력

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1486" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/6-1-2.png?fit=274%2C196" alt="Stored Job 1A 3 6-1" data-recalc-dims="1" />
</p>

  * &#8220;**확인**&#8221; 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1487" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/6-2-1.png?fit=316%2C249" alt="Stored Job 1A 3 6-2" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/6-2-1.png?w=316 316w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/6-2-1.png?resize=300%2C236 300w" sizes="(max-width: 316px) 100vw, 316px" data-recalc-dims="1" />
</p>

  * 프린터로 이동해서 인쇄를 한다 (1A-StoredJob-PINtoPRINT-DefailtPIN-1234 참조)

## <span id="2B_StoredJob-PINtoPRINT-RequestPIN-Locked">2B – StoredJob-PINtoPRINT-RequestPIN-Locked</span>

  * **드라이버 사전 구성 유틸리티** 실행
  * 파일 &#8211; 열기, “**C:\HP Universal Print Driver\UPD_CFM\2B-StoredJob-PINtoPRINT-RequestPIN-Lock.cfm**”

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1491" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/2-17.png?fit=344%2C61" alt="Stored Job 2B 2" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/2-17.png?w=344 344w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/2-17.png?resize=300%2C53 300w" sizes="(max-width: 344px) 100vw, 344px" data-recalc-dims="1" />
</p>

  * 마유스 오른쪽 클릭 > 인쇄 기본값 설정

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1469" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/3-13.png?fit=721%2C217" alt="Stored Job 1A 3" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/3-13.png?w=721 721w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/3-13.png?resize=300%2C90 300w" sizes="(max-width: 721px) 100vw, 721px" data-recalc-dims="1" />
</p>

  * “**작업 저장**” 탭 클릭 해서 드라이버 설정을 확인

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1492" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/4-18.png?fit=631%2C582" alt="Stored Job 2B 4" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/4-18.png?w=631 631w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/4-18.png?resize=300%2C277 300w" sizes="(max-width: 631px) 100vw, 631px" data-recalc-dims="1" />
</p>

  * 테스트 페이지 인쇄
  * 프린터로 이동해서 인쇄를 한다 (1A-StoredJob-PINtoPRINT-DefailtPIN-1234 참조)

## <span id="3A_StoredJob-EncryptJob-Automatic">3A – StoredJob-EncryptJob-Automatic</span>

  * 드라이버 사전 구성 유틸리티 실행
  * 파일 &#8211; 열기, “**C:\HP Universal Print Driver\UPD_CFM\3A-StoredJob-EncryptJob-Automatic.cfm**”

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1500" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/2-18.png?fit=337%2C59" alt="Stored Job 3A 2" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/2-18.png?w=337 337w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/2-18.png?resize=300%2C53 300w" sizes="(max-width: 337px) 100vw, 337px" data-recalc-dims="1" />
</p>

  * 마우스 오른쪽 클릭 > 인쇄 기본값 설정

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1469" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/3-13.png?fit=721%2C217" alt="Stored Job 1A 3" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/3-13.png?w=721 721w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/3-13.png?resize=300%2C90 300w" sizes="(max-width: 721px) 100vw, 721px" data-recalc-dims="1" />
</p>

  * “**작업 저장**” 탭 클릭 해서 드라이버 설정을 확인

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1501" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/4-19.png?fit=631%2C582" alt="Stored Job 3A 4" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/4-19.png?w=631 631w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/4-19.png?resize=300%2C277 300w" sizes="(max-width: 631px) 100vw, 631px" data-recalc-dims="1" />
</p>

  * 테스트 페이지 인쇄
  * 암호 입력 (문자, 숫자 모두 가능)

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1495" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/6-2-2.png?fit=316%2C257" alt="Stored Job 3A 6-2" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/6-2-2.png?w=316 316w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/6-2-2.png?resize=300%2C244 300w" sizes="(max-width: 316px) 100vw, 316px" data-recalc-dims="1" />
</p>

  * ㈜ 기본 암호로 저장에 체크하면 암호가 저장됨

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1496" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/6-3-1.png?fit=316%2C257" alt="Stored Job 3A 6-3" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/6-3-1.png?w=316 316w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/6-3-1.png?resize=300%2C244 300w" sizes="(max-width: 316px) 100vw, 316px" data-recalc-dims="1" />
</p>

  * “**확인**” 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1497" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-13.png?fit=316%2C249" alt="Stored Job 3A 7" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-13.png?w=316 316w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-13.png?resize=300%2C236 300w" sizes="(max-width: 316px) 100vw, 316px" data-recalc-dims="1" />
</p>

  * 프린터(복합기)로 이동
  * “**장치 메모리에서 불러오기**” 선택

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1473" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-1-2.png?fit=437%2C82" alt="Stored Job 1A 7-1" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-1-2.png?w=437 437w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-1-2.png?resize=300%2C56 300w" sizes="(max-width: 437px) 100vw, 437px" data-recalc-dims="1" />
</p>

  * 사용자명 폴더 터치 (예; Sn)

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1474" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-2-2.png?fit=480%2C272" alt="Stored Job 1A 7-2" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-2-2.png?w=480 480w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-2-2.png?resize=300%2C170 300w" sizes="(max-width: 480px) 100vw, 480px" data-recalc-dims="1" />
</p>

  * 문서 선택 (테스트 페이지)

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1475" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-3-1.png?fit=480%2C272" alt="Stored Job 1A 7-3" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-3-1.png?w=480 480w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-3-1.png?resize=300%2C170 300w" sizes="(max-width: 480px) 100vw, 480px" data-recalc-dims="1" />
</p>

  * 암호 입력화면 이 나오면 암호를 입력한다.

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1498" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-4-2.png?fit=480%2C272" alt="Stored Job 3A 7-4" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-4-2.png?w=480 480w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-4-2.png?resize=300%2C170 300w" sizes="(max-width: 480px) 100vw, 480px" data-recalc-dims="1" />
</p>

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1499" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-5-2.png?fit=480%2C272" alt="Stored Job 3A 7-5" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-5-2.png?w=480 480w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-5-2.png?resize=300%2C170 300w" sizes="(max-width: 480px) 100vw, 480px" data-recalc-dims="1" />
</p>

  * 상단의 “**장치 메모리에서 불러오기**” 녹색 버튼 터치해서 인쇄

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1480" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-8-1.png?fit=480%2C272" alt="Stored Job 1A 7-8" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-8-1.png?w=480 480w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-8-1.png?resize=300%2C170 300w" sizes="(max-width: 480px) 100vw, 480px" data-recalc-dims="1" />
</p>

## <span id="3B_StoredJob-EncryptJob-Automatic-Locked">3B – StoredJob-EncryptJob-Automatic-Locked</span>

  * **드라이버 사전 구성 유틸리티** 실행
  * 파일 &#8211; 열기, “**C:\HP Universal Print Driver\UPD_CFM\3A-StoredJob-EncryptJob-Automatic-Locked.cfm**”

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1507" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/2-19.png?fit=344%2C59" alt="Stored Job 3B 2" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/2-19.png?w=344 344w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/2-19.png?resize=300%2C51 300w" sizes="(max-width: 344px) 100vw, 344px" data-recalc-dims="1" />
</p>

  * 마우스 오른쪽 클릭 > 인쇄 기본값 설정

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1469" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/3-13.png?fit=721%2C217" alt="Stored Job 1A 3" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/3-13.png?w=721 721w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/3-13.png?resize=300%2C90 300w" sizes="(max-width: 721px) 100vw, 721px" data-recalc-dims="1" />
</p>

  * “**작업 저장**” 탭 클릭 해서 드라이버 설정을 확인

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1505" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/4-20.png?fit=631%2C582" alt="Stored Job 3B 4" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/4-20.png?w=631 631w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/4-20.png?resize=300%2C277 300w" sizes="(max-width: 631px) 100vw, 631px" data-recalc-dims="1" />
</p>

  * 시험 인쇄 출력
  * 프린터로 이동해서 인쇄를 한다 (1A-StoredJob-PINtoPRINT-DefailtPIN-1234 참조)

## <span id="4A_StoredJob-EncryptJob-Disabled">4A – StoredJob-EncryptJob-Disabled</span>

  * **드라이버 사전 구성 유틸리티** 실행
  * 파일 &#8211; 열기, “**C:\HP Universal Print Driver\UPD_CFM\4A-EncryptJob-Disabled.cfm**”

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1511" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/2-20.png?fit=352%2C59" alt="Stored Job 4A 2" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/2-20.png?w=352 352w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/2-20.png?resize=300%2C50 300w" sizes="(max-width: 352px) 100vw, 352px" data-recalc-dims="1" />
</p>

  * 마우스 오른쪽 클릭 > 인쇄 기본값 설정

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1469" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/3-13.png?fit=721%2C217" alt="Stored Job 1A 3" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/3-13.png?w=721 721w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/3-13.png?resize=300%2C90 300w" sizes="(max-width: 721px) 100vw, 721px" data-recalc-dims="1" />
</p>

  * “**작업 저장**” 탭 클릭 해서 드라이버 설정을 확인

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1512" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/3-14.png?fit=631%2C582" alt="Stored Job 4A 3" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/3-14.png?w=631 631w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/3-14.png?resize=300%2C277 300w" sizes="(max-width: 631px) 100vw, 631px" data-recalc-dims="1" />
</p>

  * 테스트 페이지 인쇄
  * &#8220;**확인**&#8221; 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1509" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/6-13.png?fit=316%2C249" alt="Stored Job 4A 6" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/6-13.png?w=316 316w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/6-13.png?resize=300%2C236 300w" sizes="(max-width: 316px) 100vw, 316px" data-recalc-dims="1" />
</p>

  * 프린터로 이동해서 인쇄를 한다 (1A-StoredJob-PINtoPRINT-DefailtPIN-1234 참조) 
      * ㈜ PIN 이나 암호를 요구하지 않음

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1510" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-6-2.png?fit=480%2C272" alt="Stored Job 4A 7-6" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-6-2.png?w=480 480w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-6-2.png?resize=300%2C170 300w" sizes="(max-width: 480px) 100vw, 480px" data-recalc-dims="1" />
</p>

## <span id="4B_StoredJob-EncryptJob-Disabled-Locked">4B – StoredJob-EncryptJob-Disabled-Locked</span>

  * **드라이버 사전 구성 유틸리티** 실행
  * 파일 &#8211; 열기, “**C:\HP Universal Print Driver\UPD_CFM\4B-EncryptJob-Disabled-Locked.cfm**”

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1514" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/2-21.png?fit=343%2C62" alt="Stored Job 4B 2" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/2-21.png?w=343 343w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/2-21.png?resize=300%2C54 300w" sizes="(max-width: 343px) 100vw, 343px" data-recalc-dims="1" />
</p>

  * 마우스 오른쪽 클릭 > 인쇄 기본값 설정

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1469" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/3-13.png?fit=721%2C217" alt="Stored Job 1A 3" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/3-13.png?w=721 721w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/3-13.png?resize=300%2C90 300w" sizes="(max-width: 721px) 100vw, 721px" data-recalc-dims="1" />
</p>

  * “**작업 저장**” 탭 클릭 해서 드라이버 설정을 확인

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1515" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/3-15.png?fit=631%2C582" alt="Stored Job 4B 3" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/3-15.png?w=631 631w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/3-15.png?resize=300%2C277 300w" sizes="(max-width: 631px) 100vw, 631px" data-recalc-dims="1" />
</p>

  * 테스트 페이지 인쇄
  * 프린터로 이동해서 인쇄를 한다 (1A-StoredJob-PINtoPRINT-DefailtPIN-1234 참조) 
      * ㈜ PIN 이나 암호를 요구하지 않음