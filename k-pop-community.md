# k-pop-community 프로젝트 
## 2023. 08. 22 
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
* Java 17
* Spring Boot 2.xx
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
