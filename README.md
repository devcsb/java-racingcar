# 자동차 경주 게임
## 진행 방법
* 자동차 경주 게임 요구사항을 파악한다.
* 요구사항에 대한 구현을 완료한 후 자신의 github 아이디에 해당하는 브랜치에 Pull Request(이하 PR)를 통해 코드 리뷰 요청을 한다.
* 코드 리뷰 피드백에 대한 개선 작업을 하고 다시 PUSH한다.
* 모든 피드백을 완료하면 다음 단계를 도전하고 앞의 과정을 반복한다.

## 3단계 - 자동차 경주 기능 요구사항
- 사용자는 경주에 참여할 자동차 대수와 주행 시도 횟수를 입력할 수 있다.
- 각 자동차는 전진 시도 시, 생성된 random 값이 4 이상일 경우에만 전진한다.
- 자동차의 주행 상태를 화면에 출력한다. 출력시점에 대한 제약은 없다.
### 테스트 케이스 정리
- [x] 입력받은 값으로 차를 만들 수 있다.
- [x] 자동차는 한 번의 주행 시도 시, random 값이 4 이상 일 때, 전진한다.
- [x] 자동차는 한 번의 주행 시도 시, random 값이 4미만일 때, 멈춘다.
- [ ] 경주에 참여하는 자동차는 최대 1대 이상이다.
- [ ] 하나의 경주는 최소 1회 이상의 주행 시도를 한다.
- [ ] 한 번의 주행이 끝난 다음 자동차의 주행 상태를 저장한다.
- [ ] 경기에서 누적된 주행 결과를 저장한다.
- [ ] 경기 실행 결과를 문자열로 출력한다.

## 문자열 계산기 테스트 케이스
- [x] null 또는 빈문자열 입력 시, 0을 반환한다.
- [x] 숫자 하나를 전달하면 값을 그대로 반환한다.
- [x] 여러 숫자를 기본 구분자(, 또는 :)와 함께 전달하면, 구분자로 구분된 숫자의 총합을 반환한다. (예: “” => 0, "1,2" => 3, "1,2,3" =>6, “1,2:3” => 6)
- [x] 문자열 앞부분에 “//”와 “\n” 사이에 위치하는 문자를 지정하면, 기본 구분자가 아닌 정의한 커스텀 구분자로 동일한 계산 결괏값을 얻을 수 있다.
- [x] 문자열 계산기에 숫자 이외의 값 또는 음수를 전달하는 경우 RuntimeException 예외를 throw한다.