---
id: 1443
title: 드라이버 자동 설치 스크립트
date: 2016-05-07T09:06:05+00:00
author: 홍 순모
layout: page
guid: http://hpidemo.net/?page_id=1443
---
프린터 추가 마법사나 벤더에서 제공하는 설치 프로그램을 이용해서 설치를 하게 되면 단계가 많아서 일반 사용자가 설치하기가 불편하고 시간도 많이 걸린다. 이를 자동화해서 쉽게 설치하려면 Windows 에서 제공하는 Rundll32 나 UPD의 경우 install.exe 를 이용해서 스크립트를 만들면 된다. 이번 실습에서는 스크립트를 이용해서 드라이버를 설치해 보겠다.

  * 실습용 샘플 파일 다운로드 <div class='w3eden'>
      <!-- WPDM Link Template: Default Template -->
      
      <div class="wpdm-link-tpl link-btn [color]" data-durl="http://hpidemo.net/download/hp-printer-driver-installer-sample/?wpdmdl=1606" >
        <div class="media">
          <div class="pull-left">
            <img class="wpdm_icon" alt="Icon"   src="http://i1.wp.com/hpidemo.net/wp-content/plugins/download-manager/assets/file-type-icons/down2.png" data-recalc-dims="1" />
          </div>
          
          <div class="media-body">
            <strong class="ptitle">HP 프린터 드라이버 자동 설치팩 샘플 <span class="label label-default" style="font-weight: 400;">76.91 MB</span></strong> 
            
            <div>
              <strong><a class='wpdm-download-link wpdm-download-locked [btnclass]' rel='nofollow' href='#' onclick="location.href='http://hpidemo.net/download/hp-printer-driver-installer-sample/?wpdmdl=1606';return false;">다운로드</a></strong>
            </div>
          </div>
        </div>
      </div>
      
      <div style="clear: both">
      </div>
    </div>

  * “**HP\_프린터\_드라이버팩_Beta.exe**” 를 바탕화면으로 복사 후 더블 클릭
  * **2** 입력 후 (엔터)

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1547" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/install_script_01.png?fit=675%2C167" alt="install_script_01" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/install_script_01.png?w=675 675w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/install_script_01.png?resize=300%2C74 300w" sizes="(max-width: 675px) 100vw, 675px" data-recalc-dims="1" />
</p>

  * **복합기 IP** 를 입력 후 엔터 (예, 172,16,10.15n)

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1548" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/install_script_02.png?fit=675%2C216" alt="install_script_02" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/install_script_02.png?w=675 675w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/install_script_02.png?resize=300%2C96 300w" sizes="(max-width: 675px) 100vw, 675px" data-recalc-dims="1" />
</p>

  * **4** 입력 후 엔터

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1549" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/install_script_03.png?fit=677%2C442" alt="install_script_03" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/install_script_03.png?w=677 677w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/install_script_03.png?resize=300%2C196 300w" sizes="(max-width: 677px) 100vw, 677px" data-recalc-dims="1" />
</p>

  * 스크립트가 실행되면서 포트를 만들고 프린터 드라이버를 자동으로 설치한다.

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1543" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/install_script_04.png?fit=674%2C74" alt="install_script_04" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/install_script_04.png?w=674 674w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/install_script_04.png?resize=300%2C33 300w" sizes="(max-width: 674px) 100vw, 674px" data-recalc-dims="1" />
</p>

  * **2** 를 입력 후 엔터 (설치 종료)

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1544" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/install_script_05.png?fit=675%2C106" alt="install_script_05" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/install_script_05.png?w=675 675w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/install_script_05.png?resize=300%2C47 300w" sizes="(max-width: 675px) 100vw, 675px" data-recalc-dims="1" />
</p>

  * **시작** – **장치 및 프린터**, 드라이버가 설치가 되었는지 확인

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1545" src="http://i2.wp.com/hpidemo.net/wp-content/uploads/2016/05/install_script_06.png?fit=102%2C147" alt="install_script_06" data-recalc-dims="1" />
</p>

  * 설치 스크립트의 내용을 확인한다. c:\HP\_Print\_Drivers  에 “**printer_install.bat**” 파일을  메모장으로 열어서 내용을 확인할 수 있음

<p style="padding-left: 30px;">
  <img class="alignnone size-full wp-image-1546" src="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/install_script_07.png?fit=734%2C549" alt="install_script_07" srcset="http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/install_script_07.png?w=734 734w, http://i0.wp.com/hpidemo.net/wp-content/uploads/2016/05/install_script_07.png?resize=300%2C224 300w" sizes="(max-width: 734px) 100vw, 734px" data-recalc-dims="1" />
</p>