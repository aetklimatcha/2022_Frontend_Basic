# md(MarkDown)

````
- # ~ ###### : 제목
- ```(backtick, 백틱)(esc아래의 작은 따옴표같은 것) : 세 번 쓰고자하는 내용 전 줄, 다음 줄로 넣으면 코드 블럭이 생성된다.
````

# Github

- 버전관리 소프트웨어인 git을 웹에서 쓸 수 있게 만들어준 것.
  (git은 cmd/프롬프트 창처럼 원하는 것을 하나씩 입력해야)

  - 버전관리 소프트웨어 : Git
  - Git 웹 서비스 : Github

- Git 버전관리 프로세스

  - 준비단계

    - remote repository 생성(원격저장소 생성)
      -> clone(복제) : 로컬 위치에 repository 가져옴

  - 작업단계

    - commit : 수정 확인
      -> push(업로드) : remote repository에 업로드

  - 협업단계
    - branch
      -> pull
      -> fetch

# 클라이언트 서버 시스템

클라이언트 서버 모델(client–server model)은 서비스 요청자인 클라이언트와 서비스 자원의 제공자인 서버 간에 작업을 분리해주는 네트워크 아키텍처를 나타낸다. 웹 시스템도 확장된 '클라이언트 서버 시스템'으로 분류되나, 일반적으로는 클라이언트 서버 시스템이라고 하면 웹 시스템이 나오기 이전의, 사용자 PC에는 클라이언트가 설치되어 화면을 처리하고 서버에서는 자료를 처리하는 시스템을 일컫는다.

# Front End(프론트 엔드) / Back End(백 엔드)

- Front End

  - 사용자를 기준으로 사용자가 제어하는 화면, 인터페이스 등이 위치하는 영역 / 사용자와 맞닿는 영역
  - UI 디자인, 개발
  - 클라이언트 시스템
    - H/W : PC, Mobile Device
    - S/W : **웹 - 브라우저**, 엣지, 익스플로러 / 앱 - 소프트웨어
  - Front End 개발
    - UI 개발
    - 브라우저(클라이언트)에서 해석되는 언어를 사용해서 개발
    - 웹 프론트엔드 언어 : HTML, CSS, Javascript
    - 앱 개발 언어(Native)
      - Android : Java -> Kotlin
      - IOS : Objective C -> Swift
  - 서버 시스템
    - H/W : 서버 컴퓨터(성능이 좋은 컴퓨터)
    - S/W : 서버 소프트웨어 - 아파치, IIS, nodejs(서버용 개발 언어 해석, 동작 도움)
  - Back End 개발
    - 서버(아파치, IIS)에서 해석되는 언어를 사용해서
    - 웹 백엔드 언어 : Java, php, asp, python, Javascript
    - 앱 개발 언어(Native)
      - Android : Java -> Kotlin
      - IOS : Objective C -> Swift

# 비트 계산
- ip 주소, 문자 표시, Color 표시
 
- bit : 컴퓨터가 표시할 수 있는 최소 단위
  - 1bit에 0 또는 1 숫자를 저장할 수 있음(2진수 : 0, 1)
  - 1bit로 의미를 부여할 수 있는 개수 : 2개

- byte : 의미있는 데이터를 표현하는 단위(=8bit)
  - 1byte로 의미를 부여할 수 있는 개수 : 256개(=2^8)(0~255)  

- 문자 표현
  - 영문 : 1byte 표현
  - 영문 + 다른 언어 표현 : 2byte 표현 => unicode

```
<meta charset="UTF-8"> : 유니코드로 문자 표시(인코딩)
```

- IP 주소
  - 1byte범위 숫자 4개로 구성
```
0~255 숫자 4개를 '.'으로 구분해서 사용
255.255.255.0
```

- 색 표현
  - 24bit 트루 컬러(3byte)
  - 16,777,216개 색 표현
  - 색 혼합 방식
    **- RGB(가산혼합 : 스크린) : Red, Green, Blue 색의 혼합**
      - R(1byte) / G(1byte) / B(1byte)
    - CMYK(감산혼합 : 프린터) : Cyan(청록색), Magenta(자주색), Yellow, Black 색의 혼합
  - 색 표현 값
    - 16진수 
    - 10진수