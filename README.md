# Board

Spring Boot 스터디 - 스프링 부트와 AWS로 혼자 구현하는 웹 서비스

**2020.06.09**

- HelloController 클래스 추가
- HelloControllerTest 테스트 코드 추가
- lombok 플러그인 추가
- HelloResponseDto 클래스 추가
- HelloResponseDto 테스트 코드 작성
- @RequiredArgsConstructor 사용, final 멤버 변수 초기화
- 위의 상황에서 오류가 발생, 롬북 버전 5 -> 4로 다운그레이드
- @RequiredArgsConstructor는 final 변수를 파라미터로 하는 생성자를 만들어주는 롬복 어노테이션(필수 어노테이션 아님)

**2020.06.11**

- JPA 실습(Posts Entity 클래스, Repository 클래스)
- @builder 어노테이션
- Builder 패턴의 장점 : 생성자를 이용할 때보다 Set하는 필드를 명확히 할 수 있다.
- application.properties 파일에서 옵션을 통해 JPA에서 생성하는 SQL 보기(spring.jpa.show-sql=true)

**2020.06.12**

- 게시글 등록/수정 기능 추가
- Web Layer/Service Layer/Repository Layer의 각 역할
- 도메인 모델
- JPA에서 어떻게 쿼리를 생성하지 않고 할 수 있나?
- 더티 체킹 : JPA에서는 특정 Entity가 조회된 시점에서 스냅샷을 남겨, Entity의 상태(Dirty 여부)를 트래킹하여 트랜잭션이 끝나는 시점에서 Update를 한다(JPA에서 쿼리를 생성하여 실행함)
