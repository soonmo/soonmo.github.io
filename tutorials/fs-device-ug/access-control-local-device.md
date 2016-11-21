---
title: '액세스 제어 &#8211; 로컬 장치'
layout: page
permalink: /tutorials/fs-device-ug/access-control-local-device
---
<div id="toc_container" class="no_bullets">
  <p class="toc_title">
    목차
  </p>
  
  <ul class="toc_list">
    <li>
      <a href="#i"><span class="toc_number toc_depth_1">1</span> 사용자 추가</a>
    </li>
    <li>
      <a href="#i-2"><span class="toc_number toc_depth_1">2</span> 복합기 테스트</a>
    </li>
    <li>
      <a href="#i-3"><span class="toc_number toc_depth_1">3</span> 복합기 테스트</a>
    </li>
    <li>
      <a href="#i-4"><span class="toc_number toc_depth_1">4</span> 여러 사용자 한꺼번에 추가 (가져오기)</a>
    </li>
  </ul>
</div>

복합기의 각 기능 (복사, 인쇄, 디지털 전송, 팩스 등)의 무단 사용을 보호하기 위해서 각 사용자 식별 코드 (숫자 5자리 이상)를 설정해서 허가된 사용자만 사용하게 할 수 있다. 중소 규모 사무실에 적합한 보안 솔루션이다.

## <span id="i">사용자 추가</span>

  * **정보** &#8211; **작업 일지** 클릭, 사용자 항목을 기록해 둔다. (예) PPSDEMO\s1

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-988" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/04/1-3.png?fit=797%2C349" alt="액세스 제어 - 로컬장치" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/04/1-3.png?w=797 797w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/04/1-3.png?resize=300%2C131 300w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/04/1-3.png?resize=768%2C336 768w" sizes="(max-width: 797px) 100vw, 797px" data-recalc-dims="1" />
</p>

  * **보안** &#8211; **액세스 제어**
  * 스크롤 다운, “**장치 사용자 계정**”, “**새로 만들기**”… 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-989" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/04/3-4.png?fit=552%2C214" alt="액세스 제어 - 로컬장치" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/04/3-4.png?w=552 552w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/04/3-4.png?resize=300%2C116 300w" sizes="(max-width: 552px) 100vw, 552px" data-recalc-dims="1" />
</p>

  * 새 장치 사용자 계정에 본인 계정 정보를 다음과 같이 입력한다. 
      * 표시이름: Studentn (n은 학생 번호) (예) Student1
      * 전자우편 주소: <sn@ppsdemo.net> (예) s1@ppsdemo.ne
      * 네트워크 이름: PPSDEMO\sn (예) PPSDEMO\s1
      * 액세스코드: 11111 (학생번호가 2이면 22222, 학생번호가 3이면 33333….)
      * 권한 집합: **장치 운영자**

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-970" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/04/4-4.png?fit=871%2C341" alt="액세스 제어 - 로컬장치" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/04/4-4.png?w=871 871w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/04/4-4.png?resize=300%2C117 300w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/04/4-4.png?resize=768%2C301 768w" sizes="(max-width: 871px) 100vw, 871px" data-recalc-dims="1" />
</p>

  * 새 장치 사용자 계정에 파트너 계정 정보를 다음과 같이 입력한다. 
      * 표시이름: Studentn (n은 학생 번호) (예) Student2
      * 전자우편 주소: <sn@ppsdemo.net> (예) <s2@ppsdemo.net>
      * 네트워크 이름: PPSDEMO\sn (예) PPSDEMO\s2
      * 액세스코드: 22222
      * 권한 집합: **장치 사용자**

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-971" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/04/5-5.png?fit=874%2C359" alt="액세스 제어 - 로컬장치" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/04/5-5.png?w=874 874w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/04/5-5.png?resize=300%2C123 300w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/04/5-5.png?resize=768%2C315 768w" sizes="(max-width: 874px) 100vw, 874px" data-recalc-dims="1" />
</p>

  * **로그인 및 권한 정책** – “**응용 프로그램 복사**”를 아래와 같이 설정 후 화면 제일 아래 “**적용**” 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-972" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/04/6-3.png?fit=1111%2C315" alt="액세스 제어 - 로컬장치" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/04/6-3.png?w=1111 1111w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/04/6-3.png?resize=300%2C85 300w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/04/6-3.png?resize=768%2C218 768w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/04/6-3.png?resize=1024%2C290 1024w" sizes="(max-width: 1000px) 100vw, 1000px" data-recalc-dims="1" />
</p>

## <span id="i-2">복합기 테스트</span>

  * 복합기 홈 화면에서 &#8220;**복사**&#8221; 선택

<p style="padding-left: 30px;">
   <img class="alignnone size-full wp-image-991" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/04/copy_menu.png?fit=298%2C115" alt="copy_menu" data-recalc-dims="1" />
