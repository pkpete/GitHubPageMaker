---
layout: post
current: post
cover:  assets/built/images/boostcamp.jpg
navigation: True
title: Week 1
date: 2021-08-05 15:00:00
tags: [boostcamp]
class: post-template
subclass: 'post tag-boostcamp'
author: pkpete
---

Week 1
====
## 목차
- [Day 01](#day-01)
- [Day 02](#day-02)
- [Day 03](#day-03)
- [Day 04](#day-04)

---

## Day 01
### 강의 복습 내용
##### [Python2-1]
###### 변수
- 데이터을 저장하기 위한 메모리 공간
- 값은 메모리 주소에 할당된다
ex A = 8 .. A라는 이름을 가진 메모리 주소에 8을 저장하라

###### Dynamic Typing
- 다른 언어와 달리 파이썬은 코드 실행 시점에 데이터의 Type을 경정한다

###### List 
- Indexing
    - List에 있는 값들은 주소를 갖는다
- Slicing
    - List의 값들을 잘라서 쓰는 것
ex) alpha = ['a', 'b', 'c', 'd', 'e']
print(alpha[:]) #['a', 'b', 'c', 'd', 'e']
print(alpha[-4:])    #['b', 'c', 'd', 'e']

- List의 연산
    - \+ : 합치기
    - \* : 반복
    - len() : 리스트 길이
    - append : 이어붙이기
    ex) alpha.append('z')
    - extend : 새로운 리스트 추가
    ex) alpha.extend(['z'])
    - insert
    ex) alpha.insert(0,'a')
    - remove
    ex) alpha.remove('z')
    - del
    ex) del alpha[0]

###### 패킹과 언패킹
- 패킹 : 한 변수에 여러 개의 데이터를 넣는 것
- 언패킹 : 한 변수의 데이터를 각각의 변수로 반환
ex) t = [1,2,3]
a, b, c = t

##### [Python 2-2]
###### 함수
- 어떤 일을 수행하는 코드의 덩어리
- def 함수이름 () : 

###### print formatting
- %string, format 함수, fstring 중 fstring이 가장 깔끔!
    - fstring example ****************

##### [Python 2-3]
###### 조건문
- 어떤 일을 수행하는 코드의 덩어리
- def 함수이름 () : ***********

###### 반복문
- 반복 시작 조건, 종료 조건, 수행 명령으로 구성
- for문
    - range() 사용하기
    - **************
- while문

##### [Python 2-4]
###### String
- 시퀀스 자료형으로 문자형 data를 메모리에 저장
- string은 1byte 크기로 한 글자씩 메모리 공간이 할당됨
    - Indexing
    - Slicing
    - 덧셈 뺄셈 연산 가능
    - 문자열 함수 **************

###### 파이썬 함수 호출 방식
- Call by Object Reference 객체의 주소가 함수로 전달되는 방식
    - 전달된 객체를 참조하여 변경 시 호출자에 영향을 주나, 새로운 객체를 만들면 호출자에 영향을 주지 않는다

### 피어세션 정리 및 학습 회고
BoostCamp 첫 날 서로에 대해 알아가는 시간을 갖고 무슨 활동을 해야되는지 정했다. 매일 진행 정도를 맞추어서 강의 중 이해하기 어려웠던 부분과 과제 코드 리뷰를 하기로 했다.
다른 조원 분들과 같이 부스트 캠프를 완료하기 위해 많이 노력해야 될거 같다!

---

## Day 02
### 강의 복습 내용
##### [Python3-1]
###### 자료 구조
- 스택 (Stack)
    - 리스트를 사용하여 스택 구현 가능
    - append(), pop()
- 큐 (Queue)
    - 리스트를 사용하여 큐 구현 가능
    - append(), pop(0)
- 튜플 (Tuple)
    - 값의 변경이 불가능한 리스트
    - 선언 시 '()'를 사용
    - 리스트의 특징과 동일하다 --> 왜 쓸까??
    프로그램을 작동하는 동안 변경되지 않은 데이터를 저장하기 위해!
