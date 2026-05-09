# spring-intro-practice
> 인프런 **[스프링 입문 - 코드로 배우는 스프링 부트, 웹 MVC, DB 접근 기술]** 강의 실습 코드 정리  
> 강사: 김영한 | [강의 링크](https://www.inflearn.com/course/%EC%8A%A4%ED%94%84%EB%A7%81-%EC%9E%85%EB%AC%B8-%EC%8A%A4%ED%94%84%EB%A7%81%EB%B6%80%ED%8A%B8)

---

## 개발 환경

- **Java** 17
- **Spring Boot** 3.x
- **Gradle**
- **IntelliJ IDEA**
- **H2 Database**
- **Thymeleaf**

---

## 프로젝트 구조

```
spring-intro-practice/
│
├── src/
│   └── main/
│       ├── java/hello/hellospring/
│       │   ├── HelloSpringApplication.java
│       │   ├── controller/          # 섹션 3, 6 - 웹 MVC
│       │   ├── domain/              # 섹션 4 - 회원 도메인
│       │   ├── repository/          # 섹션 4, 7 - 리포지토리 (Memory → JDBC → JPA → Spring Data JPA)
│       │   ├── service/             # 섹션 4 - 회원 서비스
│       │   └── aop/                 # 섹션 8 - AOP
│       └── resources/
│           ├── static/              # 섹션 3 - 정적 컨텐츠
│           ├── templates/           # 섹션 3, 6 - 타임리프 템플릿
│           └── application.properties
│
├── README.md
└── build.gradle
```

---

## 섹션별 학습 내용

### Section 1. 강의 소개
- 강의 방향성 및 목표 소개

### Section 2. 프로젝트 환경설정
- Spring Initializr로 프로젝트 생성
- 라이브러리 살펴보기 (spring-web, thymeleaf, logging 등)
- View 환경설정
- 빌드하고 실행하기

### Section 3. 스프링 웹 개발 기초
- 정적 컨텐츠
- MVC와 템플릿 엔진
- API 방식 (`@ResponseBody`, JSON 반환)

### Section 4. 회원 관리 예제 - 백엔드 개발
- 비즈니스 요구사항 정리
- 회원 도메인과 리포지토리 만들기
- 회원 리포지토리 테스트 케이스 작성
- 회원 서비스 개발
- 회원 서비스 테스트

### Section 5. 스프링 빈과 의존관계
- 컴포넌트 스캔과 자동 의존관계 설정
- 자바 코드로 직접 스프링 빈 등록하기

### Section 6. 회원 관리 예제 - 웹 MVC 개발
- 회원 웹 기능 - 홈 화면 추가
- 회원 웹 기능 - 등록
- 회원 웹 기능 - 조회

### Section 7. 스프링 DB 접근 기술
- H2 데이터베이스 설치
- 순수 JDBC
- 스프링 통합 테스트
- 스프링 JdbcTemplate
- JPA
- 스프링 데이터 JPA

### Section 8. AOP
- AOP가 필요한 상황
- AOP 적용

### Section 9. 다음으로
- 다음 단계 안내 (스프링 완전 정복 로드맵)

---

## 핵심 개념 정리

- **IoC / DI** : 스프링 컨테이너가 객체 생성·주입 관리
- **컴포넌트 스캔** : `@Component`, `@Service`, `@Repository`, `@Controller`
- **스프링 빈** : 스프링 컨테이너에 등록된 객체
- **OCP** : 개방-폐쇄 원칙 - 기존 코드 변경 없이 구현체 교체 가능
- **AOP** : 공통 관심사(로그, 트랜잭션 등)를 비즈니스 로직에서 분리

---
