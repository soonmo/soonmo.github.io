---
title: AutoSend
layout: page
permalink: /tutorials/fs-device-ug/autosend/
---
AutoSend는 주기적으로 일련 번호, 이벤트 로그, 사용 페이지 수, 소모품 상태 정보 등 프린터 구성 정보 등을 HP 로 전송하거나 이메일, 웹서버 등으로 전송하는 기능이다.

사전 준비 사항

메일전송(SMTP) 서버

  * 일반 &#8211;  AutoSend
  * 다음과 같이 설정 
      * “**AutoSend 활성화**” 체크
      * 일, 주, 월, 인쇄 페이지 중에서 “**인쇄** **페이지**” 선택하고, 50 입력
      * HP로 보내기 체크 해제
      * 전자우편으로 전송 체크 후 수신자에 [s**n**@ppsdemo.net](mailto:sn@ppsdemo.net) 입력 후 “**추가**” 클릭
      * (**노트**) 전송 주기 설정에 따라서 프린터 정보를 보낸다. 예를 들어서 “일” 을 선택하고 “1” 을 입력면 하루에 한번 씩 프린터 정보를 메일로 보낸다.

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1238" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/2-6.png?fit=820%2C726" alt="AutoSend  2" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/2-6.png?w=820 820w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/2-6.png?resize=300%2C266 300w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/2-6.png?resize=768%2C680 768w" sizes="(max-width: 820px) 100vw, 820px" data-recalc-dims="1" />
</p>

  * 주소 지정에 [mfp**n**@ppsdemo.net](mailto:mfpn@ppsdemo.net) 을 입력 후 “**적용**” 클릭 (보내는 사람 주소로 표시)

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1238" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/2-6.png?fit=820%2C726" alt="AutoSend  2" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/2-6.png?w=820 820w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/2-6.png?resize=300%2C266 300w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/2-6.png?resize=768%2C680 768w" sizes="(max-width: 820px) 100vw, 820px" data-recalc-dims="1" />
</p>

  * &#8220;**테스트**&#8221; 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1240" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/4-7.png?fit=524%2C252" alt="AutoSend  4" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/4-7.png?w=524 524w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/4-7.png?resize=300%2C144 300w" sizes="(max-width: 524px) 100vw, 524px" data-recalc-dims="1" />
</p>

  * <http://mail.ppsdemo.net> 접속 후 로그인
  * 메일 확인 – “**Device Snapshot …** “ 으로 시작하는 제목의 메일임 더블 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1241" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/6-5.png?fit=1141%2C160" alt="AutoSend 6" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/6-5.png?w=1141 1141w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/6-5.png?resize=300%2C42 300w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/6-5.png?resize=768%2C108 768w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/6-5.png?resize=1024%2C144 1024w" sizes="(max-width: 1000px) 100vw, 1000px" data-recalc-dims="1" />
</p>

  * 첨부 파일 “Device.xml” 더블 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1234" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-6.png?fit=1138%2C257" alt="AutoSend  7" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-6.png?w=1138 1138w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-6.png?resize=300%2C68 300w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-6.png?resize=768%2C173 768w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-6.png?resize=1024%2C231 1024w" sizes="(max-width: 1000px) 100vw, 1000px" data-recalc-dims="1" />
</p>

  * &#8220;그래도 항상 표시&#8221; 클릭

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1235" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-1-1.png?fit=1145%2C228" alt="AutoSend  7-1" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-1-1.png?w=1145 1145w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-1-1.png?resize=300%2C60 300w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-1-1.png?resize=768%2C153 768w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-1-1.png?resize=1024%2C204 1024w" sizes="(max-width: 1000px) 100vw, 1000px" data-recalc-dims="1" />
</p>

  * 무슨 내용인지 알아 보기 힘들다. &#8220;다운로드&#8221; 클릭 후 바탕 화면에 저장

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1236" src="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-2-1.png?fit=1154%2C363" alt="AutoSend  7-2" srcset="http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-2-1.png?w=1154 1154w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-2-1.png?resize=300%2C94 300w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-2-1.png?resize=768%2C242 768w, http://i1.wp.com/hpidemo.net/wp-content/uploads/2016/05/7-2-1.png?resize=1024%2C322 1024w" sizes="(max-width: 1000px) 100vw, 1000px" data-recalc-dims="1" />
</p>

  * XML 파일 내에 아래와 같은 많은 정보가 포함되어 있다.

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1237" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/8-6.png?fit=647%2C773" alt="AutoSend  8" srcset="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/8-6.png?w=647 647w, http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/8-6.png?resize=251%2C300 251w" sizes="(max-width: 647px) 100vw, 647px" data-recalc-dims="1" />
</p>

&nbsp;