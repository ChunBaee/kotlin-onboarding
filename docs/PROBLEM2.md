## 🚀 기능 요구 사항

암호문을 좋아하는 괴짜 개발자 브라운이 이번에는 중복 문자를 이용한 새로운 암호를 만들었다. 예를 들어 "browoanoommnaon"이라는 암호문은 다음과 같은 순서로 해독할 수 있다.

1. "browoanoommnaon"
2. "browoannaon"
3. "browoaaon"
4. "browoon"
5. "brown"

임의의 문자열 cryptogram이 매개변수로 주어질 때, 연속하는 중복 문자들을 삭제한 결과를 return 하도록 solution 함수를 완성하라.

### 제한사항

- cryptogram은 길이가 1 이상 1000 이하인 문자열이다.
- cryptogram은 알파벳 소문자로만 이루어져 있다.

### 실행 결과 예시

| cryptogram | result |
| --- | --- |
| "browoanoommnaon" | "brown" |
| "zyelleyz" | "" |

### 기능 목록
1. 문자를 각 자리별로 비교하기 쉽게 배열로 변환하기.
2. 해당 배열 내에 연달아 있는 중복값이 있는지 판별하기.
3. 중복값이 있다면 해당 위치에 있는 중복값들 제거하기.
4. 더이상 중복이 없을 때 까지 2~3 과정을 반복하기.
5. 더이상 중복이 없다면 배열을 다시 문자열로 바꾸기.