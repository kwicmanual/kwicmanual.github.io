---
title: 디몬팀원 매뉴얼
sidebar: manual_sidebar
permalink: manual_introduction_dmon.html
folder: manual
---

    모니터링 레벨순위
<left><img src="/images/monitoring_level_dmon.png" width="100%" height="100%"></left>
<left><img src="/images/alert_manual_dmon.png" width="100%" height="100%"></left>

    근무자 역할
<left><img src="/images/team_role_dmon.png" width="100%" height="100%"></left>

    




## 장애 대응 매뉴얼
    장애는 아래와 같이 3단계로 분류됩니다.
    1,2단계는 입력정보 및 로그정보를 VOC로 작성하여, 담당팀에 전달해주시기 바랍니다.
    3단계는 내용을 정리하여, 디몬 팀장에게 보고 합니다.
<left><img src="/images/error_range.png" width="100%" height="100%"></left>


## 장애VOC 기재 방법
    VOC 기재는 다음과 같은 양식을 유지하여 작성해주시기 바랍니다. 

<left><img src="/images/issue_type.png" width="100%" height="100%"></left>
<left><img src="/images/issue_title.png" width="100%" height="100%"></left>
<left><img src="/images/issue_contents.png" width="100%" height="100%"></left>


## 장애상황 안내
    장애상황 전달은 다음과 같은 양식을 유지하여 작성해주시기 바랍니다.

|변수명|옵션|
|------|---|
|{기관명}||
|{시점}|MM/dd hh:mm|
|{장애원인}|1. 사이트 접속지연 이슈<br>2. 사이트 장애<br>3. 홈페이지 변경에 따른 스크래핑 장애|
|{점검내용}|1. 사이트 점검<br>2. 서버인증서 교체작업<br>3. 기타|
|{사이트주소}||
|{업무명}||

|정상안내|
|-------|
|[정상화안내]<br><br>사이트명: {기관명}<br>업무명: {업무명}<br>정상화시점: {시점}<br><br>{장애원인}  해결로<br>스크래핑 정상조회됨을 안내드립니다 

|장애안내|
|-------|
|[장애 안내]<br><br>사이트명: {기관명}<br>업무명: {업무명}<br>장애시점: {시점} <br><br>{장애원인}로 인하여<br>스크래핑 오류율이 증가되고 있음을 안내드립니다.

|점검안내|
|-------|
|[점검예정 안내]<br><br>사이트명: {기관명}<br>점검일시: {시점} <br><br>점검내용: {점검내용} <br><br>위와 같은 이유로 해당시점에는 스크래핑조회가 원활하지 않을 수 있으니 참고해주시기 바랍니다. <br><br>자세한 내용은 {사이트주소}를 참고해주시기 바랍니다. |
|[본사 점검 안내]<br><br>점검일시: {시점 ~ 시점}<br>점검내용: {점검내용} <br><br>위와 같은 이유로 인하여, 서비스 이용시 일시적인 장애가 발생되실 수 있습니다.<br>업무에 참고해주시기 바랍니다.|

<p style="color:red;">페이지 작성 중에 있습니다.</p>

<!--bundle exec jekyll serve-->

<!-- 
{% include checkErr.html %}
<p style="color:red;">장애가 발생된 상황에서 5분내로 담당자가 문자 회신이 없을 경우 전화 해주시기 바랍니다.</p>

## 0. 업무 시작시 담당자에게 시작함을 알립니다.

## 1. 제공해드린 입력값으로 조회가 잘 되는지 확인 바랍니다.
    유의사항: DukTape Version (버전받기) 누른 후 진행 해주시기 바랍니다. 
<left><img src="/images/manual/manual01.png" width="100%" height="100%"></left>

## 2. 장애 발생시 담당자에게 연락해주시기 바랍니다.
<left><img src="/images/manual/manual02.png" width="100%" height="100%"></left>
    연락예시: 오전 10:21 정부24 주민등록표등본발급 장애 감지하였습니다. 

## 3. 그라파나 모니터링 장애 그래프를 캡쳐한 후 담당자에게 전달합니다.
<left><img src="/images/manual/manual03.png" width="100%" height="100%"></left>

## 4. 스크래핑 툴을 통해 정상 작동 되는지 확인 바랍니다.
    참고사항: 정상적으로 작동될 경우 담당자에게 정상작동 됨을 안내합니다. (안될 경우 결과값을 담당자에게 보내줍니다.)
<left><img src="/images/manual/manual04.png" width="100%" height="100%"></left>

## 5. 스크래핑 장애 발생시 사이트에서 정상 작동되는지 유무를 확인 바랍니다.
    참고사항: 업무별 매뉴얼은 모니터링 매뉴얼 또는 검색을 통해 확인해 주시기 바랍니다. 
<left><img src="/images/manual/manual05.png" width="100%" height="100%"></left>

## 6. 해당케이스의 모든상황은 담당자가 알고 있어야 합니다.
    연락예시: 정부24 주민등록표등본 장애 확인해본 결과 툴은 장애이며, 사이트는 정상입니다.

## 7. 정상화 감지시 담당자에게 보고합니다.
<left><img src="/images/manual/manual06.png" width="100%" height="100%"></left>
    연락예시: 오전 10:45 정부24 주민등록표등본발급 정상화 감지하였습니다.

## 8. 업무가 종료된 후 최대 30분 내로 담당자에게 보고서를 제출해주시기 바랍니다. 
    유의사항: 시간내에 제출하지 않을 경우 근무하지 않은 케이스로 의심 받으실 수 있습니다.

{% include monitoringex.html %}
<left><img src="/images/manual/manual07.png" width="70%" height="70%"></left>

{% include note.html content="
1. 알람감지를 신속하게 하지 못할 경우
2. 사전에 의논없이 휴가를 통보하여 업무에 공백이 발생할 경우(최소 1~2주 전 미리 상의 바랍니다.)
해당 사항이 발생할 경우 업무는 종료됩니다." %}

{% include links.html %} -->
