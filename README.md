# 전도명 이력서

## 📞 Contact  
이메일: domyoung.jeon@gmail.com

Github: https://github.com/D3vJ30n

Project: https://github.com/D3vJ30n/stoblyx-portfolio

Koyeb: https://dry-valli-stoblyx-8abace55.koyeb.app

API 문서화: https://dry-valli-stoblyx-8abace55.koyeb.app/docs/index.html

Blog: https://velog.io/@d3vj30n

Koyeb 무료 플랜의 정책상 서버가 24시간 연속으로 운영되지 않으며, 일정 시간 후 자동으로 슬립 모드로 전환되니 접속이 안되어도 양해 부탁드립니다.

---

## 📌 Introduce  
백엔드 개발자로서 문제 해결에 보람을 느끼며, 사용자 중심의 서비스 개발을 목표로 합니다.  
디자인과 마케팅 경험을 바탕으로 데이터 기반의 의사결정을 중요하게 생각하며, 효율적인 백엔드 시스템 설계에 집중하고 있습니다.  
특히 Java와 Spring Boot를 활용한 안정적인 서비스 개발을 선호하며, 트러블 슈팅은 Velog로 개발 과정은 Github에 기록하고 있습니다.  

---

## 🔨 Skill  
### Backend  
- **Java 17**, **Spring Boot 3.3.9**, **JPA**, **Spring Security**  
  - RESTful API 설계 및 개발  
  - Spring Security를 활용한 인증 및 인가 구현  
  - JPA를 활용한 효율적인 데이터 관리  

### Database  
- **MySQL**, **H2**  
  - 관계형 데이터베이스 모델링 및 최적화  

### Deploy  
- **Docker**, **Koyeb**  
  - Docker 기반의 컨테이너화된 서비스 배포  
  - Koyeb을 활용한 JAR 파일 기반의 백엔드 서비스 배포  

### ETC  
- **Git**, **Github**, **Spring RestDocs**, **Postman**, **Eraser.io**  
  - Git을 활용한 버전 관리 및 협업  
  - Spring RestDocs를 통한 API 문서화  
  - AI를 이용한 시스템 아키텍처 설계  

---

## 📋 Project  

### Stoblyx - AI 기반 독서 숏폼 플랫폼  
**KoBART를 활용한 독서 요약 및 추천 서비스**  
- **기간:** 2025.02 ~ 2025.03
- **기술 스택:** Java 17 / Spring Boot 3.3.9 / JPA / MySQL / H2 / KoBART / pyttsx3 / Docker  
- **주요 개발 사항**  
  - KoBART을 활용한 텍스트 요약 기능 테스트 성공 → 현재 최적화 작업 진행 중
  - 사용자 맞춤형 추천 시스템 설계 완료 → Redis 기반 캐싱 기능 추가 예정
  - pyttsx3 오픈 소스를 활용한 텍스트 TTS 기능 테스트 성공 구현 예정
  - 사용자 맞춤형 추천 시스템 설계 및 구현  
  - Spring Security 기반의 인증 및 인가 시스템 구축  
  - RESTful API 설계를 기반으로 한 확장성 높은 아키텍처 구축  
  - JUnit 및 Mockito를 활용한 단위 테스트와 통합 테스트 진행  
  - Spring RestDocs를 이용한 API 문서화  
  - 협업을 위한 GitHub 프로젝트 관리 및 코드 리뷰 프로세스 정립  
  - Koyeb을 이용한 무중단 배포 및 CI/CD 구축  
  - BGM 기능의 경우 감정과 관련된 단어들을 기쁨, 슬픔, 침착함, 중립으로 나누어 기능 구현(향후 책 내용에 맞는 알맞은 BGM AI 도입 예정)
  - Pexels API 연동 완료 및 책 콘텐츠에 맞는 이미지 및 영상 자동 추천 기능 최적화 작업 진행 중
 
## 주요 해결 사례 요약

프로젝트 개발 과정에서 발생한 다양한 문제와 해결 방법에 대한 자세한 내용은 아래 블로그 포스트에서 확인할 수 있습니다.

