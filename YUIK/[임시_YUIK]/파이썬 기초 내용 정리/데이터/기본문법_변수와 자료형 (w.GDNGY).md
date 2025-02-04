![wjdqlswh 파이썬](https://github.com/user-attachments/assets/48ab558d-7aa7-4bfa-b377-61fc277d3ac1)

# 변수와 자료형 
### 정수형, 실수형, 자료형
- <b>정수형(int)</b>: 정수를 저장하는 자료형
- <b>실수형(float)</b>: 소수점이 있는 숫자를 저장하는 자료형
- <b>문자열(str)</b>: 문자나 문자의 집합을 저장하는 자료형
  - 파이썬에서 변수는 값을 저장하는 공간으로, 변수에 자료형을 별도로 명시하지 않아도 됨.
  - 문자열의 경우
    - 작은 따옴표('') 또는 큰 따옴표("")를 사용하여 표현할 수 있으며, 여러 줄의 문자열의 삼중 따옴표(''') 또는 (""")를 사용함.
      <br/>
      또한, 문자열의 연산을 통해 문자열을 결합하거나 반복할 수 있다.

#### 예제코드 
```
# 정수형 변수
num1 = 10 // num1이라는 정수형 변수를 만들고, 값과 자료형을 출력
// type(num1)은 num1의 자료형을 알려줌
print(f"num1: {num1}, type: {type(num1)}") 

# 실수형 변수
num2 = 3.14 // num2라는 실수형 변수를 만들고, 동일하게 값과 자료형을 출력
print(f"num2: {num2}, type: {type(num2)}")

# 문자열 변수
num3 = "Hello, World!" // num3라는 문자열 변수를 만들고, 이거 역시 동일하게 값과 자료형 출력
// greeting 변수가 없어서 에러가 발생할 수 있음! (실제로 num3를 직접 출력하거나 greeting = "" 처럼 변수를 맞추면 사용이 가능하다)
print(f"greeting: {greeting}, type: {type(num3)}")

# 여러 줄의 문자열
multiline = '''파이썬 // 작은따옴표 세 개(''')를 사용하면 여러 줄로 된 문자열을 쉽게 담을 수 있음.
프로그래밍 
환영합니다.'''
print(multiline) // 출력하면 엔터(줄바꿈)도 그대로 표현된다

# 문자열 연산
name = "홍길동"
message = "안녕하세요, " + name + "님!" // + 연산자를 이용하면 문자열끼리 이어 붙일 수 있음
print(message) // 결과 => "안녕하세요, 홍길동님!" 문자열 완성
```
### 복소수 (Complex) 주요 특징 및 사용법
1. 복소수 생성
   - 복소수는 a + b; 형태로 나타내며, 여기서 a는 실수 부분이고 b는 허수 부분입니다. (j는 허수 단위를 나타낸다.)
   - 복소수 생성하는 방법 (두가지)
     - complex(a, b)를 사용하여 a + b; 복소수를 생성
     - 직접 a + b; 형태로 입력
       ```
       z1 = complex(3, 4) # 3 + 4;
       z2 = 3 + 4; # 3 + 4;
       ```
3. 복소수의 속성

### 핵심 포인트 정리
- <b>변수(Variable)</b>: 데이터를 저장하는 공간(num1, num2, ...등)
- <b>자료형(Type)</b>: 정수(int), 실수(float), 문자열(str) 등 어떤 종류의 데이터인가를 나타내는 것
- <b>출력(print 함수)</b>: print() 안에 변수나 문자열을 넣어 콘솔에 보여줌
- <b>문자열 연산</b>: + 연산자로 문자열을 이어 붙이거나, f"..."방식을 쓰면 {변수}처럼 변수를 간단히 포함할 수 있다.
- <b>여러 줄 문자열</b>: '''...''' 또는 """..."""를 쓰면 편하게 여러 줄을 표현할 수 있음

### 추가적으로, ```NameError: name 'greeting' is not defined```의 경우
- <b>NameError</b>: 정의되지 않은 (또는 선언되지 않은)변수를 사용하려 할 때 발생하는 에러
  - 코드 예시 (올바른 변수 선언)
    ```
    # 문자열 변수
    greeting = "Hello, World!" # 여기에 greeting 변수를 선언해줍니다.
    print(f"greeing: {greeting}, type: {type(greeting)}")
    ```
    - greeting 변수를 먼저 선언하였기 때문에, print 구문에서 greeting을 문제없이 사용할 수 있음
      
  - 코드 예시 (올바르지 않은 변수 선언)
    ```
    print(f"greeing: {greeting}, type: {type(greeting)}")
    greeting = "Hello, World!" # 여기에 greeting 변수를 선언해줍니다.
    ```

### 정리
- <b>NameError</b>: 정의(선언)되지 않은 변수를 참조할 때 발생하는 에러
- 해결 방법
  - 변수르 사용하기 전에 반드시 선언해야 함.
  - 코드에서 변수가 쓰이는 순서를 체크하며 선언해야 하고, 사용 순으로 두면 문제를 해결할 수 있음

# 블로그 참조
- https://gdngy.tistory.com/74 (GDNDY님 티스토리)
https://sosodev.tistory.com/entry/Python-complex-%ED%81%B4%EB%9E%99%EC%8A%A4%EB%A5%BC-%EC%82%AC%EC%9A%A9%ED%95%B4%EC%84%9C-%EB%B3%B5%EC%86%8C%EC%88%98-%EB%8B%A4%EB%A3%A8%EA%B8%B0
