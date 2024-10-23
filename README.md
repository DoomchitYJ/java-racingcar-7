# java-racingcar-precourse

# 예상 시나리오

1. 자동차 이름을 입력한다.
2. 시도 횟수를 입력한다.
3. 전진 혹은 정지를 결정한다.
4. 해당 차수의 실행 결과를 출력한다.
5. 시도 횟수만큼 3-4를 반복한다.
6. 우승자를 선정한다.
7. 우승자를 출력한다.

### 예외 처리

1. 2대 이하의 자동차 이름을 입력한다.
2. 5자 초과의 이름을 입력한다.
3. 중복 이름을 입력한다.
4. 시도 횟수로 0 이하의 값을 입력한다.

# 구현 기능 목록

### 자동차 이름을 입력받는 기능

- [x]  “경주할 자동차 이름을 입력하세요.(이름은 쉼표(,) 기준으로 구분)” 를 출력한다.
- [x]  문자열을 입력받는다.
- [x]  이름을 파싱한다.
- [ ]  입력을 검증한다.
    - [ ]  쉼표로 구분했을 때 이름이 5자 이하인가?
    - [ ]  2대 이상의 자동차 이름이 입력되었는가?
    - [ ]  중복된 이름이 있는가?

### 시도할 횟수를 입력받는 기능

- [x]  “시도할 횟수는 몇 회인가요?” 를 출력한다.
- [x]  숫자를 입력받는다.
- [ ]  입력을 검증한다.
    - [ ]  양수가 입력되었는가?

### 입력받은 이름을 할당한 자동차 객체를 생성하는 기능

- [x]  자동차 객체를 생성한다.
- [x]  이름을 저장한다.
- [ ]  경주에서 승리한 횟수를 저장한다.

### 아래 두 기능을 입력받은 횟수만큼 반복한다.

### 해당 차례에서 전진 조건을 만족하는지 확인하는 기능

- [ ]  각 자동차별로 무작위 값(0 ~ 9)을 추출한다.
- [ ]  무작위 값이 4 이상일 경우 승리 횟수에 1을 더한다.

### 실행 결과를 출력하는 기능

- [ ]  차수별로 실행 결과를 출력한다.
    - [ ]  “자동차 이름 : - ” 를 출력한다. (’-’는 해당 차수까지 전진한 횟수만큼)


### 우승자를 출력하는 기능

- [ ]  승리 횟수가 가장 높은 자동차를 최종 우승자로 선정한다.
- [ ]  “최종 우승자 : 자동차 이름” 을 출력한다.
    - [ ]  단독 우승일 경우, 자동차 이름 한 대만 출력한다.
    - [ ]  공동 우승일 경우, 쉼표로 구분하여 출력한다. (ex. 최종 우승자 : abc, def)

# 고려할 점

1. 이름 사이에 공백이 있어도 되는가?
    - O. 쉼표(,)로만 구분되게 구현한다.
2. 이름에 숫자나 특수문자가 포함되어도 되는가?
    - O. 쉼표(,)로만 구분되게 구현한다.
3. 이름이 중복되어도 되는가?
    - X. 구분을 위해 중복 불가로 구현한다.