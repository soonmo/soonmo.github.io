---
title: Scan to email
layout: page
permalink: /tutorials/fs-device-ug/scan-to-email/
---
<div id="toc_container" class="no_bullets">
  <p class="toc_title">
    목차
  </p>
  
  <ul class="toc_list">
    <li>
      <a href="#__SMTP"><span class="toc_number toc_depth_1">1</span> 메일 전송 서버 (SMTP) 설정</a>
    </li>
    <li>
      <a href="#i"><span class="toc_number toc_depth_1">2</span> 메일 수신 확인</a>
    </li>
    <li>
      <a href="#i-2"><span class="toc_number toc_depth_1">3</span> 세부 설정</a>
    </li>
    <li>
      <a href="#i-3"><span class="toc_number toc_depth_1">4</span> 복합기 테스트</a>
    </li>
    <li>
      <a href="#i-4"><span class="toc_number toc_depth_1">5</span> 메일 수신 확인</a>
    </li>
  </ul>
</div>

복합기에서 스캔한 문서를 메일 전송 서버를 통해서 전송하는 방식으로 로컬 인증, LDAP 인증 설정과 연동되면 강력해진다. 어떻게 작동하는지 이번 실습을 통해서 살펴 본다.

## <span id="__SMTP">메일 전송 서버 (SMTP) 설정</span>

  * “**스캔/디지털 전송**” &#8211; &#8220;**전자우편**&#8221; (좌측 메뉴) 클릭, 발신 **전자우편 서버(SMTP)** 하단 “**추가**” 메뉴 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1021" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/1.png?fit=637%2C339" alt="Scan to email " srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/1.png?w=637 637w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/1.png?resize=300%2C160 300w" sizes="(max-width: 637px) 100vw, 637px" data-recalc-dims="1" />
</p>

  * SMTP 서버 주소 입력 후 &#8220;**다음**&#8221; 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1022" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/2.png?fit=510%2C216" alt="Scan to email " srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/2.png?w=510 510w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/2.png?resize=300%2C127 300w" sizes="(max-width: 510px) 100vw, 510px" data-recalc-dims="1" />
</p>

  * &#8220;**다음**&#8221; 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1023" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/3.png?fit=680%2C290" alt="Scan to email " srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/3.png?w=680 680w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/3.png?resize=300%2C128 300w" sizes="(max-width: 680px) 100vw, 680px" data-recalc-dims="1" />
</p>

  * **서버에 인증이 필요하지 않습니다**. “**다음**”

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1024" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/4.png?fit=502%2C201" alt="Scan to email " srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/4.png?w=502 502w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/4.png?resize=300%2C120 300w" sizes="(max-width: 502px) 100vw, 502px" data-recalc-dims="1" />
</p>

  * &#8220;**다음**&#8220;

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1025" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/5.png?fit=498%2C263" alt="Scan to email " srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/5.png?w=498 498w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/5.png?resize=300%2C158 300w" sizes="(max-width: 498px) 100vw, 498px" data-recalc-dims="1" />
</p>

  * 테스트 전자우편 보낼 주소: [s**n**@ppsdemo.net](mailto:sn@ppsdemo.net) (예) <s1@ppsdemo.net> 후 “**테스트**” 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1026" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/6.png?fit=437%2C320" alt="Scan to email " srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/6.png?w=437 437w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/6.png?resize=300%2C220 300w" sizes="(max-width: 437px) 100vw, 437px" data-recalc-dims="1" />
</p>

  * &#8220;**마침**&#8221; 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1027" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/7.png?fit=492%2C399" alt="Scan to email " srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/7.png?w=492 492w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/7.png?resize=300%2C243 300w" sizes="(max-width: 492px) 100vw, 492px" data-recalc-dims="1" />
</p>

