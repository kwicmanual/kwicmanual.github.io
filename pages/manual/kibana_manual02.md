---
title: 키바나 구성
keywords: 키바나, kibana, Kibana, KIBANA, 데이터, 대시보드, 매뉴얼
last_updated: Aug 28, 2022
tags: #[getting_started]
summary: "키바나 구성에 대한 매뉴얼 입니다."
sidebar: manual5_sidebar
permalink: kibana_manual02.html
folder: manual
---


||설명|
|---------------|---|
|Discover|Elasticsearch에 색인된 소스 데이터들의 검색|
|Visualize|조회된 데이터의 통계를 다양한 차트로 표현할 수 있는 패널을 만드는 메뉴|
|Dashboard|Visualize 메뉴에서 만들어진 시각화 도구들을 조합하여 페이지 구성|


## Discover

검색 창에 질의문을 통해 데이터를 간편하게 검색, 필터링 할 수 있습니다.<br>
보고 싶은 필드만 선택해서 조회가 가능하며, 히스토그램 그래프를 통해 시간대별 로그 확인이 가능합니다.

<left><img src="/images/kibana_view.png" width="100%" height="100%"></left><br>

1. Index Pattern    

    Data Source를 elasticsearch에서 가져오는 것으로, Index mapping 정보 등을 Kibana에서 사용하기 적합하게 미리 캐싱해둔 것입니다.
    여러개의 Index에 대한 Metadata를 병합해 저장했다가 검색/시각화 생성시 활용한다.

    |smartaib-*|최근 3개월이내 조회결과|
    |event-summary-*|최근 1년이내 조회결과(요약)|


2. Query

    관심 있는 필드 이름과 값을 사용하여 검색을 구성할 수 있습니다. 
    숫자 필드에는 보다 큼 (>), 보다 작음(<), 같음(=)과 같은 비교 연산자를 사용할 수 있습니다. 
    여러 요소를 논리 연산자 AND, OR, NOT(모두 대문자)으로 연결할 수 있습니다.

    [KQL(Kibana Query Language) 참고자료](https://blog.naver.com/PostView.nhn?blogId=occidere&logNo=222139661612&categoryNo=0&parentCategoryNo=0&viewDate=&currentPage=1&postListTopCurrentPage=1&from=postView)


3. Field

    | 필 드 명 | 의 미 | 비 고 |
    |----------|-------|------|
    |ACCESSKEY|업체 라이센스키||
    |ECODE|오류코드||
    |EMSG|개발자 오류메시지||
    |ERRMSG|고객용 오류메시지||
    |ETRACK|오류추적번호||
    |FCODE|기관코드||
    |MODULE|업무||
    |OS|실행된 OS환경||
    |RESULT|실행 결과||
    |UUID|고객ID|모바일 고객 오류 추적 시 사용되는 필드|
    |CERTKEY|업체 인증키||
    |FUNCNAME|오류 발생시 함수 추적||
    |HW|하드웨어||
    |REQID|추적ID|API 고객 오류 추적시 사용되는 필드|
    |REQTIME|실행 시작시간||
    |RESTIME|실행 종료시간||
    |VERCORE|엔진 버전||
    |VERSCR|스크래핑 버전||
    |createDT|로그 수집시간||
    |duration|스크래핑 실행시간||

## Visualize

Visualize는 조회된 데이터의 통계를 다양한 차트로 표현할 수 있는 패널을 만드는 메뉴입니다.

<left><img src="/images/visualize01.png" width="100%" height="100%"></left><br>

<p style="color:red;">페이지 작업 중입니다.</p>

{% include links.html %}
