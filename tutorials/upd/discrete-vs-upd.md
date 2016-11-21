---
id: 1329
title: 모델 드라이버, UPD 설치 및 비교
date: 2016-05-03T13:52:37+00:00
author: 홍 순모
layout: page
guid: http://hpidemo.net/?page_id=1329
---
<div id="toc_container" class="no_bullets">
  <p class="toc_title">
    목차
  </p>
  
  <ul class="toc_list">
    <li>
      <a href="#i"><span class="toc_number toc_depth_1">1</span> 기존에 설치되어 있는 프린트 드라이버 삭제</a>
    </li>
    <li>
      <a href="#i-2"><span class="toc_number toc_depth_1">2</span> 모델 드라이버 설치</a>
    </li>
    <li>
      <a href="#UPD"><span class="toc_number toc_depth_1">3</span> UPD 설치</a>
    </li>
    <li>
      <a href="#_UPD"><span class="toc_number toc_depth_1">4</span> 모델 드라이버와 UPD 비교</a>
    </li>
  </ul>
</div>

이번 실습에서는 모델 드라이버 (모델 별 전용)와 UPD (Universal Print Driver)를 각각 설치해 보고 차이점을 비교해 본다.

## <span id="i">기존에 설치되어 있는 프린트 드라이버 삭제</span>

  * 도메인 사용자 (ppsdemo\s**n**) 계정으로 로그-인
  * 윈도우키 + R, **printmanagement.ms**c 입력 후 “엔터” 키를 누른다.
  * **인쇄 서버 > 컴퓨터이름 (로컬) > 프린터** 클릭, 삭제하고자 하는 프린터 이름 위에 마우스 포인터를 위치 시킨 후 마우스 오른쪽 버튼 클릭 – **삭제** 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1358" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/2-9.png?fit=842%2C572" alt="model vs upd 2" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/2-9.png?w=842 842w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/2-9.png?resize=300%2C204 300w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/2-9.png?resize=768%2C522 768w" sizes="(max-width: 842px) 100vw, 842px" data-recalc-dims="1" />
</p>

  * “**예**” 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1359" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/3-7.png?fit=490%2C171" alt="model vs upd 3" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/3-7.png?w=490 490w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/3-7.png?resize=300%2C105 300w" sizes="(max-width: 490px) 100vw, 490px" data-recalc-dims="1" />
</p>

  * HP Universal Printing PCL 6 프린터도 같은 방법으로 삭제 (있으면)
  * **인쇄서버 > 컴퓨터이름(로컬) > 드라이버** 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1363" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/printmanagement-01.png?fit=844%2C573" alt="printmanagement-01" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/printmanagement-01.png?w=844 844w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/printmanagement-01.png?resize=300%2C204 300w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/printmanagement-01.png?resize=768%2C521 768w" sizes="(max-width: 844px) 100vw, 844px" data-recalc-dims="1" />
</p>

  * 지우고자 하는 드라이버에 마우스 포인터를 위치시킨 후 마우스 오른쪽 버튼 클릭, “**드라이버** **패키지** **제거**” 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1362" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/printmanagement-02.png?fit=841%2C331" alt="printmanagement-02" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/printmanagement-02.png?w=841 841w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/printmanagement-02.png?resize=300%2C118 300w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/printmanagement-02.png?resize=768%2C302 768w" sizes="(max-width: 841px) 100vw, 841px" data-recalc-dims="1" />
</p>

