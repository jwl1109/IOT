
# pandas 라이브러리 소개

`pandas`는 Python에서 데이터 조작 및 분석을 위한 강력하고 사용하기 쉬운 오픈 소스 라이브러리입니다. 특히 구조화된 데이터(예: 테이블 형식의 데이터)를 다루는 데 탁월합니다.

## 주요 객체

### 1. Series
- 1차원 배열 형태의 자료구조
- 인덱스를 가지는 배열과 유사
- 예시:
  ```python
  import pandas as pd
  s = pd.Series([10, 20, 30], index=["a", "b", "c"])
  ```

### 2. DataFrame
- 2차원 테이블 형태의 자료구조
- 행과 열로 구성되어 있으며, 각각 인덱스와 컬럼명을 가짐
- 예시:
  ```python
  data = {'name': ['Alice', 'Bob'], 'age': [25, 30]}
  df = pd.DataFrame(data)
  ```

## 주요 기능

- **CSV/Excel 파일 읽기 및 쓰기**:
  ```python
  df = pd.read_csv('file.csv')
  df.to_excel('output.xlsx')
  ```

- **데이터 탐색**:
  ```python
  df.head()       # 처음 5행
  df.describe()   # 요약 통계
  df.info()       # 데이터 요약
  ```

- **데이터 인덱싱 및 필터링**:
  ```python
  df['column']         # 특정 열 선택
  df.loc[0]            # 라벨 기반 인덱싱
  df.iloc[0]           # 위치 기반 인덱싱
  df[df['age'] > 20]   # 조건 필터링
  ```

- **결측치 처리**:
  ```python
  df.dropna()          # 결측치 제거
  df.fillna(0)         # 결측치 채우기
  ```

- **그룹화 및 집계**:
  ```python
  df.groupby('column').mean()
  ```

- **데이터 병합**:
  ```python
  pd.concat([df1, df2])
  pd.merge(df1, df2, on='key')
  ```

## 설치 방법

```bash
pip install pandas
```

## 공식 문서

- [pandas 공식 문서](https://pandas.pydata.org/docs/)

