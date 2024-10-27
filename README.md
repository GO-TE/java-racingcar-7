# java-racingcar-precourse

## 기능 요구 사항
초간단 자동차 경주 게임을 구현한다.

- 주어진 횟수 동안 n대의 자동차는 전진 또는 멈출 수 있다.
- 각 자동차에 이름을 부여할 수 있다. 전진하는 자동차를 출력할 때 자동차 이름을 같이 출력한다.
- 자동차 이름은 쉼표(,)를 기준으로 구분하며 이름은 5자 이하만 가능하다.
- 사용자는 몇 번의 이동을 할 것인지를 입력할 수 있어야 한다.
- 전진하는 조건은 0에서 9 사이에서 무작위 값을 구한 후 무작위 값이 4 이상일 경우이다.
- 자동차 경주 게임을 완료한 후 누가 우승했는지를 알려준다. 우승자는 한 명 이상일 수 있다.
- 우승자가 여러 명일 경우 쉼표(,)를 이용하여 구분한다.
- 사용자가 잘못된 값을 입력할 경우 `IllegalArgumentException`을 발생시킨 후 애플리케이션은 종료되어야 한다.


## 기능 구현 목록


### 입력
- [X] 자동차의 이름을 받는다.
- [X] 시도할 횟수를 받는다.

### 입력 값 검증
- 자동차 이름 검증
  - [X] 자동차의 이름이 5자 초과한다면 예외 처리
  - [X] 자동차의 이름이 중복된다면 예외 처리
  - [X] 자동차의 이름이 입력되지 않았다면 예외 처리
  - [X] 경주를 해야하니 자동차가 1개만 입력되었다면, 예외 처리

- 시도 횟수 검증
  - [X] 양의 정수가 아니라면 예외 처리
  - [X] int 범위를 벗어난다면 예외 처리

### 출력
- [X] 진행 상황을 출력한다.
- [X] 우승자를 출력한다.

### 자동차
- [X] 자동차의 이름, 엔진을 초기화한다.
- [X] 엔진을 가동시킨다.

### 엔진
- [X] 랜덤한 숫자를 생성해 이동할지 말지 결정한다.

### 심판
- [X] 경기를 진행한다.
- [ ] 우승자를 결정한다.

### 트랙
- [X] 턴마다 자동차의 위치를 전달한다.