# NumPy 기초 정리

`NumPy`(Numerical Python)는 Python에서 **수치 계산과 과학 계산**을 위한 핵심 라이브러리입니다.  
다차원 배열 처리, 선형대수, 통계 계산, 난수 생성 등을 빠르고 효율적으로 수행할 수 있습니다.

---

## 📌 NumPy의 주요 특징

| 특징 | 설명 |
|------|------|
| 다차원 배열 객체 (`ndarray`) | 리스트보다 메모리 효율적이고 빠름 |
| 벡터화 연산 | 반복문 없이 빠르게 연산 가능 |
| 브로드캐스팅 | 크기가 다른 배열 간 연산 지원 |
| 수학 함수 제공 | 통계, 선형대수, 푸리에 변환 등 포함 |

---

## 🔧 설치 및 사용

```bash
pip install numpy
```

```python
import numpy as np
```

---

## 🧮 배열 생성

```python
a = np.array([1, 2, 3])            # 1차원 배열
b = np.array([[1, 2], [3, 4]])     # 2차원 배열

np.zeros((2, 3))      # 2x3 배열, 0으로 초기화
np.ones((3, 3))       # 3x3 배열, 1로 초기화
np.eye(3)             # 3x3 단위 행렬
np.arange(0, 10, 2)   # [0, 2, 4, 6, 8]
np.linspace(0, 1, 5)  # [0. 0.25 0.5 0.75 1.]
```

---

## 🔢 배열 연산

```python
x = np.array([1, 2, 3])
y = np.array([4, 5, 6])

x + y     # 요소별 덧셈
x * y     # 요소별 곱셈
x @ y     # 벡터 내적
```

### 브로드캐스팅 예시

```python
a = np.array([[1], [2], [3]])
b = np.array([10, 20, 30])

result = a + b
```

---

## 📐 배열 속성

```python
a.shape      # (행, 열)
a.ndim       # 차원 수
a.size       # 전체 요소 개수
a.dtype      # 데이터 타입
```

---

## 🎲 난수 생성

```python
np.random.rand(2, 3)       # 0~1 균일분포 난수
np.random.randn(2, 3)      # 표준정규분포 난수
np.random.randint(0, 10, size=(2, 2))  # 정수 난수
```

---

## 📊 유용한 함수들

```python
np.mean(a)     # 평균
np.std(a)      # 표준편차
np.sum(a)      # 합계
np.max(a)      # 최댓값
np.min(a)      # 최솟값
np.argmax(a)   # 최댓값 인덱스
```

---

## ✅ 마무리

NumPy는 Python의 수치 연산과 데이터 분석의 기반 라이브러리로,  
Pandas, Scikit-learn, TensorFlow, PyTorch 등에서도 광범위하게 사용됩니다.

