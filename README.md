# spring-security-study

Spring Security의 핵심 개념과 인증/인가 흐름을 학습하기 위해 만든  
**Spring Boot 기반 Security 실습 프로젝트**입니다.  
JWT 기반 인증 방식을 직접 구현하며 보안 동작 원리를 이해하는 것을 목표로 합니다.

---

## 학습 목적

- Spring Security 기본 구조 이해
- Security Filter Chain 동작 방식 학습
- 인증(Authentication)과 인가(Authorization) 흐름 이해
- JWT 기반 Stateless 인증 방식 구현
- 테스트 환경에서의 Security 검증

---

## 기술 스택

### Backend

- **Java:** 21  
- **Spring Boot:** 3.2.2  
- **Spring Security**
- **Spring Data JPA**
- **Build Tool:** Gradle  

### Database

- **H2 Database** (In-Memory)

### Authentication

- **JWT (JSON Web Token)**

### Validation / Test

- **Spring Validation**
- **Spring Security Test**
- **JUnit 5**

---

## 주요 학습 내용

### Spring Security

- `SecurityFilterChain` 설정
- 인증 / 인가 분리 설계
- `UsernamePasswordAuthenticationFilter` 동작 이해
- 커스텀 인증 로직 구현

---

### JWT 인증 흐름

1. 사용자 로그인 요청
2. 사용자 정보 검증
3. JWT Access Token 발급
4. 이후 요청 시 Authorization Header에 토큰 전달
5. 토큰 검증 후 SecurityContext에 인증 정보 저장
6. 권한에 따른 API 접근 제어

---