- 집합 (Set)
    - 값을 순서없이 저장, 중복 불허 하는 자료형
    - *************
- 사전 (Dictionary)
    - Key와 Value를 매칭하여 key로 value 검색
    - .items()
    - .keys()
    - .values()
- Counter
    - Sequence type의 data element들의 개수를 dict 형태로 반환
    - ****************

##### [Python 3-2]
###### Pythonic Code
- 파이썬의 특유의 문법을 활용해 효율적으로 코드를 표현
- split
    - string 값을 기준으로 나눠서 List 형태로 변환
- join
    - string으로 구성된 List를 합쳐 하나의 string으로 반환
- list comprehension
    - 기존 list를 사용해 다른 list를 만드는 기법
    - for + append 보다 빠름
    - ********************
- enumerate
    - list의 element를 추출할 때 번호를 붙여서 추출
    - ********************
- zip
    - 두 개의 list의 값을 병렬적으로 추출함
- 가변인자 (variable-length)
    - 개수가 정해지지 않은 변수를 함수의 파라미터로 사용하는 법
    - \* 기호를 사용하여 표시
    - *********************
- 키워드 가변인자 (Keyword variable-length)
    - 파라미터 이름을 따로 지정하지 않고 입력
    - \*\*기호를 사용하여 표시
    - **********************

##### [Python 4-1]
###### 클래스와 객체
- 속성(변수)과 행동(함수)을 갖는다
- ************예시 사진
- \_\_init\_\_ : 객체 초기화 예약 함수
- \_\_는 특수한 예약 함수나 변수로 사용
- Class 함수로 self를 반드시 추가해야된다
- 상속 (Inheritance)
    - 부모클래스로부터 속성과 Method를 물려받은 자식 클래스를 생성하는 것
- 다형성 (Polymorphism)
    - 같은 이름 메소드의 내부 로직을 다르게 작성


##### [Python 4-2]
###### Module
- 프로그램에서의 작은 프로그램 조각들, 모듈을 모아 하나의 큰 프로그램 개발
- import 문을 사용해서 모듈 호출
###### Package
- 모둘을 모아 놓은 단위, 하나의 프로그램

##### [AI Math 1]
###### Module
- 
###### Package
-

##### [AI Math 2]
###### Module
- 
###### Package

##### [AI Math 3]
###### Module
- 
###### Package

##### [AI Math 4]
###### Module
- 
###### Package

##### [AI Math 5]
###### Module
- 
###### Package
- 

### 피어세션 정리 및 학습 회고
과제의 코드 리뷰를 통해 다른 조원분들이 파이썬 코드를 어떻게 짜는 지 보고 배울 수 있었다. 확실히 C++로만 코딩한 나보다 더 효율적으로 잘 짜신다. 보고 많이 배워야 될거같다! 파이썬의 모듈들을 빨리 알아 보고 정규표현도 공부해야된다. 수학은 역시나 어렵다.... 주말을 통해 다시 정리해야될거 같다

---

## Day 03
### 강의 복습 내용
##### [Python3-1]
###### 자료 구조
- 스택 (Stack)
    - 리스트를 사용하여 스택 구현 가능
    - append(), pop()
- 큐 (Queue)
    - 리스트를 사용하여 큐 구현 가능
    - append(), pop(0)
- 튜플 (Tuple)
    - 값의 변경이 불가능한 리스트
    - 선언 시 '()'를 사용
    - 리스트의 특징과 동일하다 --> 왜 쓸까??
    프로그램을 작동하는 동안 변경되지 않은 데이터를 저장하기 위해!
- 집합 (Set)
    - 값을 순서없이 저장, 중복 불허 하는 자료형
    - *************
- 사전 (Dictionary)
    - Key와 Value를 매칭하여 key로 value 검색
    - .items()
    - .keys()
    - .values()
- Counter
    - Sequence type의 data element들의 개수를 dict 형태로 반환
    - ****************

