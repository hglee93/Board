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

**2020.06.13**
- 서버 템플릿 엔진 : mustaeche 엔진 사용
- Layout 방식을 이용하여 프론트 페이지 구성
(Layout방식으로 구성하면 추후 header, footer 코드 변경시, Layout만 변경하면 된다.)
- 외부 CDN 방식을 통해 부트스트랩 라이브러리 사용(실제 서비스에서는 X, 외부 CDN에 의존적이기 때문에)
- 부트 스트랩을 이용해서 프론트 페이지 구성하는 방법 참고하기
- JPA Auditing을 이용하여 객체 생성, 업데이트 시점 자동 로깅
- 위의 시점들이 중요한 이유는 추후 유지보수, 디버깅에 유용하게 사용되기 때문이다
- PostsUpdateRequestDto 추가
- 더티 체킹 : JPA에서 어떻게 쿼리를 생성하지 않고 할 수 있나?
- JPA에서는 특정 Entity가 조회된 시점에서 스냅샷을 남겨, Entity의 상태(Dirty 여부)를 트래킹하여 트랜잭션이 끝나는 시점에서 Update를 한다(JPA에서 쿼리를 생성하여 실행함)
