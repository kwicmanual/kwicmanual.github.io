---
title: 모니터링 근무자 업무 매뉴얼
sidebar: manual_sidebar
permalink: manual_introduction.html
folder: manual
---

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

{% include links.html %}
