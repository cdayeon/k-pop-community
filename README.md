# SpringBoot 프로젝트 생성
### 사전 준비물
* Java 11 설치 (Java 11이 Springframework의 프로젝트를 생성할 때도 오류없이 잘 작동한다.)
* IDE : IntelliJ 또는 Eclipse 설치 (실무에서 Eclipse는 많이 사용하지 않는 편, 필자는 IntelliJ 사용)
------
## IntilliJ 설치 (ver.mac)
#### (1) https://www.jetbrains.com/idea/ IntelliJ 사이트로 이동해서 다운로드 클릭
<img width="1415" alt="스크린샷 2023-08-07 오후 2 20 10" src="https://github.com/cdayeon/SpringBoot/assets/119835857/ee14b06b-06e9-49ec-9a6b-eacdb1a1ac7e">

#### (2) Ultimate는 유료버전, Community Edition은 무료버전이다. (필자는 Community Edition 선택)
#### (3) 맥 인텔은 **.dmg(Intel)** 로, 맥 m1,m2는 **.dmg(Apple Silicon)** 으로 다운 (필자는 인텔이어서 .dmg(Intel)로 다운)
<img width="1415" alt="스크린샷 2023-08-07 오후 2 22 04" src="https://github.com/cdayeon/SpringBoot/assets/119835857/d1ad8f32-05eb-4ffa-9de3-7550d4801d2a">

#### (4) 다운로드를 받은 파일을 실행시켜 Applications로 드래그해주면 설치 완료
<img width="446" alt="스크린샷 2023-08-07 오후 2 30 41" src="https://github.com/cdayeon/SpringBoot/assets/119835857/32fd8bfd-6519-42e2-ac68-362f31250c7d">

#### (5) 설치된 IntelliJ를 실행하면 팝업이 뜨는데 **열기** 클릭
<img width="446" alt="스크린샷 2023-08-07 오후 2 33 17" src="https://github.com/cdayeon/SpringBoot/assets/119835857/4a4c23fa-a998-4922-a616-c3b7c0a16aa1">

#### (6) IntelliJ가 실행되고 사용자 동의 팝업 **체크** 하고 **continue** 클릭
<img width="600" alt="스크린샷 2023-08-07 오후 2 35 23" src="https://github.com/cdayeon/SpringBoot/assets/119835857/8ff0e6db-f92c-4a1d-966c-c50a8c1bb399">

#### (7) Data Sharing 은 하지 않아도 될 것 같아 **Don't Send** 클릭
<img width="595" alt="스크린샷 2023-08-07 오후 2 35 38" src="https://github.com/cdayeon/SpringBoot/assets/119835857/9054bd93-836e-427b-a923-4de1f7ddfae4">

#### (8) 해당 화면이 뜨면 IntelliJ설치 완료
<img width="593" alt="스크린샷 2023-08-07 오후 2 35 56" src="https://github.com/cdayeon/SpringBoot/assets/119835857/a0dcd130-be25-4d32-98c8-0689dc06bcc6">
------

## SpringBoot 프로젝트 생성 시작 
#### (1) https://start.spring.io 스프링 부트 스타터 사이트로 이동해서 스프링 프로젝트 생성
#### (2) spring Initializr 라는 사이트로 이동
<img width="1270" alt="스크린샷 2023-08-07 오후 2 49 24" src="https://github.com/cdayeon/SpringBoot/assets/119835857/4b6ecdde-bcc8-42eb-88de-419b699ee429">

#### (3) Project에서 **Gradle - Groovy** 선택 (현재 실무에서는 Maven에서 Gradle로 넘어오는 추세라고 한다.)
#### (4) Language는 **Java** 선택
#### (5) Spring Boot 버전은 2.7.14 버전 선택 (Java 11과 오류없이 연동하기 위해서는 2.x.x버전이 좋다. SNAPSHOT 또는 M1이라고 적혀있는 버전들은 사용하기에는 불안정하다.)
#### (6) Project Metadata에서 Group, Artifact, Packaging, Java만 변경해주었다. (보통 Group에는 기업 도메인명을 적어준다고 한다. Artifact 프로젝트명 이라고 생각하면 된다.)
#### (7) Packaging은 **Jar** 선택, Java는 **11** 선택
#### (8) Dependencies는 내가 사용할 라이브러리를 추가할 수 있다.
#### (9) **ADD DEPENDENCIES** 를 클릭해여, **Spring Web** 과 **Thymeleaf**만 추가해주었다.
#### (10) 최종적으로 **GENERATE** 를 누르면 다운로드를 받게 된다.
