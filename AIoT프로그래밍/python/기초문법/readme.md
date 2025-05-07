# Python 기초 문법 정리

Python은 간결하고 가독성이 좋은 프로그래밍 언어로, 다양한 분야에서 널리 사용됩니다. 이 문서는 Python의 기본 문법을 간단히 정리한 것입니다.

---

## 1. 변수와 자료형

```python
# 변수 선언
x = 10        # 정수
pi = 3.14     # 실수
name = "Alice" # 문자열
is_valid = True # 불리언
```

- `int`: 정수
- `float`: 실수
- `str`: 문자열
- `bool`: 참/거짓

---

## 2. 출력과 입력

```python
print("Hello, World!")  # 출력
name = input("이름을 입력하세요: ")  # 입력
```

---

## 3. 조건문

```python
age = 20

if age >= 18:
    print("성인입니다.")
elif age >= 13:
    print("청소년입니다.")
else:
    print("어린이입니다.")
```

---

## 4. 반복문

### for 반복문

```python
for i in range(5):  # 0부터 4까지
    print(i)
```

### while 반복문

```python
count = 0
while count < 5:
    print(count)
    count += 1
```

---

## 5. 리스트와 튜플

```python
# 리스트 (수정 가능)
fruits = ["apple", "banana", "cherry"]
fruits.append("orange")

# 튜플 (수정 불가능)
colors = ("red", "green", "blue")
```

---

## 6. 함수

```python
def greet(name):
    print(f"Hello, {name}!")

greet("Alice")
```

---

## 7. 딕셔너리

```python
person = {
    "name": "Alice",
    "age": 25,
    "city": "Seoul"
}

print(person["name"])
```

---

## 8. 예외 처리

```python
try:
    x = int(input("숫자를 입력하세요: "))
    print(10 / x)
except ZeroDivisionError:
    print("0으로 나눌 수 없습니다.")
except ValueError:
    print("유효한 숫자를 입력하세요.")
```

---

## 9. 파일 입출력

```python
# 쓰기
with open("example.txt", "w") as f:
    f.write("Hello, file!")

# 읽기
with open("example.txt", "r") as f:
    content = f.read()
    print(content)
```

---

## 10. 모듈과 라이브러리

```python
import math

print(math.sqrt(16))  # 4.0
```

---

## 마무리

이 문서는 Python의 기초적인 문법을 간단하게 요약한 것입니다. 실제 프로그래밍에서는 연습과 실습을 통해 익숙해지는 것이 중요합니다.

