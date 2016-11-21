---
title: PC Send Fax 소프트웨어
layout: page
permalink: /tutorials/fs-device-ug/pc-send-fax/
---
PC Send Fax 소프트웨어는 PC 에서 전자 문서를 복합기의 아날로그 팩스를 통해서 보낼 때 사용하는 소프트웨어 입니다.

## 팩스 테스트 환경 만들기

아날로그 팩스 회선이 없기 때문에 LAN Fax 설정을 한 후 팩스 테스트를 진행하고 추후 아날로그 회선이 가능한 환경에서 본 가이드를 사용해서 직접 기능을 확인해 보세요.

  * 팩스 탭 
      * “**팩스 발신 활성화**” 체크
      * 팩스 발신 방법: “**LAN 팩스 서비스**”
      * “**LAN 팩스 설정**” 탭 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1117" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/1-2.png?fit=474%2C343" alt="PC Send Fax" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/1-2.png?w=474 474w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/1-2.png?resize=300%2C217 300w" sizes="(max-width: 474px) 100vw, 474px" data-recalc-dims="1" />
</p>

  * 다음 화면과 같이 설정 
      * 타사 LAN 팩스 제품: “**통지 기능이 없는 일반 LAN 팩스 제품**”
      * UNC 폴더 경로: \\dc\lanfax
      * Windows 도메인: ppsdemo
      * 사용자 이름: sn (본인 아이디: s1, …)
      * 암호: Sn (본인 암호: S1, …)
      * “**폴더 이용 권한 확인**” 클릭
      * 화면 제일 하단 “**적용**” 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1118" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/2-1.png?fit=662%2C420" alt="PC Send Fax" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/2-1.png?w=662 662w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/2-1.png?resize=300%2C190 300w" sizes="(max-width: 662px) 100vw, 662px" data-recalc-dims="1" />
</p>

  * 보안-액세스 제어, 로그인 및 권한 정책의 &#8220;**팩스 응용 프로그램**&#8220;을 아래와 같이 설정 후 **&#8220;적용**&#8221; 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1119" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/4-2.png?fit=1100%2C59" alt="PC Send Fax" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/4-2.png?w=1100 1100w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/4-2.png?resize=300%2C16 300w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/4-2.png?resize=768%2C41 768w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/4-2.png?resize=1024%2C55 1024w" sizes="(max-width: 1000px) 100vw, 1000px" data-recalc-dims="1" />
</p>

## 복합기 테스트

  * ADF 에 용지 적재 후 복합기 홈화면 &#8220;**팩스**&#8221; 선택

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1120" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/5-2.png?fit=370%2C144" alt="PC Send Fax" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/5-2.png?w=370 370w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/5-2.png?resize=300%2C117 300w" sizes="(max-width: 370px) 100vw, 370px" data-recalc-dims="1" />
</p>

  * 인증

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1176" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/MFP-Auth.png?fit=226%2C208" alt="MFP Auth" data-recalc-dims="1" />
</p>

  * 팩스 번호를 입력 하거나 주소록에서 이름 선택

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1121" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-2.png?fit=800%2C600" alt="PC Send Fax" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-2.png?w=800 800w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-2.png?resize=300%2C225 300w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-2.png?resize=768%2C576 768w" sizes="(max-width: 800px) 100vw, 800px" data-recalc-dims="1" />
</p>

  * 화면 상단 &#8220;**팩스 발신**&#8221; 선택

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1177" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/Send-Fax-Button.png?fit=148%2C35" alt="Send Fax Button" data-recalc-dims="1" />
</p>

  * 확인

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1122" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/8-2.png?fit=800%2C600" alt="PC Send Fax" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/8-2.png?w=800 800w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/8-2.png?resize=300%2C225 300w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/8-2.png?resize=768%2C576 768w" sizes="(max-width: 800px) 100vw, 800px" data-recalc-dims="1" />
</p>

  * “윈도우키+R” \\dc\lanfax

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1123" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/9-3.png?fit=711%2C172" alt="PC Send Fax" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/9-3.png?w=711 711w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/9-3.png?resize=300%2C73 300w" sizes="(max-width: 711px) 100vw, 711px" data-recalc-dims="1" />
</p>

  * TIFF 이미지 파일, hpf 파일 한쌍이 있다. 
      * TIFF 이미지 열어서 확인
      * 메모장으로 hpf 파일 열어서 내용 확인

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1124" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/10-2.png?fit=518%2C376" alt="PC Send Fax" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/10-2.png?w=518 518w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/10-2.png?resize=300%2C218 300w" sizes="(max-width: 518px) 100vw, 518px" data-recalc-dims="1" />
</p>

