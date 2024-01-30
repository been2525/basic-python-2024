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
    ## 구구단 : 내일...
    ```

    ## 3일차
    - 파이썬 기초
        - 입력 방법
        - 별찍기
        - 함수
        - 객체지향