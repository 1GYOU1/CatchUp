## __Node.js__
JavaScript 기반으로 구성된 서버 사이드 서비스를 JavaScript로 구현할 수 있게 만든 런타임

package.json : 프로젝트에 대한 명세 파일

## __npm__
node.js 기반의 모듈을 모아둔 집합 저장소

Node Package Manager 또는 Node Package Modules

npm은 Node.js 기반의 JavaScript로 개발된 오픈 소스를 모듈로 올려놓은 곳이다.
웹 개발에 필요한 jQuery, gulp, webpack 등의 모듈들을 npm명령어를 통해 쉽게 다운받고 쓸 수가 있다.

<br>

__package.json__

프로젝트의 정보와 특히 프로젝트가 의존하고 있는(설치한) 패키지(모듈)에 대한 정보가 저장되어 있는 파일.

----

## __Node.js 설치 (window)__

<br>

[__Node.js Download site__](https://nodejs.org/ko/download/)

<br>

vs code -> 폴더 진입 -> 보기 메뉴 -> 터미널 -> node -v 입력 -> 버전 확인

<br>

① 폴더 진입 명령어
```
cd node.js 
```
② 버전 확인 명령어
```
node -v
```
③ package.json파일 생성 - 옵션 선택
```
npm init
```
④ package.json파일 생성 - 옵션 기본값으로 자동 설정
```
npm init -y
```

----

## 명령어 ↓↓

<br>

__ctrl + `__ : vs code - node.js 터미널 실행 단축키

__node -v__ : node 설치(버전) 확인

__npm -v__ : npm 설치 확인

<br>

__cd 파일이름__ 앞부분 작성 + __tab__ -> 자동완성 : node.js 터미널 파일경로 찾기

<br>

__npm init__  
1. 패키지명을 명시해 특정 패키지를 설치하는 동작
2. 패키지명을 명시하지 않고 package.json 파일의 의존성을 설치하는 동작

ex) 
- `$ npm install express` 를 실행하면 express 모듈이 설치
- `$ npm install` 을 실행하면 package.json 에 포함된 의존성 패키지들이 일괄적으로 설치

__npm init -y__ : 기본값으로 설정 -> package.json파일 생성

__npm i nodemon -D__ : 모듈 설치

__npm i @babel/core @babel/cli @babel/node @babel/preset-env -D__ : 여러개 모듈 설치 예시

__npm i socket.io express ejs__ : 3개 모듈 설치

__npm run start__ : 시작

__ctrl + C__ : 끝내기

<br>

__http://localhost:포트숫자__ : 브라우저 테스트 url

<br>

__cls__ : 터미널 이전 기록 지우기

__clear__ : 터미널 이전 기록 지우기

<br>

__참고사이트 ↓↓__

[__Node.js와 NPM 설치__](https://kdydesign.github.io/2017/07/15/nodejs-npm-tutorial/)

[__npm-install-정리__](https://c17an.netlify.app/blog/node.js/npm-install-%EC%A0%95%EB%A6%AC/article/)

[__Node.js__](https://heropy.blog/2018/02/18/node-js-npm/)

<br>

----

## __Node.js 설치 (Mac OS)__

① [__Homebrew 설치__](https://brew.sh/index_ko)

mac에서 개발환경 세팅을 할 때 가장 먼저 설치해야 할 패키지 관리 프로그램

② [__Node.js 다운로드__](https://nodejs.org/ko/download/)


<br>

## __Node.js 버전 업그레이드 (Mac)__

<br>

① __sudo npm cache clean -f__ : (강제) npm 캐시를 지우기

② __sudo n stable__ : 현재 안정 버전으로 업그레이드

<br>

[참고사이트](https://choseongho93.tistory.com/293)



----
## __React 설치 (window)__

<br>

① cd 폴더명 - 설치할 폴더로 진입
```
cd .\React\
```
② npx create-react-app 폴더안에 생성할 프로젝트명
```
npx create-react-app project
```
③ cd 생성된 프로젝트 폴더명
```
cd project
```
```
npm run start
```
④ 테스트 페이지 진입

http://localhost:포트숫자

<br>

[참고사이트](https://codingapple.com/unit/react1-install-create-react-app-npx/)

[참고사이트](https://joyfulhome.tistory.com/181)

## __React.js 설치 (Mac OS)__

npx create-react-app 파일이름

cd 파일이름

npm start


[참고사이트 ①](https://eunhee-programming.tistory.com/165)

[참고사이트 ②](https://eunhee-programming.tistory.com/266)

----

오류

npm audit fix

npm audit fix --force

[참고사이트](https://medium.com/@kimjnsjwj/npm-about-audit-8e02e3b7c833)