</p>

  * 액세스 코드에 사용자 추가시 설정한 본인의 코드를 입력한다. (예) 1111

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-973" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/04/7-3.png?fit=800%2C600" alt="액세스 제어 - 로컬장치" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/04/7-3.png?w=800 800w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/04/7-3.png?resize=300%2C225 300w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/04/7-3.png?resize=768%2C576 768w" sizes="(max-width: 800px) 100vw, 800px" data-recalc-dims="1" />
</p>

  * 복사 화면이 나오면 화면 상단에 사용자 이름으로 로그인인 되었는지 확인한다.

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-974" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/04/8-4.png?fit=800%2C600" alt="액세스 제어 - 로컬장치" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/04/8-4.png?w=800 800w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/04/8-4.png?resize=300%2C225 300w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/04/8-4.png?resize=768%2C576 768w" sizes="(max-width: 800px) 100vw, 800px" data-recalc-dims="1" />
</p>

  * 같은 방법은 다른 사용자 액세스 코드로 로그인 한다.

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-975" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/04/9-1.png?fit=800%2C600" alt="액세스 제어 - 로컬장치" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/04/9-1.png?w=800 800w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/04/9-1.png?resize=300%2C225 300w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/04/9-1.png?resize=768%2C576 768w" sizes="(max-width: 800px) 100vw, 800px" data-recalc-dims="1" />
</p>

## <span id="i-3">복합기 테스트</span>

  * 내장 웹서버 우측 상단 &#8220;**로그아웃**&#8221; 클릭해서 로그 아웃한다

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-976" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/04/10-2.png?fit=233%2C102" alt="Access Control-Local 10" data-recalc-dims="1" />
</p>

  * &#8220;**로그인**&#8221; 선택

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-977" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/04/11-3.png?fit=221%2C100" alt="액세스 제어 - 로컬장치" data-recalc-dims="1" />
</p>

  * 로컬 장치 계정을 “**로컬 장치 사용자**” 로 변경 후 암호에 admin 이 아니라 본인이 설정장 액세스 코드 (예, 11111) 를 입력한다

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-978" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/04/12-3.png?fit=453%2C390" alt="액세스 제어 - 로컬장치" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/04/12-3.png?w=453 453w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/04/12-3.png?resize=300%2C258 300w" sizes="(max-width: 453px) 100vw, 453px" data-recalc-dims="1" />
</p>

  * 우측 상단에 사용자 이름을 보면 실제 사용자명이 나타난다. (예) Student

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-979" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/04/13-2.png?fit=196%2C73" alt="액세스 제어 - 로컬장치" data-recalc-dims="1" />
</p>

  * 로그 아웃 후 같은 방법으로 파트너 코드 (권한 집합이 장치 사용자)로 로그인한다. 무엇이 다른가?

## <span id="i-4">여러 사용자 한꺼번에 추가 (가져오기)</span>

  * **보안** &#8211; **액세스 제어**
  * 스크롤 다운 &#8220;**장치 사용자 계정**&#8220;, **내보내기** 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-980" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/04/16.png?fit=1105%2C221" alt="액세스 제어 - 로컬장치" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/04/16.png?w=1105 1105w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/04/16.png?resize=300%2C60 300w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/04/16.png?resize=768%2C154 768w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/04/16.png?resize=1024%2C205 1024w" sizes="(max-width: 1000px) 100vw, 1000px" data-recalc-dims="1" />
</p>

  * 내보내기 클릭 후 바탕화면에 CSV 파일을 저장한다.

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-982" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/04/18-1.png?fit=79%2C75" alt="액세스 제어 - 로컬장치" data-recalc-dims="1" />
</p>

  * 파일을 열어 보면 아래와 같다. (엑셀이 없으면 노트패드로 내용을 확인)

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-983" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/04/19-1.png?fit=918%2C98" alt="액세스 제어 - 로컬장치" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/04/19-1.png?w=918 918w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/04/19-1.png?resize=300%2C32 300w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/04/19-1.png?resize=768%2C82 768w" sizes="(max-width: 918px) 100vw, 918px" data-recalc-dims="1" />
</p>

  * 엑셀로 파일에 사용자 정보를 추가 후 바탕화면에 저장함 (예, “User_list.csv”)

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-984" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/04/20-2.png?fit=918%2C265" alt="액세스 제어 - 로컬장치" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/04/20-2.png?w=918 918w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/04/20-2.png?resize=300%2C87 300w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/04/20-2.png?resize=768%2C222 768w" sizes="(max-width: 918px) 100vw, 918px" data-recalc-dims="1" />
</p>

  * “**장치 사용자 계정**”, 가져오기 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-985" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/04/21-2.png?fit=1112%2C234" alt="액세스 제어 - 로컬장치" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/04/21-2.png?w=1112 1112w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/04/21-2.png?resize=300%2C63 300w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/04/21-2.png?resize=768%2C162 768w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/04/21-2.png?resize=1024%2C215 1024w" sizes="(max-width: 1000px) 100vw, 1000px" data-recalc-dims="1" />
</p>

  * “**찾아보기**” 클릭 후 바탕화면의 “User_list.csv” 선택, **가져오기** 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-986" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/04/22.png?fit=549%2C358" alt="액세스 제어 - 로컬장치" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/04/22.png?w=549 549w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/04/22.png?resize=300%2C196 300w" sizes="(max-width: 549px) 100vw, 549px" data-recalc-dims="1" />
</p>

  * 아래와 같이 사용자들이 추가됨

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-987" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/04/23.png?fit=794%2C450" alt="액세스 제어 - 로컬장치" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/04/23.png?w=794 794w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/04/23.png?resize=300%2C170 300w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/04/23.png?resize=768%2C435 768w" sizes="(max-width: 794px) 100vw, 794px" data-recalc-dims="1" />
</p>

  * 복합기에서 “**복사**” 를 누르고 등록된 액세스 코드로 로그인이 되는지 확인한다.

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-991" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/04/copy_menu.png?fit=298%2C115" alt="copy_menu" data-recalc-dims="1" />
</p>