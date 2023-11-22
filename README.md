# Tasty Code

### 3조 묵찌빠 프로젝트 저장소

#### 팀원
- 동대문 1기 🤖 홍, 📸 폴

#### Step 1 가위, 바위, 보 게임 구현 (23.11.20 ~ 23.11.22)

문구의 안내에 따라 플레이어가 입력한 숫자 `String` 값을 `readLine()`으로 입력받습니다.

입력받은 숫자 `String`값을 `Selection` 열거형을 통해 `Selection`열거형의 값을 인자로 받는 `handleSelection(_ enumValue: Selection)`에 입력할 `case`로 치환합니다.

`handleSelection` 함수는 열거형을 통해 치환된 case에 따라 `runningGame(_ myChoice: Int)`함수에 `Int`값 전달합니다.

`Int`값 0은 runningGame의 프로그램 종료 코드로 연결되고, 1~3은 각각 가위, 바위, 보를 의미하게 됩니다. 

`runningGame`함수는 전달받은 `Int`값을 myChoice, 즉 플레이어의 선택에 할당하고, `comChoice` 즉 컴퓨터의 선택을 `Int.Random(in: 1…3)`으로 무작위 할당합니다.

그 후, `comChoice`와 `myChoice`의 값에 따라 가위바위보 게임 로직을 실행 후 적절한 문구를 출력하거나 프로그램을 종료합니다.