## <span id="i-2">모델 드라이버 설치</span>

  * \\dc\lab_sw 열고 “drivers” 폴더 안에 본인의 복합기 기종에 맞는 드라이버를 바탕화면으로 복사한다. (또는 http://www.hp.com 에서 드라이버를 다운로드 받는다.)
  * 드라이버 파일을 더블 클릭 후 압축 해제하는 창이 뜨면 “**예**”를 클릭, ㈜ 드라이버 파일이 저장되는 경로를 기억해 둔다.

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1360" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/5-7.png?fit=381%2C161" alt="model vs upd 5" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/5-7.png?w=381 381w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/5-7.png?resize=300%2C127 300w" sizes="(max-width: 381px) 100vw, 381px" data-recalc-dims="1" />
</p>

  * 시작 – 장치 및 프린터 클릭, “**프린터 추가**” 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1361" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/add-printer.png?fit=548%2C139" alt="add printer" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/add-printer.png?w=548 548w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/add-printer.png?resize=300%2C76 300w" sizes="(max-width: 548px) 100vw, 548px" data-recalc-dims="1" />
</p>

  * “**로컬 프린터 추가**” 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1332" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/6-6.png?fit=628%2C460" alt="model vs upd 6" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/6-6.png?w=628 628w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/6-6.png?resize=300%2C220 300w" sizes="(max-width: 628px) 100vw, 628px" data-recalc-dims="1" />
</p>

  * **새 포트 만들기**, 포트 종류 “**Standard TCP/IP Port**” 선택 후 “**다음**” 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1333" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-7.png?fit=628%2C460" alt="model vs upd 7" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-7.png?w=628 628w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-7.png?resize=300%2C220 300w" sizes="(max-width: 628px) 100vw, 628px" data-recalc-dims="1" />
</p>

  * IP 주소에 본인의 복합기 IP 주소 입력 (예, 172.16.10.15n), “**프린터를 검색하고 사용할 드라이버를 자동으로 선택**” 앞에 체크 **해제** 후 “**다음**” 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1334" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/8-7.png?fit=628%2C460" alt="model vs upd 8" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/8-7.png?w=628 628w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/8-7.png?resize=300%2C220 300w" sizes="(max-width: 628px) 100vw, 628px" data-recalc-dims="1" />
</p>

  * “**디스크 있음**” 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1335" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/9-7.png?fit=628%2C460" alt="model vs upd 9" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/9-7.png?w=628 628w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/9-7.png?resize=300%2C220 300w" sizes="(max-width: 628px) 100vw, 628px" data-recalc-dims="1" />
</p>

  * “**찾아 보기**” 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1336" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/10-6.png?fit=509%2C219" alt="model vs upd 10" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/10-6.png?w=509 509w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/10-6.png?resize=300%2C129 300w" sizes="(max-width: 509px) 100vw, 509px" data-recalc-dims="1" />
</p>

  * 드라이버 경로 선택 후 “**열기**” – “**확인**” 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1337" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/11-5.png?fit=664%2C394" alt="model vs upd 11" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/11-5.png?w=664 664w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/11-5.png?resize=300%2C178 300w" sizes="(max-width: 664px) 100vw, 664px" data-recalc-dims="1" />
</p>

  * 모델이 여러 개 나오면 본인 복합기 모델을 선택 후 “**다음**” 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1338" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/12-6.png?fit=628%2C460" alt="model vs upd 12" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/12-6.png?w=628 628w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/12-6.png?resize=300%2C220 300w" sizes="(max-width: 628px) 100vw, 628px" data-recalc-dims="1" />
</p>

  * “**다음**” 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1339" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/13-4.png?fit=628%2C460" alt="model vs upd 13" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/13-4.png?w=628 628w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/13-4.png?resize=300%2C220 300w" sizes="(max-width: 628px) 100vw, 628px" data-recalc-dims="1" />
</p>

  * 드라이버 설치 진행

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1340" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/14-4.png?fit=628%2C460" alt="model vs upd 14" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/14-4.png?w=628 628w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/14-4.png?resize=300%2C220 300w" sizes="(max-width: 628px) 100vw, 628px" data-recalc-dims="1" />
</p>

  * “**공유 안 함**” 선택 후 “**다음**” 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1341" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/15-4.png?fit=628%2C460" alt="model vs upd 15" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/15-4.png?w=628 628w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/15-4.png?resize=300%2C220 300w" sizes="(max-width: 628px) 100vw, 628px" data-recalc-dims="1" />
</p>

  * “**테스트 페이지**” 인쇄 클릭, “**마침**” 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1342" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/16-5.png?fit=628%2C460" alt="model vs upd 16" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/16-5.png?w=628 628w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/16-5.png?resize=300%2C220 300w" sizes="(max-width: 628px) 100vw, 628px" data-recalc-dims="1" />
</p>

## <span id="UPD">UPD 설치</span>

  * \\dc\lab_sw 열고 “UPD” 폴더 안에 “upd-pcl6-x64-6.0.0.18849.exe” 파일을 바탕화면으로 복사한다. (또는 http://www.hp.com/go/upd 에서 다운로드 받는다.)
  * 바탕화면의 upd 설치 파일 더블 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1343" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/17-6.png?fit=76%2C104" alt="model vs upd 17" data-recalc-dims="1" />
</p>

  * “**Unzip**” 클릭, ㈜ 압축 파일이 해제되어 복사되는 폴더를 잘 기억해 둔다.

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1344" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/18-5.png?fit=351%2C218" alt="model vs upd 18" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/18-5.png?w=351 351w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/18-5.png?resize=300%2C186 300w" sizes="(max-width: 351px) 100vw, 351px" data-recalc-dims="1" />
</p>

  * “**확인**” 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1345" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/19-5.png?fit=225%2C144" alt="model vs upd 19" data-recalc-dims="1" />
</p>

  * 사용자 계정 콘트롤 창이 뜨면 “**예**” 클릭
  * “**예**” 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1346" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/21-4.png?fit=525%2C403" alt="model vs upd 21" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/21-4.png?w=525 525w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/21-4.png?resize=300%2C230 300w" sizes="(max-width: 525px) 100vw, 525px" data-recalc-dims="1" />
</p>

  * “**일반 모드**” 선택 후 “**다음**” 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1347" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/22-6.png?fit=525%2C399" alt="model vs upd 22" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/22-6.png?w=525 525w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/22-6.png?resize=300%2C228 300w" sizes="(max-width: 525px) 100vw, 525px" data-recalc-dims="1" />
</p>

  * “**로컬 프린터 추가**” 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1348" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/23-5.png?fit=618%2C450" alt="model vs upd 23" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/23-5.png?w=618 618w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/23-5.png?resize=300%2C218 300w" sizes="(max-width: 618px) 100vw, 618px" data-recalc-dims="1" />
</p>

  * “**기존 포트 사용**” 선택 후 모델 드라이버 설치 때 만들 었던 포트 선택 후 “**다음**” 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1349" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/24-5.png?fit=618%2C450" alt="model vs upd 24" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/24-5.png?w=618 618w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/24-5.png?resize=300%2C218 300w" sizes="(max-width: 618px) 100vw, 618px" data-recalc-dims="1" />
</p>

  * “HP Universal Printing PCL 6 (6.0.0)” 선택 후 “다음” 클릭; **(질문)** “HP Universal Printing PCL 6” 와 “HP Universal Printing PCL 6 (v6.0.0)” 의 차이점은?

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1350" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/25-4.png?fit=618%2C450" alt="model vs upd 25" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/25-4.png?w=618 618w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/25-4.png?resize=300%2C218 300w" sizes="(max-width: 618px) 100vw, 618px" data-recalc-dims="1" />
</p>

  * “**다음**” 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1351" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/26-5.png?fit=618%2C450" alt="model vs upd 26" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/26-5.png?w=618 618w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/26-5.png?resize=300%2C218 300w" sizes="(max-width: 618px) 100vw, 618px" data-recalc-dims="1" />
</p>

  * 드라이버가 설치될 때 까지 기다린다.
  * “**공유 안 함**” 선택 후 “**다음**” 클릭
  * “**테스트 페이지 인쇄**” 클릭, 테스트 페이지가 출력되면 “**닫기**” 클릭
  * 아래와 같은 화면이 나오면 기다린다.

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1352" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/30-2.png?fit=525%2C408" alt="model vs upd 30" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/30-2.png?w=525 525w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/30-2.png?resize=300%2C233 300w" sizes="(max-width: 525px) 100vw, 525px" data-recalc-dims="1" />
</p>

  * “**마침**” 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1353" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/31-2.png?fit=525%2C408" alt="model vs upd 31" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/31-2.png?w=525 525w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/31-2.png?resize=300%2C233 300w" sizes="(max-width: 525px) 100vw, 525px" data-recalc-dims="1" />
</p>

## <span id="_UPD">모델 드라이버와 UPD 비교</span>

  * 모델 드라이버, UPD의  **프린터 속성** &#8211; **장치 설정**  탭을 각각 클릭 해서 비교해 본다.

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1354" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/32-1.png?fit=479%2C512" alt="model vs upd 32-1" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/32-1.png?w=479 479w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/32-1.png?resize=281%2C300 281w" sizes="(max-width: 479px) 100vw, 479px" data-recalc-dims="1" />
</p>

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1355" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/32-2.png?fit=479%2C512" alt="model vs upd 32-2" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/32-2.png?w=479 479w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/32-2.png?resize=281%2C300 281w" sizes="(max-width: 479px) 100vw, 479px" data-recalc-dims="1" />
</p>

  * 모델 드라이버, UPD의  **인쇄 기본 설정** &#8211; **고급**  탭을 각각 클릭 해서 비교해 본다.

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1356" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/33-1-1.png?fit=631%2C582" alt="model vs upd 33-1" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/33-1-1.png?w=631 631w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/33-1-1.png?resize=300%2C277 300w" sizes="(max-width: 631px) 100vw, 631px" data-recalc-dims="1" />
</p>

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1357" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/33-2.png?fit=631%2C582" alt="model vs upd 33-2" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/33-2.png?w=631 631w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/33-2.png?resize=300%2C277 300w" sizes="(max-width: 631px) 100vw, 631px" data-recalc-dims="1" />
</p>

  * ㈜ 모델 드라이버와 UPD 일반 모드는 사용자 입장에서 전혀 차이가 없음