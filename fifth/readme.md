# TypeScript를 이용한 블록체인 클론코딩

## TypeScript와 JavaScript
1.타입스크립트는 자바스크립트와 다르게 컴파일 언어이다.<br>
2.정적 타입 언어여서 컴파일 시간이 걸리지만 안정성이 보장된다.<br>
3.반면 자바스크립트는 동적 타입 언어여서 런타임 속도는 빠르지만 안정성이 떨어진다.<br>
4.타입스크립트를 컴파일하면 자바스크립트로 변환이 된 후 실행이 된다.<br>
5.타입스크립트는 class와 interface의 특징을 지원함으로서 객체지향 프로그래밍 환경을 제공한다.<br>

## TypeScript 프로젝트 생성하는법
1. 프로젝트 폴더를 만든다.
2. 프로젝트 폴더 안에서 npm init -y 명령어로 package.json을 만든다.
![package_json](https://github.com/ChamChiii7/EcoleProject/assets/126247047/b4e8206d-7674-4db2-8963-e59243b0c7db)
3. npm install -D typescript 명령어로 devDependencies에 typescript를 설치한다.
4. src 폴더 생성 후 작업할 index.ts 파일을 생성한다.
5. touch tsconfig.json을 만든다.(이 파일 있으면 vscode에서 내가 typescript로 작업을 하고 있다는걸 알게되면서, 자동완성기능을 제공한다.) ![tsconfig_json](https://github.com/ChamChiii7/EcoleProject/assets/126247047/c0e071bd-80f6-4118-bc47-a700e30d407b)
6. tsconfig.json파일에 "outDir": "build" 코드를 추가해서 변환될 javascript 파일이 생성될 디렉토리를 지정해준다.

## Blockchain 코드
![Blockchain_1](https://github.com/ChamChiii7/EcoleProject/assets/126247047/5906cd92-4b6a-4318-8b74-3587a9ff7201)
![Blockchain_2](https://github.com/ChamChiii7/EcoleProject/assets/126247047/6aa9ce82-c3b0-4775-a71c-a9f9089c5efe)
![Blockchain_3](https://github.com/ChamChiii7/EcoleProject/assets/126247047/b23a1e27-5f51-41eb-bae1-a08677194477)

### Blockchain이 반영된 블록 결과
![Blockchain_4](https://github.com/ChamChiii7/EcoleProject/assets/126247047/d1c27bfe-fe79-4449-880e-dd3531091f23)

## Blockchain의 취약점을 노린 코드
![Hacked_code](https://github.com/ChamChiii7/EcoleProject/assets/126247047/25347a27-5d79-4714-938b-31b8c9ca0d3a)
새로운 블록을 push 할때 this.blocks으로 바로 리턴이 돼서 외부에서 원래 데이터와 관계없는 블록을 생성할 수 있다.<br>

### 취약점이 노출된 Blockchain의 결과
![Hacked_result](https://github.com/ChamChiii7/EcoleProject/assets/126247047/767b5772-4867-4382-a12c-f22c40b085e5)

## 취약점을 보완한 코드
![supple_code](https://github.com/ChamChiii7/EcoleProject/assets/126247047/00503b48-079a-41a2-8d51-44da0668f80e)

기존에는 this.blocks로 리턴이 됐지만, 코드를 수정하면서 getBlock 함수의 리턴값을 아예 새로운 블록으로 리턴시킴으로써
관련없는 블록 추가를 막았다.

### 취약점을 보완한 결과
![supple_result](https://github.com/ChamChiii7/EcoleProject/assets/126247047/18af9067-6cc3-4775-bdf6-5e5ddc560296)

### Clon Coding을 하며 느낀 점
일부러 완전히 처음 접하는 TypeScript를 활용하여 평소 관심있는 주제와 관련된 Blockchain 구현을 선택했다.<br>
그래서 처음 개념을 잡는것부터 시간이 많이 걸렸지만 본격적으로 코딩을 시작하며 평소 흥미있는 주제에 관련돼서 그런지 금방 끝낼 수 있었다.<br>
새로운 언어를 접했음에도 Clon Coding으로 접하니 생각보다 빠르게 적응을 할 수 있어서 좋았고, <br>
무작정 코드를 따라치기보다는 설명을 한번씩 더 들어보면서 코드를 따라쳐야 조금이라도 얻어가는게 더 많겠다고 느꼈다.