## <span id="i">메일 수신 확인</span>

  * IE 주소에 [http://mail.ppsdemo.net](http://mail.ppsdemo.net/) 입력 
      * 사용자명: 이메일 주소, (예) <s1@ppsdemo.net>
      * 암호: 계정 암호, (예)S1
      * “**로그인**” 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1028" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/8.png?fit=576%2C413" alt="Scan to email" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/8.png?w=576 576w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/8.png?resize=300%2C215 300w" sizes="(max-width: 576px) 100vw, 576px" data-recalc-dims="1" />
</p>

  * 메일 확인

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1029" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/9.png?fit=1365%2C204" alt="Scan to email" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/9.png?w=1365 1365w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/9.png?resize=300%2C45 300w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/9.png?resize=768%2C115 768w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/9.png?resize=1024%2C153 1024w" sizes="(max-width: 1000px) 100vw, 1000px" data-recalc-dims="1" />
</p>

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1030" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/9-1.png?fit=1135%2C164" alt="Scan to email" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/9-1.png?w=1135 1135w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/9-1.png?resize=300%2C43 300w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/9-1.png?resize=768%2C111 768w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/9-1.png?resize=1024%2C148 1024w" sizes="(max-width: 1000px) 100vw, 1000px" data-recalc-dims="1" />
</p>

## <span id="i-2">세부 설정</span>

  * 주소 및 메시지 필드 제어 
      * 보내는 사람: **사용자 주소(로그인 필수)** , “**사용자 편집 가능**” 해제
      * 받는 사람: **사용자 주소(로그인 필수)**
      * 제목: 디지털 전송
      * 메시지: 안녕하세요? 첨부문서는 hp 디지털 복합기에서 200dpi PDF로 스캔한 문서입니다. 감사합니다.

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1032" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/11.png?fit=594%2C582" alt="Scan to email" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/11.png?w=594 594w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/11.png?resize=300%2C294 300w" sizes="(max-width: 594px) 100vw, 594px" data-recalc-dims="1" />
</p>

  * 스캔 설정 
      * 이미지 미리 보기: “**미리 보기 필요**”
      * **여러 장의 페이지 급지 인식**: 해제
      * ㈜ 선택이 될 때와 해제될 때의 차이점이 무엇인가?

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1033" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/12.png?fit=1071%2C298" alt="Scan to email" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/12.png?w=1071 1071w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/12.png?resize=300%2C83 300w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/12.png?resize=768%2C214 768w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/12.png?resize=1024%2C285 1024w" sizes="(max-width: 1000px) 100vw, 1000px" data-recalc-dims="1" />
</p>

  * 첨부 설정 
      * 기본 해상도: **200dpi**
      * 파일 이름 접두사: “**사용자이름(%SECURITY_USERNAME%)**”
      * 기본 파일 이름: **\_문서\_**
      * 파일 이름 접미사: “**날짜(%DEVICE\_DATE\_YYYYMMDD%)**”
      * 파일 이름 미리 보기: “**업데이트 미리 보기**” 클릭해서 확인
      * 여러 파일로 스캔: 이 옵션을 선택하면 1장당 1개의 PDF 파일로 생성한다.
      * &#8220;**적용**&#8221; 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1034" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/13.png?fit=813%2C610" alt="Scan to email" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/13.png?w=813 813w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/13.png?resize=300%2C225 300w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/13.png?resize=768%2C576 768w" sizes="(max-width: 813px) 100vw, 813px" data-recalc-dims="1" />
</p>

  * 보안 – 액세스 제어, 로그인 및 권한 정책의 “**전자우편 응용 프로그램**”을 아래와 같이 설정한다.

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1035" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/14.png?fit=1102%2C119" alt="Scan to email" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/14.png?w=1102 1102w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/14.png?resize=300%2C32 300w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/14.png?resize=768%2C83 768w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/14.png?resize=1024%2C111 1024w" sizes="(max-width: 1000px) 100vw, 1000px" data-recalc-dims="1" />
</p>

  * &#8220;**적용**&#8221; 클릭

## <span id="i-3">복합기 테스트</span>

  * 복합기 홈화면에서 “**전자우편**” 선택

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1036" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/15.png?fit=369%2C143" alt="Scan to email" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/15.png?w=369 369w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/15.png?resize=300%2C116 300w" sizes="(max-width: 369px) 100vw, 369px" data-recalc-dims="1" />
</p>

  * 사용자 이름, 암호 입력

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1037" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/16.png?fit=800%2C600" alt="Scan to email" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/16.png?w=800 800w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/16.png?resize=300%2C225 300w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/16.png?resize=768%2C576 768w" sizes="(max-width: 800px) 100vw, 800px" data-recalc-dims="1" />
</p>

  * ㈜ 보내는 사람 변경 불가능하다. 
      * ADF (문서 공급기) 에 스캔할 문서를 3~4장 정도 적재한다.\
      * 스크린 상단의 “전자 우편 전송” 선택

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1038" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/17.png?fit=800%2C600" alt="Scan to email" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/17.png?w=800 800w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/17.png?resize=300%2C225 300w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/17.png?resize=768%2C576 768w" sizes="(max-width: 800px) 100vw, 800px" data-recalc-dims="1" />
</p>

  * 미리보기: 스캔된 문서가 복합기의 화면에 나타난다.

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1039" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/18.png?fit=800%2C600" alt="Scan to email" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/18.png?w=800 800w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/18.png?resize=300%2C225 300w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/18.png?resize=768%2C576 768w" sizes="(max-width: 800px) 100vw, 800px" data-recalc-dims="1" />
</p>

  * 화면 하단의 “**확대(돋보기)**” 아이콘 선택하면 스캔된 문서가 확대된다.

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1056" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/magnifier.png?fit=73%2C36" alt="magnifier" data-recalc-dims="1" />
</p>

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1040" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/19.png?fit=800%2C600" alt="Scan to email" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/19.png?w=800 800w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/19.png?resize=300%2C225 300w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/19.png?resize=768%2C576 768w" sizes="(max-width: 800px) 100vw, 800px" data-recalc-dims="1" />
</p>

  * 화면 하단의 “**썸네일**” 아이콘 선택

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1059" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/thumbnail.png?fit=74%2C34" alt="thumbnail" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/thumbnail.png?w=74 74w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/thumbnail.png?resize=520%2C245 520w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/thumbnail.png?resize=720%2C340 720w" sizes="(max-width: 74px) 100vw, 74px" data-recalc-dims="1" />
</p>

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1041" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/20.png?fit=800%2C600" alt="Scan to email" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/20.png?w=800 800w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/20.png?resize=300%2C225 300w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/20.png?resize=768%2C576 768w" sizes="(max-width: 800px) 100vw, 800px" data-recalc-dims="1" />
</p>

  * 페이지 삭제 &#8211; 첫번째 페이지 선택 후 좌측 쓰레기통 아이콘 선택

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1054" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/delete.png?fit=70%2C55" alt="delete" data-recalc-dims="1" />
</p>

  * 페이지 삭제 확인 메시지가 나타나면 “**삭제**” 버튼 선택

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1042" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/21.png?fit=800%2C600" alt="Scan to email" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/21.png?w=800 800w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/21.png?resize=300%2C225 300w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/21.png?resize=768%2C576 768w" sizes="(max-width: 800px) 100vw, 800px" data-recalc-dims="1" />
</p>

  * 페이지 순서 바꾸기 – 첫번째 페이지 선택 후 좌측 페이지 순서 바꾸기 아이콘 선택

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1043" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/22.png?fit=800%2C600" alt="Scan to email" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/22.png?w=800 800w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/22.png?resize=300%2C225 300w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/22.png?resize=768%2C576 768w" sizes="(max-width: 800px) 100vw, 800px" data-recalc-dims="1" />
</p>

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1057" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/reorder.png?fit=74%2C54" alt="reorder" data-recalc-dims="1" />
</p>

  * 마지막 페이지 위에 아이콘 선택해서 마지막 페이지로 이동

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1043" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/22.png?fit=800%2C600" alt="Scan to email" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/22.png?w=800 800w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/22.png?resize=300%2C225 300w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/22.png?resize=768%2C576 768w" sizes="(max-width: 800px) 100vw, 800px" data-recalc-dims="1" />
</p>

  * 가로/세로 회전 – 첫번째 페이지 선택 후 문서 회전 아이콘 선택

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1058" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/rotate.png?fit=73%2C51" alt="rotate" data-recalc-dims="1" />
</p>

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1045" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/23.png?fit=800%2C600" alt="Scan to email" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/23.png?w=800 800w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/23.png?resize=300%2C225 300w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/23.png?resize=768%2C576 768w" sizes="(max-width: 800px) 100vw, 800px" data-recalc-dims="1" />
</p>

  * 새로운 페이지 추가 – 페이지 추가 아이콘 선택

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1053" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/add_page.png?fit=71%2C53" alt="add_page" data-recalc-dims="1" />
</p>

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1046" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/24.png?fit=800%2C600" alt="Scan to email" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/24.png?w=800 800w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/24.png?resize=300%2C225 300w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/24.png?resize=768%2C576 768w" sizes="(max-width: 800px) 100vw, 800px" data-recalc-dims="1" />
</p>

  * ADF 에 문서을 적재 후 “**스캔**” 선택
  * 화면 상단의 “**전자우편 전송**” 선택

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1055" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/email_app.png?fit=193%2C39" alt="email_app" data-recalc-dims="1" />
</p>

  * &#8220;**추가**&#8221; 선택

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1048" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/26.png?fit=800%2C600" alt="Scan to email" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/26.png?w=800 800w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/26.png?resize=300%2C225 300w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/26.png?resize=768%2C576 768w" sizes="(max-width: 800px) 100vw, 800px" data-recalc-dims="1" />
</p>

  * &#8220;**확인**&#8220;

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1049" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/27.png?fit=800%2C600" alt="Scan to email" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/27.png?w=800 800w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/27.png?resize=300%2C225 300w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/27.png?resize=768%2C576 768w" sizes="(max-width: 800px) 100vw, 800px" data-recalc-dims="1" />
</p>

## <span id="i-4">메일 수신 확인</span>

  * IE 주소에 [http://mail.ppsdemo.net](http://mail.ppsdemo.net/) 입력 
      * 사용자명: 이메일 주소, (예) <s1@ppsdemo.net>
      * 암호: 계정 암호, (예)S1
      * “**로그인**” 클릭
  * 메일확인

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1050" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/29.png?fit=1133%2C263" alt="Scan to email" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/29.png?w=1133 1133w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/29.png?resize=300%2C70 300w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/29.png?resize=768%2C178 768w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/29.png?resize=1024%2C238 1024w" sizes="(max-width: 1000px) 100vw, 1000px" data-recalc-dims="1" />
</p>