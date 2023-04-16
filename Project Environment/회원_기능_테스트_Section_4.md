# @RunsWith(SpringRunner.class)

# @SpringBootTest

# @Transactional

# @Test(expected_
# 테스트 케이스

## 작성법(Recommend)
- Given: Input Data
- When: Action
- Then: Result
## 설정
메모리 DB를 사용하는 것이 이상적: 격리된 환경, 데이터 초기화
우영 환경과 스프링 환경이 다르므로 설정 파일을 다르게 사용
- ***main***/resources/application.yml
- ***test***/resources/application.yml
- 스프링 부트는 기본적으로 메모리 DB를 사용하므로 JPA 관련 별도 추가 설정 하지 않아도 된다.
