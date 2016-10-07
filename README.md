### Slipp QnA 만들기 - Spring boot를 이용해 개발 

#### 1-1 개발 환경 셋팅 

1. STS 설치 

2. 클라우드 서버 1대

3. spring boot project -> web/mustache/dev-tools 선택 

4. 크롬 확장 프로그램 - live reload 설치

#### 1-2 bootstrap 활용한 html 페이지 개발

1. bootstrap start html 추가
2. bootstrap css 라이브러리 추가
3. jquery, javascript 라이브러리 추가 
4. index.html -> navigation bar 추가
5. 회원가입 페이지 개발

* webjars로 라이브러리 추가 할 경우 서버를 재시작 해주어야 반영 됨.

#### 1-3 github에 소스 코드 추가 

* sourcetree에 저장소 추가 
* github에 소스 코드 추가

#### 1-4 원격 서버에 유저 생성 하기 

1. 우분투 환경에서 셋팅 하도록 한다. 
2. 유저가 root만 존재하다면, 새로 생성 한다. 
3. 생성한 유저에 sudo 권한을 설정 한다.
 
#### 1-5 원격 서버에 환경 셋팅 하기 

**jdk 설치**
 * `wget --no-cookies --header "Cookie: oraclelicense=accept-securebackup-cookie" http://download.oracle.com/otn-pub/java/jdk/8u101-b13/jdk-8u101-linux-x64.tar.gz`
 
**.gz 압축풀기** 
 * `gunzip jdk-8u101-linux-x64.tar.gz`
**.tar 풀기**
 * `tar -xvf jdk-8u101-linux-x64.tar` 
* `ln -s jdk 디렉토리명 링크명` 이 명령어를 통해 심볼릭 링크를 만든다. 

#### .bash_profile에 패쓰 추가 

```bash
JAVA_HOME=/home/seungdols/java_home
PATH=$PATH:$JAVA_HOME/bin
```

* maven 설치 필요 없이 git repository를 clone 받는다. 

* `./mvnw clean package`를 통해 빌드를 한다.

**서버 실행**

* `cd /target`이동

* `java -jar my-slipp.jar(file name) [&]`
 * `&`는 붙이면 데몬으로 서버가 동작하게 된다.*
  

#### 2-1 반복주기 2

1. Controller 추가 및 mustache에 인자 전달
2. 회원가입 페이지 구현
3. 사용자 목록 페이지 구현
4. 원격 서버에 배포
5. 이전 상태로 원복 후 반복 구현 


#### 2-2 반복주기 2 

1. controller 추가 및 회원 가입 구현


#### 2-3 반복주기 3

1. 사용자 목록 기능 구현 

