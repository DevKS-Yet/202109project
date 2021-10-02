# Java Spring framework를 이용한 밀키트 

## 0. 목차

[1. 개요](#1-개요)

[2. 기술](#2-기술)

[3. Use Case](#3-Use-Case)

[4. Flow Chart](#4-Flow-Chart)

[5. database ER Diagram](#5-database-er-diagram)

[6. 사이트 맵](#6-사이트-맵)

[7. 기능](#7-기능)

[8. 구현한 기능](#8-구현한-기능)

[9. 게시물 실행 영상](#9-게시물-실행-영상)

## 1. 개요

jsp을 사용한 회원들은 자유롭게 판매자가 올린 밀키트를 주문하는 사이트입니다.

게시판으로는 공지사항/이벤트/1대1문의 게시판이 있습니다.

지도 항목은 다음주소api를 사용해 판매자의 위치를 확인할 수 있고 해당 판매자 클릭시 판매자의 판매 상품을 볼 수 있습니다.

결제는 카카오페이 api를 이용해 결제할 수 있습니다.

관리자는 기간별 상품 판매 통계를 확인할 수 있습니다.

## 2. 기술
1. Web Front : `HTML5` , `CSS`, `JavaScript`, `Jquery` , `Ajax`
2. Web Server :  `Java`, `ApacheTomcat`
3. DBMS : `Oracle DB`
4. 개발환경 : `Eclipse, Spring framework`


## 3. Use Case
![image](https://user-images.githubusercontent.com/81474598/135708449-3c7f48d6-9cf6-4640-9a47-c5e11b4f90bd.png)


## 4. Flow Chart
![image](https://user-images.githubusercontent.com/81474598/135708462-7bce6caa-f6c0-4d37-a1e5-c322b1357e4e.png)


## 5. database ER Diagram
![캡처](https://user-images.githubusercontent.com/81474598/135708360-7d1501c2-e749-426b-b15a-4779d3728dac.png)


## 6. 사이트맵
![image](https://user-images.githubusercontent.com/81474598/135651292-d68b441d-7d2a-4df0-8643-ab00f277f77d.png)


## 7. 기능
1. 로그인/회원가입
2. 게시판 CRUD
3. 장바구니/결제
4. 마이페이지
5. 기간별 통계 차트

1. 메인페이지 - 베스트 상품 (별점순으로 높은 상품 3개가 메인페이지에 표시)
2. 메인페이지 - 베스트 리뷰 (별점중 4점 이상이며 사진이 몇장 이상인 리뷰 3개를 메인페이지에 표시)
3. 회원가입 - sms인증 (SENS API)
4. 회원가입 - Daum 주속 API
5. 회원가입 - Ajax를 이용한 아이디 중복 검사
6. 회원가입 - spring-security를 이용한 비밀번호 암호화(bcryt)
7. 로그인
8. 지도 - 등록된 상호들을 지도에서 확인 가능 및 클릭 시 판매 상품 확인 가능
9. 이벤트 게시판 - CRUD
10. 공지사항 계시판 - CRUD
11. 1대1문의 게시판 - 상품/환불/배송 문의와 전체/제목/내용/작성자로 검색 가능
12. 상품 리스트/뷰
13. 장바구니 - Ajax를 이용한 상품 변경
14. 결제 - 카카오 결제 API 사용
15. 주문내역 조회(상호)
16. 마이페이지(일반) - 수정 및 주문 내역 조회 가능하며 환불처리 가능
17. 마이페이지(일반) - 상품 평가 기능
18. 마이페이지(상호) - 회원정보 수정 및 상품 CRUD 가능
19. 관리자페이지 - 회원정보 CRUD
20. 관리자페이지 - 사업자 정보 출력 및 해당 상호 상품 목록 출력 가능
21. 관리자페이지 - Datepicker와 Zingchart를 활용한 기간별 상품 판매량을 그래프 및 수치로 확인


## 8. 구현한 기능
제가 구현한 기능입니다.

1. 회원가입 - SMS 인증 (SENS API)
2. 회원가입 - 도로명 주소 API (Daum API)
3. 회원가입 - Ajax를 이용한 아이디 중복 검사 및 그 외 유효성 검사
4. 로그인
5. 상품 리스트 - 분류/조리시간과 전체/상품명/상호명에 따른 검색 기능
6. 상품 리스트 - 페이징 처리
7. 장바구니 - Ajax를 용한 상품 변경
8. 관리자페이지 - 회원정보 CRUD
9. 관리자페이지 - Zingchart를 활용한 기간별 상품 판매량을 그래프로 표시


## 9. 게시물 실행 영상
https://www.youtube.com/watch?v=bn91sRhUtxg&feature=youtu.be

