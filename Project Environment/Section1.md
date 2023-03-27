# 프로젝트 생성
- 스프링 부트 스타터 https://start.spring.io/
- Maven, Gradle 차이:

# 라이브러리 살펴보기
- 환경 설정이 잘 됐는지, gradlew의 dependencies를 통해 확인 가능

# View 환경 설정
- 정적 = static/
- 동적(서버사이드 렌더링) = templates/

# H2 데이터베이스 설치
- IN Memory DB
- 가볍고 간편, 웹 화면 제공
- 가볍고 편리해서 개인 프로젝트에 용이
- 대규모 프로젝트에서는 안정성 미흡(백업, 복구 기능 부족)

# JPA와 DB설정, 동작확인
- .properties or .yml을 통해 설정, 한 줄이냐, 계층적이냐 차이
- JPA: 자바 ORM API 표준 명세(ORM 사용을 위한 인터페이스 모음)
- EntityManager: JPA 인터페이스의 일부, @Entity 어노테이션을 사용하는 Entity 객체들을 관리(DB와 매핑)
- Hibernate: Java ORM 프레임워크(가장 대중적)
- Junit4: Unit Test 프레임워크

- @RunWith(SpringRunner.class): Junit4에서 지원, @Autowired, @MockBean에 해당하는 것들만 로딩, Jnunit5에서는 @Autowired 사용 x
- @Transactional: Teest 안에서는 Rollback 실행, Rollback(false) 가능

- 모든 로그 출력은 가급적 로거를 통해.
- 쿼리 파라미터를 위해 외부 라이브러리 사용할 경우, 성능테스트 필요