## PC Send Fax 소프트웨어 설치

  * \\dc\lab_sw “PC-Send-Fax-Driver” 폴더

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1125" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/11-2.png?fit=692%2C341" alt="PC Send Fax" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/11-2.png?w=692 692w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/11-2.png?resize=300%2C148 300w" sizes="(max-width: 692px) 100vw, 692px" data-recalc-dims="1" />
</p>

  * “HP\_MFP\_SendFax300_64bit” 더블 클릭 후 압푹 해제한다

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1126" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/12-2.png?fit=559%2C187" alt="PC Send Fax" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/12-2.png?w=559 559w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/12-2.png?resize=300%2C100 300w" sizes="(max-width: 559px) 100vw, 559px" data-recalc-dims="1" />
</p>

  * 시작 – 장치 및 프린터, 프린터 추가
  * 로컬 프린터 추가

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1127" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/14-1.png?fit=628%2C460" alt="PC Send Fax" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/14-1.png?w=628 628w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/14-1.png?resize=300%2C220 300w" sizes="(max-width: 628px) 100vw, 628px" data-recalc-dims="1" />
</p>

  * 새포트 만들기, “Standard TCP/IP port”

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1128" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/15-2.png?fit=628%2C460" alt="PC Send Fax" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/15-2.png?w=628 628w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/15-2.png?resize=300%2C220 300w" sizes="(max-width: 628px) 100vw, 628px" data-recalc-dims="1" />
</p>

  * 본인의 프린터 IP 주소 입력 (예) 172.16.10.151

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1106" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/16-2.png?fit=628%2C460" alt="PC Send Fax" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/16-2.png?w=628 628w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/16-2.png?resize=300%2C220 300w" sizes="(max-width: 628px) 100vw, 628px" data-recalc-dims="1" />
</p>

  * 디스크 있음

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1107" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/17-2.png?fit=628%2C460" alt="PC Send Fax" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/17-2.png?w=628 628w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/17-2.png?resize=300%2C220 300w" sizes="(max-width: 628px) 100vw, 628px" data-recalc-dims="1" />
</p>

  * 찾아보기 “c:\HP PC Send Fax 64bit Driver”

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1108" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/18-2.png?fit=664%2C394" alt="PC Send Fax" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/18-2.png?w=664 664w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/18-2.png?resize=300%2C178 300w" sizes="(max-width: 664px) 100vw, 664px" data-recalc-dims="1" />
</p>

  * 다음

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1109" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/19-2.png?fit=628%2C460" alt="PC Send Fax" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/19-2.png?w=628 628w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/19-2.png?resize=300%2C220 300w" sizes="(max-width: 628px) 100vw, 628px" data-recalc-dims="1" />
</p>

  * 다음

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1110" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/20-2.png?fit=628%2C460" alt="PC Send Fax" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/20-2.png?w=628 628w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/20-2.png?resize=300%2C220 300w" sizes="(max-width: 628px) 100vw, 628px" data-recalc-dims="1" />
</p>

  * &#8220;**공유안함**&#8220;, 다음

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1111" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/21-2.png?fit=628%2C460" alt="PC Send Fax" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/21-2.png?w=628 628w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/21-2.png?resize=300%2C220 300w" sizes="(max-width: 628px) 100vw, 628px" data-recalc-dims="1" />
</p>

  * 테스트 페이지 인쇄

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1112" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/22-3.png?fit=628%2C460" alt="PC Send Fax" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/22-3.png?w=628 628w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/22-3.png?resize=300%2C220 300w" sizes="(max-width: 628px) 100vw, 628px" data-recalc-dims="1" />
</p>

  * LAN Fax 구성으로는 지원이 안된다는 경고 메시지…, 무시하고 &#8220;**확인**&#8220;

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1113" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/23-2.png?fit=497%2C199" alt="PC Send Fax" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/23-2.png?w=497 497w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/23-2.png?resize=300%2C120 300w" sizes="(max-width: 497px) 100vw, 497px" data-recalc-dims="1" />
</p>

  * 설정 탭 
      * 발신자 이름: 홍길동
      * 팩스번호: 02-2199-1111
      * 회사이름: hp
      * 음성전화번호: 02-2199-2222
      * 미리보기 체크

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1114" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/24-2.png?fit=631%2C582" alt="PC Send Fax" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/24-2.png?w=631 631w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/24-2.png?resize=300%2C277 300w" sizes="(max-width: 631px) 100vw, 631px" data-recalc-dims="1" />
</p>

  * 팩스 작업 탭 
      * 수신자 이름: 김유신
      * 팩스 번호: 02-1234-5678
      * &#8220;**미리보기 후 전송**&#8221; 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1115" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/25-2.png?fit=631%2C582" alt="PC Send Fax" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/25-2.png?w=631 631w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/25-2.png?resize=300%2C277 300w" sizes="(max-width: 631px) 100vw, 631px" data-recalc-dims="1" />
</p>

  * 미리보기 화면을 본 후 &#8220;**팩스 취소**&#8221; 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1116" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/26-2.png?fit=1164%2C940" alt="PC Send Fax" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/26-2.png?w=1164 1164w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/26-2.png?resize=300%2C242 300w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/26-2.png?resize=768%2C620 768w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/26-2.png?resize=1024%2C827 1024w" sizes="(max-width: 1000px) 100vw, 1000px" data-recalc-dims="1" />
</p>