[Spring Boot 프로젝트 API 응답 표준화 및 중복 코드 리팩토링](https://buly.kr/7mBCl7Q)

[API 연동, 보안, 트랜잭션, 비동기 처리 등 개발 중 발생한 오류와 해결 과정](https://buly.kr/31SkH68)

[Stoblyx 프로젝트 테스트 코드 오류 해결 및 코드 품질 개선](https://buly.kr/6Mr8ubR)

[Stoblyx 프로젝트 API 통합 테스트 개선 과정에서 마주친 오류와 해결 방법](https://buly.kr/1xyCO7J)

1. JSON 파싱 오류 (ArrayList 생성 실패)

- **문제**: 문자열로 전송된 `genres` 필드를 서버가 배열로 파싱하려고 시도하여 발생한 오류
- **해결**: 클라이언트에서 데이터를 배열 형태로 전송하도록 수정

2. ID 변환 오류 (MethodArgumentTypeMismatchException)

- **문제**: null 값이 Long 타입으로 변환되지 않아 발생한 오류
- **해결**: 테스트에서 고정된 ID 값을 사용하도록 변경

3. 필수 필드 누락 오류

- **문제**: API 요청에 필수 필드가 포함되지 않아 발생한 오류
- **해결**: 요청 데이터에 필수 필드 추가

4. 테스트 간 의존성 문제

- **문제**: 테스트 간 상태 공유로 인한 연쇄 실패
- **해결**: 독립적인 테스트 환경 구성 및 @BeforeEach, @AfterEach를 통한 테스트 데이터 관리

5. REST Docs 테스트 실패

- **문제**: 문서화되지 않은 필드로 인한 테스트 실패
- **해결**: 최대한 relaxedResponseFields 적용하지않고 스키마 불일치 문제여서 스키마 수정하여 문서화 구현

6. 데이터베이스 스키마 관련 오류

- **문제**: 시퀀스 테이블 관련 SQL 문법 오류
- **해결**: Hibernate 설정 변경 및 SQL 초기화 모드 조정

7. 코드 품질 개선

- **문제**: 사용되지 않는 변수, 불필요한 메서드 호출 등으로 인한 정적 분석 도구 경고
- **해결**: 미사용 변수 제거, 불필요한 eq() 메서드 호출 제거 등 코드 정리

8. 보안 관련 이슈

- **문제**: 리플렉션을 사용한 접근 제한 우회로 인한 보안 취약점
- **해결**: 적절한 setter 메서드 추가 및 리플렉션 코드 제거

9. 데이터베이스 방언 차이 문제

- **문제**: H2 데이터베이스와 MySQL 간의 SQL 함수 차이
- **해결**: 데이터베이스에 독립적인 JPQL 쿼리 사용

10. 인증 관련 테스트 실패

- **문제**: 인증이 필요한 API에 대한 테스트 실패
- **해결**: 테스트 환경에서 인증을 우회하는 SecurityTestConfig 구현

11. 메서드 복잡도 문제

- **문제**: 메서드의 인지적 복잡도가 허용 수준을 초과
- **해결**: 메서드를 여러 작은 메서드로 분리하여 단일 책임 원칙 준수

12. API 통합 테스트 환경 구성 문제

- **문제**: 실제 서비스와 유사한 환경에서의 통합 테스트 실행 어려움
- **해결**: RestAssured와 ExtentReports를 활용한 통합 테스트 프레임워크 구축

13. 응답 상태 코드 불일치

- **문제**: 예상한 상태 코드(401)와 실제 반환된 상태 코드(403) 불일치
- **해결**: Spring Security 설정에 맞게 테스트 코드의 예상 값 조정

14. 500 Internal Server Error (내부 서버 오류) 해결

**문제**
- 외부 API(Pexels) 호출 시 타임아웃이나 응답 오류 처리가 미흡
- 예외 처리가 되지 않은 부분에서 NPE(NullPointerException)가 발생
- 트랜잭션 관리가 제대로 되지 않아 데이터 무결성 문제가 발생

**해결**
- 모든 외부 API 호출에 폴백 메커니즘을 구현하여 API 실패 시에도 서비스가 계속 동작하도록 함
- GlobalExceptionHandler를 구현하여 모든 예외를 적절히 처리하고 표준화된 응답 형식으로 반환
- 트랜잭션 범위를 조정하고 @Transactional 어노테이션의 propagation 속성을 적절히 설정

14. 빈 의존성 주입 오류 해결

**문제**
- 순환 참조(circular dependency) 문제가 발생했습니다.
- 컴포넌트 스캔 범위가 잘못 설정되어 일부 빈이 등록되지 않았습니다.
- 테스트 환경에서 필요한 빈이 모킹되지 않았습니다.

**해결**
- 순환 참조를 해결하기 위해 설계를 수정하고 필요한 경우 @Lazy 어노테이션을 활용
- @ComponentScan 설정을 올바르게 수정하고 누락된 @Service, @Repository 어노테이션을 추가
- 테스트 클래스에 @MockBean과 @SpyBean을 올바르게 사용하여 의존성을 모킹
- 일부 의존성 주입 방식을 필드 주입에서 생성자 주입으로 변경하여 명시적으로 의존성 관리

15. 스키마 불일치 오류 해결

**문제**
- JPA 엔티티와 실제 데이터베이스 스키마 간의 불일치
- REST Docs 테스트 시 API 문서화 필드와 실제 응답 필드 불일치
- DTO와 엔티티 간 변환 과정에서 필드명이나 타입 불일치

**해결**
- 엔티티 클래스의 필드 정의를 데이터베이스 스키마와 일치하도록 수정
- Hibernate의 ddl-auto 옵션을 'validate'로 설정하여 애플리케이션 시작 시 스키마 검증을 수행
- REST Docs 테스트에서 relaxed 모드를 최소화하고 필드를 명확히 문서화
- MapStruct를 활용하여 DTO와 엔티티 간 일관된 매핑 규칙을 정의

이러한 오류들을 해결함으로써 애플리케이션의 안정성과 신뢰성이 크게 향상되었으며, 개발 및 테스트 과정이 더욱 효율적으로 진행될 수 있었습니다. 특히 외부 API 의존성이 높은 서비스에서 폴백 메커니즘 구현은 서비스 가용성을 크게 개선했습니다.

이러한 문제 해결 과정을 통해 더 안정적이고 유지보수하기 쉬운 코드베이스를 구축할 수 있었습니다.
 
## 성능 최적화

1. 캐싱 전략

- @Cacheable 적용: 자주 접근하는 데이터에 Spring Cache 적용

2. 데이터베이스 최적화

- 인덱싱: 자주 조회되는 필드에 인덱스 적용
- 페이징 처리: 대용량 데이터 조회 시 페이징 적용
- N+1 문제 해결: @EntityGraph 사용으로 연관 엔티티 조회 최적화

3. API 요청 제한

- Rate Limiting: 사용자별 API 요청 제한 구현

## 테스트 전략

프로젝트의 테스트 전략은 효율성과 실용성을 중시하여 기존 테스트 피라미드 개념을 컨트롤러 테스트와 k6 테스트의 조합으로 재구성하였습니다.

1. 단위 테스트 (Unit Test)

- **컨트롤러 테스트가 대체**
  - 컨트롤러 메소드별 격리된 테스트
  - 서비스 레이어 모킹으로 비즈니스 로직 분리
  - 요청/응답 구조 검증으로 API 계약 테스트

2. 통합 테스트 (Integration Test)

- **컨트롤러 테스트 + k6 테스트로 대체**
  - 컨트롤러 테스트: Spring Security, 필터 등 통합
  - k6 테스트: 실제 DB 연동, 외부 API 연동 검증

3. E2E 테스트 (End-to-End Test)

- **k6 테스트가 완벽히 대체**
  - 실제 애플리케이션 환경에서 전체 흐름 테스트
  - 사용자 시나리오 기반 테스트
  - 성능/부하 테스트 병행 가능

4. 장점

- **효율성**: 적은 코드로 넓은 테스트 범위 커버
- **실용성**: 실제 프로젝트에서도 많이 사용하는 방식
- **가시성**: 테스트 결과를 시각적으로 확인 가능

이런 접근법은 시간 효율성과 테스트 효과 측면에서 균형을 잡으려 위와 같은 방식으로 테스트를 진행하였습니다.

---

## ✒️ Experience  

### 베플 (2023.06 ~ 2023.12, 7개월)  
**마케팅 프리랜서**  
- SEO 최적화 및 검색 광고 운영  
- 베플 앱 관련 콘텐츠 업로드 및 마케팅 전략 수립  

### 일분육십초 (2019.08 ~ 2022.12, 3년 5개월)  
**대표 (개인 사업)**  
- 인테리어 소품 판매 및 바이럴 마케팅 운영  
- 데이터 분석을 기반으로 마케팅 전략 최적화  

---

## 🎓 Education  

### 한국외국어대학교 경영대학원 (2023.03 ~ 2025.02)  
**Business & Finance MBA**  

---

## 🔎 Additional Information  

### TIL (Today I Learned)  
- Spring Boot, Database 설계, Docker 기반 배포, CI/CD 구축 등 실무에서 필요한 백엔드 개발 지식을 정리
  
🔎 [Github Repository](https://github.com/D3vJ30n/be-dev)
