## 현재 환경

- Windows 10
- Python 3.6.7(pip 19.1)
- Java 12.0.2

## 설치

1. [https://spark.apache.org/downloads.html](https://spark.apache.org/downloads.html) 들어가서 기본값으로 tgz 파일 설치
2. 적절한 위치에 압축해제
    - 관리자 권한 문제가 발생되지 않는 곳에 압축해제 ex. [C:\Users\USER_NAME]
    - 저 같은 경우 C:\Users\USER_NAME\spark에 추가
3. 환경변수 추가 / PATH 추가
    - 내 PC 우클릭 → 속성 → 고급 시스템 설정 → 환경변수 → 사용자 변수에서 아래 3개 추가
    - {변수 이름: HADOOP_HOME, 변수 값: C:\Users\USER_NAME\spark}
    - {변수 이름: SPARK_HOME, 변수 값: C:\Users\USER_NAME\spark}
    - PATH 추가: ~~\C:\Users\USER_NAME\spark\bin
4. winutils 설치
    - [https://github.com/steveloughran/winutils](https://github.com/steveloughran/winutils) 요기에 들어가서 Clone or Download 클릭
    - 압축해제 후 1번에서 설치한 하둡버전과 맞는 winutils.exe를  C:\Users\USER_NAME\spark\bin에 추가
5. 확인

    ```spark --submit --version```

    - Version이 뜨긴 뜨는데 Warning도 함께 뜸 🤔

    - [stack overflow](https://stackoverflow.com/questions/52155078/how-to-fix-hadoop-warning-an-illegal-reflective-access-operation-has-occurred-e)에 나온 내용들
        1. Use Java 8 for Hadoop. Spark, Scala, etc. do not yet support Java 9 or newer yet.
        2. 할 수 있는게 없다 ?
        3. The message means that the hadoop native libraries are compiled 32-bit and you are running on a 64-bit setup. **You can ignore that message for a small Hadoop setup.**

        ~~→ 결론: 무시해보겠습니다 🤷‍♂️~~

        → Java 8로 다운그레이드 하면 워닝이 뜨지 않습니다 !
