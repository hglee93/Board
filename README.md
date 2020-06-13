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
