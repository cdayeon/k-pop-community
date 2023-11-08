# SpringBoot 프로젝트 생성
### 사전 준비물
* Java 17 또는 Java 11 설치 (필자는 Java17 설치)
* IDE : IntelliJ 또는 Eclipse 설치 (실무에서 Eclipse는 많이 사용하지 않는 편, 필자는 IntelliJ 사용)
------
## IntilliJ 설치 (ver.mac)
1. https://www.jetbrains.com/idea/ IntelliJ 사이트로 이동해서 다운로드 클릭
<img width="1415" alt="스크린샷 2023-08-07 오후 2 20 10" src="https://github.com/cdayeon/SpringBoot/assets/119835857/ee14b06b-06e9-49ec-9a6b-eacdb1a1ac7e">

2. Ultimate는 유료버전, Community Edition은 무료버전이다. (필자는 Ultimate 선택 -> 대학생 인증받아서 Ultimate이지만 무료로 사용중)
3. 맥 인텔은 **.dmg(Intel)** 로, 맥 m1,m2는 **.dmg(Apple Silicon)** 으로 다운 (필자는 인텔이어서 .dmg(Intel)로 다운)
<img width="1415" alt="스크린샷 2023-08-07 오후 2 22 04" src="https://github.com/cdayeon/SpringBoot/assets/119835857/d1ad8f32-05eb-4ffa-9de3-7550d4801d2a">

4. 다운로드를 받은 파일을 실행시켜 Applications로 드래그해주면 설치 완료
<img width="446" alt="스크린샷 2023-08-07 오후 2 30 41" src="https://github.com/cdayeon/SpringBoot/assets/119835857/32fd8bfd-6519-42e2-ac68-362f31250c7d">

5. 설치된 IntelliJ를 실행하면 팝업이 뜨는데 **열기** 클릭
<img width="446" alt="스크린샷 2023-08-07 오후 2 33 17" src="https://github.com/cdayeon/SpringBoot/assets/119835857/4a4c23fa-a998-4922-a616-c3b7c0a16aa1">

6. IntelliJ가 실행되고 사용자 동의 팝업 **체크** 하고 **continue** 클릭
<img width="600" alt="스크린샷 2023-08-07 오후 2 35 23" src="https://github.com/cdayeon/SpringBoot/assets/119835857/8ff0e6db-f92c-4a1d-966c-c50a8c1bb399">

7. Data Sharing 은 하지 않아도 될 것 같아 **Don't Send** 클릭
<img width="595" alt="스크린샷 2023-08-07 오후 2 35 38" src="https://github.com/cdayeon/SpringBoot/assets/119835857/9054bd93-836e-427b-a923-4de1f7ddfae4">

8. 해당 화면이 뜨면 IntelliJ설치 완료
<img width="593" alt="스크린샷 2023-08-07 오후 2 35 56" src="https://github.com/cdayeon/SpringBoot/assets/119835857/a0dcd130-be25-4d32-98c8-0689dc06bcc6">
------
# SpringBoot 프로젝트 
## 2023. 08. 22 ~ 23 회의록
### 1. 개발 기획
#### * 기획 목표
##### K-POP 기업에서 굿즈 스토어를 운영하는 경우가 있지만 아이돌 시장의 경우에는 개인이 굿즈를 제작해서 판매하는 경우가 많다. 또한, 아이돌의 생일이나 콜라보 카페 등을 탐색하는 방법이 굉장히 불편한 경우가 많다. 지도로 하나하나 찾는 일이 쉽지 않다. 또한 트위터나 인스타그램 등 SNS에서 접근하기에는 불편한 감이 있기 때문에 굿즈 스토어를 직접 만들어 플랫폼을 통일해보자는 목표를 가지고 시작하게 되었다.
------

### 2. 요구 사항
#### * 회원 관련 기능
* 로그인
* 소셜로그인 OAuth
* 회원가입
* 로그아웃
* 회원정보 수정
* 회원 탈퇴
* 프로필 관리(닉네임, 프로필 이미지 등)
* 찜 목록(굿즈, 장소는 각각 별개로)
* 내가 판매한 상품 목록
* 내가 구매한 상품 목록
* 관심사
* 유저 팔로우 기능

#### * 굿즈 관련 기능
* 굿즈 수요조사 폼
* 필터링
* 등록
* 판매
* 구매창
* 굿즈 판매 시 대화가능한 채팅 또는 댓글형식
* 결제 기능
* 외부사이트 연결(출처 기입)

#### * 지도 관련 기능
* 지도 api 사용해 지도에 장소 표기
* 장소 등록
* 장소 세분화(인물 혹은 지역에 따라)
* 장소 검색

#### * Admin 기능
* 유저 관리
* 굿즈 장르별 데이터 정리
* 그룹 관리(생성 및 정보 수정)(그래프)
------

### 3. 기술 스택
#### * BackEnd
* Java 11 or Java 17
* Spring Boot 3
* Spring Security
* JWT
* Lombock
* Swagger/Postman/Scratch
* JPA
* OAuth
* DB
  * RDBMS - MYSQL(AWS RDS)
  * GraphDB - Neo4j/Amazon Neptune
  * NoSQL(K/V) - Redis
  * Bucket - Amazon S3(Simple Storage Service)
* Python
  * selenium, BeautifulSoup
 
#### * FrontEnd
* NEXT.JS 13
* React 18
* Typescript
* SWR
* Vercel
* Websocket

#### * Deploy
* GitHub
* Jenkins
* AWS

#### * Communication
* Discord
* Notion
* GitHub

#### * API
* GoogleMap API
* iamport API
* MailGun
