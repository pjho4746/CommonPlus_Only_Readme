# 커먼플러스🛒 : 쇼핑몰 통합 관리 서비스
<div align="center">
  <img width="500" alt="main_image_5" src="https://github.com/harin1212/spring/assets/99604087/167173cf-b706-446e-a5ca-eaf6d64f5eae">
    <img width="500" alt="main_image_3" src="https://github.com/harin1212/spring/assets/99604087/5175999e-154f-44ac-99e3-7f62c11e43e1">
</div>

- 배포 URL : https://commonplus.store/
- Test ID : test@test.com
- Test PW : qqqqqqqq!

<br>

## 프로젝트 소개

- 커먼플러스는 ‘다중 플랫폼 쇼핑몰’ 통합 관리 서비스 입니다.
- 쿠팡, 11번가, g마켓, 옥션 셀러들은 자신의 쇼핑몰 계정을 등록하고, 보관상품 등록 + 쇼핑몰 그룹 등록을 통해 외부로 상품을 등록할 수 있습니다.

<br>

## 팀원 구성 및 역할

| **이름** |                                                                   **GitHub**                                                                   |                                                                           **구현 기능**                                                                            |
|:------:|:----------------------------------------------------------------------------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------------------------------------------------------------------------------:|
|  김은지   | [<img src="https://avatars.githubusercontent.com/u/78680486?v=4" height="100" width="100"> <br/> @thisiseunji](https://github.com/thissieunji) |     <ul><li>프로젝트 매니저</li><li>프로젝트 초기셋팅</li><li>외부상품 등록, 수정, 조회 기능</li><li>카테고리 조회, 고시정보 조회 기능</li><li>외부몰 계정 등록, 수정, 삭제, 조회 기능</li><li>택배사 조회 기능</li></ul>     |
|  김서영   |  [<img src="https://avatars.githubusercontent.com/u/111834724?v=4" height="100" width="100"> <br/> @seoyeong12](https://github.com/seoyeong12)   |                                                              <ul><li>비밀번호 재설정 기능</li><li>외부상품 등록, 수정, 조회 기능</li><li>주소록 등록, 수정, 조회 기능</li><li>출고지 등록, 수정, 조회,기타 기능</li><li>쇼핑몰 그룹 생성, 조회, 수정, 삭제 기능</li><li>상품 가격/재고/판매상태 수정, 조회 기능</li><li>커스텀 에러</li><li>쿠팡 반품 기능</li></ul>                                                                 |
|  김하린   |   [<img src="https://avatars.githubusercontent.com/u/99604087?v=4" height="100" width="100"> <br/> @harin1212](https://github.com/harin1212)   | <ul><li>로그인, 이메일 중복확인, 회원가입, 로그아웃 기능</li><li>이미지 및 상품 등록, 상품 수정, 조회, 삭제</li><li>외부몰 주문 조회, 취소</li><li>송장 입력, 수정</li><li>상품 준비중으로 변경</li><li>CI/CD 구축 및 배포</li> |
| 박지호  | [<img src="https://github.com/user-attachments/assets/5b67ef40-5da0-4622-b7ad-2b2104564372" alt="KakaoTalk" height="100"> <br/> @pjho4746](https://github.com/pjho4746)   | <ul><li>Swagger 문서 (로컬/배포 서버)</li><li>11번가 반품 기능</li> <li>11번가 고시 정보 DB 덮어쓰기 옵션 설정</li> |
|  정혜인   |   [<img src="https://avatars.githubusercontent.com/u/118713353?v=4" height="100" width="100"> <br/> @hyeinj](https://github.com/hyeinj)   | <ul><li> 작성 예정 </li><li> 작성 예정 </li> |
***

<br>

## 시작가이드

### 환경
* java 17
* Gradle 8.x
* Spring Boot 3.2.x
* MySQL 8.x

<br>

### 실행과정
<pre><code>git clone https://github.com/commonplus/commonplus-back.git
cd commonplus-back
build gradle
gradlew run
</code></pre>
<br>

### 환경변수
> [노션페이지](https://www.notion.so/env-8308e3ffd01843b8a49d9a173452c2a5?pvs=4) 참고

<br>

### 폴더 구조 설명
* address : 외부 쇼핑몰 주소록 관리
* category : 외부 쇼핑몰 카테고리
* cs : 외부 쇼핑몰 고객 문의 관리
* mall : 외부 쇼핑몰 계정 관리
* mallGroup : 외부 상품 등록시 필요한 데이터 관리
* notification : 외부 쇼핑몰 고시정보 관리(11번가)
* order : 외부 쇼핑몰 주문 관리
* product : 등록상품 관리
* shipping : 외부 쇼핑몰 출고지 관리
* shopProduct : 외부 쇼핑몰 상품 등록 관리
* user : 사용자 계정 관리

<br>

### 데이터베이스 설정
<pre><code>create database commonplus character set utf8mb4 collate utf8mb4_general_ci;</code></pre>

<br>

### ERD
<img src="https://github.com/commonplus/commonplus-back/assets/78680486/c0cec1da-f868-4f07-b12a-fd327801eb65">

***
