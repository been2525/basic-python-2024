# 파이선 기초 2024
부경대 2024 IoT 개발자과정 기초 프로그래밍 언어 - 파이썬

## 1일차
- 개발환경 구축
    - 코딩폰트 - 나눔고딕코딩
    - Notepad++ 설치
    - Python 설치
    - Visual Studio code 설치
    - Git 설치
        - TortoiseGit 설치
        - Github 가입
        - Github Desktop 설치

- 파이썬 기초
    - 파이썬 개발자는 귀도 반 로썸
    - 1990년대 귀도 반 로썸이 크리스마스 이브에 취미로 개발
    - 콘솔출력
    - 주석
    - 변수
    - 자료형
    - 연산자

    ```python
    # 이부분은 주석입니다.
    var01 = 10 # 정수, 실수, 불, 문자열 모두 가능
    print(var01) # 10
    print(type(var01)) # <class of 'int'>

    print(5 + 4 / 2) # 7.0
    print(5 == 4) # False
    ```

## 2일차
- 파이썬 기초
    - 흐름제어
        - if : 참/거짓으로 조건 분기 (다른언어 switch)
        - for : 반복문 기본 ( 다른 언어 foreach)
        - while : 반복문 변형 (다른 언어 do~while)
    - 복합자료형 + 연산자(연산 함수)
        - 복합자료형 : list, tuple, dictionary
        - 마이너스 인덱스 : 뒤에서 부터 앞으로 점점 작아짐 ex/ -10  -9  .... -2 -1
        - 이중리스트 : list[][]
        - 리스트 연산은 +, *만 사용가능
            - +는 리시트를 연결 해주는 역할
            - *는 리스트를 반복하는 역할
        - len() : 리스트 길이함수
        - append() : 리스트 마지막에 하나 추가
        - insert : insert(index, val)의 경우 리스트의 index이후에 val추가
        - extend() : 기존 리스트 확장 +와 거의 유사
        - del() : 리스트 삭제
        - clear() : 내용만 삭제
    - 출력 포맷, 입력 방법
    - 구구단 + 디버깅

    ```python
    # debugging
    # F5(디버그시작), F10(한줄씩 실행), F11(함수안으로 진입), F9(중단점 토글)
    # shift + F5(디버깅종료)
    print('구구단 시작!')
    for x in range(2, 9+1): # 2부터 9까지 반복
        print(f'{x}단 ----->')
        for y in range(1, 9+1): # 1부터 9까지 반복
            print(f'{x} x {y} = {x*y:2d}', end='  ') # end= 엔터대신 공백으로 변경
        print() # 안쪽 for문이 끝나면 마지막 엔터를 하나 추가
    ```

## 3일차
- 파이썬 기초
    - 입력 방법
    - 별찍기(피라미드만들기)
    - 함수, 람다함수는 나중에...
    - 객체지향 OOP
        - 객체는 명사와 동사의 집합
        - 명사는 변수, 동사는 함수
        - 변수와 함수를 모두 모아둔 곳 : 클래스(class) / class = 객체는 아님
        - 클래스에서 하나씩 생성 : 객체(object)
        - 캡슐화 (__plateNumber)
    - 패키지, 모듈


## 4일차
- 파이썬 기초
    - 패키지, 모듈 계속
        - pip 사용

        ```shell
        > pip --version # 버전확인
        > pip list  # 현재 설치된 라이브러리 목록 확인
        > pip install 패키지명 # 패키지를 내컴퓨터에 설치
        > pip uninstall 패키지명 # 패키지를 삭제
        ```
    - 예외처리 : 비정상적 프로그램종료 막기


    ```python
    def divide(x, y):
        try:
            return x / y # ZeroDivisionError 발생
        except ZeroDivisionError as e:
            print('[오류!!] 제수는 0 될 수 없습니다.')
            return 0
    ```
    - 텍스트 파일 입출력

    ```python
    f = open('파일명', mode='r|w|a', encoding='cp949|utf-8')
    f.read()
    f.readline() # 읽기
    f.write('text') # 쓰기
    f.close() # 파일은 반드시 닫는다
    ```

- 파이썬 활용
    - 주피터 노트북
        - Ctrl + Shift + P (명령팔레트) 로 시작
        - 사용벙법 (test31_Jupiternb.ipynb 참조)
    - folium 기본사용
    ![folium사용법](https://raw.githubusercontent.com/been2525/basic-python-2024/main/images/python_001.png)

## 5일차
- 파이썬 응용
    - 주피터 노트북 활용 - 구글 코랩(Colab)






    - 가상환경
    - 객체지향(나중에....)
        - 오버로딩, 오버라이딩(재정의)
        - 상속, 다중상속
        - 추상클래스
