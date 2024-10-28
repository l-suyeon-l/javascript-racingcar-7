# javascript-racingcar-precourse : l-suyeon-l
### 기능 요구 사항
초간단 자동차 경주 게임을 구현한다.

- 주어진 횟수 동안 n대의 자동차는 전진 또는 멈출 수 있다.
- 각 자동차에 이름을 부여할 수 있다. 전진하는 자동차를 출력할 때 자동차 이름을 같이 출력한다.
- 자동차 이름은 쉼표(,)를 기준으로 구분하며 이름은 5자 이하만 가능하다.
- 사용자는 몇 번의 이동을 할 것인지를 입력할 수 있어야 한다.
- 전진하는 조건은 0에서 9 사이에서 무작위 값을 구한 후 무작위 값이 4 이상일 경우이다.
- 자동차 경주 게임을 완료한 후 누가 우승했는지를 알려준다. 우승자는 한 명 이상일 수 있다.
- 우승자가 여러 명일 경우 쉼표(,)를 이용하여 구분한다.
- 사용자가 잘못된 값을 입력할 경우 "[ERROR]"로 시작하는 메시지와 함께 Error를 발생시킨 후 애플리케이션은 종료되어야 한다.

<br>

### 입출력 요구 사항
**입력**
- 경주할 자동차 이름(이름은 쉼표(,) 기준으로 구분)
```
pobi,woni,jun
```

- 시도할 횟수
```
5
```

**출력**
- 차수별 실행 결과
```
pobi : --
woni : ----
jun : ---
```

- 단독 우승자 안내 문구
```
최종 우승자 : pobi
```

- 공동 우승자 안내 문구
```
최종 우승자 : pobi, jun
```

- 실행 결과 예시
```
경주할 자동차 이름을 입력하세요.(이름은 쉼표(,) 기준으로 구분)
pobi,woni,jun
시도할 횟수는 몇 회인가요?
5

실행 결과
pobi : -
woni : 
jun : -

pobi : --
woni : -
jun : --

pobi : ---
woni : --
jun : ---

pobi : ----
woni : ---
jun : ----

pobi : -----
woni : ----
jun : -----

최종 우승자 : pobi, jun
```
<br>

### 구현 기능 목록
1. "경주할 자동차 이름을 입력하세요.(이름은 쉼표(,) 기준으로 구분)" 출력과 동시에 문자열 입력받기
2. "시도할 횟수는 몇 회인가요?" 출력과 동시에 문자열 입력받기
3. 자동차 이름 쉼표(,) 기준으로 구분하기
4. 자동차 이름이 5자를 초과하면 Error 발생
5. 시도할 횟수만큼 각 자동차 전진 반복
6. 무작위 값이 4 이상일 경우 자동차 전진
7. 최종적으로 전진한 자동차 결과 출력
8. 최종 우승자 출력