##### [Python 3-2]
###### Pythonic Code
- 파이썬의 특유의 문법을 활용해 효율적으로 코드를 표현
- split
    - string 값을 기준으로 나눠서 List 형태로 변환
- join
    - string으로 구성된 List를 합쳐 하나의 string으로 반환
- list comprehension
    - 기존 list를 사용해 다른 list를 만드는 기법
    - for + append 보다 빠름
    - ********************
- enumerate
    - list의 element를 추출할 때 번호를 붙여서 추출
    - ********************
- zip
    - 두 개의 list의 값을 병렬적으로 추출함
- 가변인자 (variable-length)
    - 개수가 정해지지 않은 변수를 함수의 파라미터로 사용하는 법
    - \* 기호를 사용하여 표시
    - *********************
- 키워드 가변인자 (Keyword variable-length)
    - 파라미터 이름을 따로 지정하지 않고 입력
    - \*\*기호를 사용하여 표시
    - **********************

##### [Python 4-1]
###### 클래스와 객체
- 속성(변수)과 행동(함수)을 갖는다
- ************예시 사진
- \_\_init\_\_ : 객체 초기화 예약 함수
- \_\_는 특수한 예약 함수나 변수로 사용
- Class 함수로 self를 반드시 추가해야된다
- 상속 (Inheritance)
    - 부모클래스로부터 속성과 Method를 물려받은 자식 클래스를 생성하는 것
- 다형성 (Polymorphism)
    - 같은 이름 메소드의 내부 로직을 다르게 작성


##### [Python 4-2]
###### Module
- 프로그램에서의 작은 프로그램 조각들, 모듈을 모아 하나의 큰 프로그램 개발
- import 문을 사용해서 모듈 호출
###### Package
- 모둘을 모아 놓은 단위, 하나의 프로그램

##### [AI Math 6]
###### 

##### [AI Math 7]
###### 

##### [AI Math 8]
###### 

##### [AI Math 9]
###### 


### 피어세션 정리 및 학습 회고


---

## Day 04
### 강의 복습 내용
##### [Python5-1]
###### Exception
- try ~ except 문법
    -  ************** 사진 올리기
    -  Built in exception 표 사진 올리기
###### File handling
- 디렉토리
    - 폴더 또는 디렉토리로 불림
    - 파일과 다른 디렉토리를 포함할 수 있음
- 파일
    - 컴퓨터에서 정보를 저장하는 논리적인 단위
    - 실행, 쓰기, 읽기 등 가능
    - *************** 이미지 넣기


##### [Python 5-2]
###### Python Data Handling
- CSV
    - 쉼표로 구분한 텍스트 파일
    - 엑셀 양식의 데이터를 프로그램에 상관없이 쓰기위한 데이터 형식
- 정규식 (Regular expression) ******
    - 복잡한 문자열 패턴을 정의하는 문자 표현 공식
    - 특정한 규칙을 가진 문자열의 집합 추출


##### [Python 6]
###### Numpy

##### [AI Math 10]
###### 

### 피어세션 정리 및 학습 회고
다 같이 과제에 대한 코드리뷰를 진행했다. 오늘도 역시나 파이썬의 좋은 모듈들을 볼 수 있어 좋은 기회였다. 그리고 정규표현식의 중요성을 다시 느꼈다.마스터 클래스 수업에서 임성빈 교수님의 말씀을 들을 수 있었다. 부스트코스의 많은 수강생 역시 나 처럼 수학에 대해 어려움을 겪고 있어, 교수님이 소소한 팁들을 알려 주었다.
- 용어의 정의(Definition)부터 외우자!
    - 교과서, 위키피디아 등 구글링해서 알아보자!
    - AI Korea, PyTorch KR, TensorFlow KR 에 질문글 남겨라
- 용어를 외웠다면 예제를 찾아 보도록 하자!
    - 언제, 어디서, 어떤 경우에 쓰인다를 알아가는 것이 중요!!

- 선형대수 / 확률론 / 통계학은 꼭 알아두자!
- 책 추천 : [Dive into Deep Learning](https://d2l.ai/)

---


