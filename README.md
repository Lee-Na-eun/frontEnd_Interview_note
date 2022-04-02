# 기술 면접 인터뷰 준비하기

① 나만의 주의사항

```
- 공부하면서 필기 꼼꼼하게 🔥

- 틀린 필기는 최대한 빠르게 업데이트 🚀

- 실제 면접에서 답변하는 것처럼 깔끔하게 🧹
```

<br/>

② 목차

```
- Computer Science

- JavaScript

- React

- HTML

- CSS
```

<br/>
<br/>

### Computer Science

- `프로세스와 스레드 🔥`

  - 프로세스가 뭔가요?
    - 정적인 데이터 묶음, 즉 프로그램을 메모리에 적재되면 실행이 되는데, 이때 실행 중인 프로그램을 의미
    - 프로세스는 각각 독립된 메모리 영역(Code, Data, Stack, Heap의 구조)을 할당받는다.
  - 스레드가 뭔가요?
    - 프로세스 내에서 실제로 작업을 수행하는 주체
  - 프로세스와 스레드는 어떤 차이가 있나요?
    - 프로세스는 실행중인 프로그램을 뜻하고, 스레드는 그 프로세스 안에서 작업되는 무언가를 얘기한다.
    - ex) 프로세스 : 크롬, 스레드 : 크롬에서 유튜브를 시청, 게임 다운로드 등등

- `싱글 스레드와 멀티 스레드 🔥`

  - 싱글 스레드 장점
    - 공유자원을 접근하는 동기화 문제를 신경쓰지 않아도 된다.
    - context switch 작업을 요구하지 않아서, 전환 비용이 들지 않는다.
  - 싱글 스레드 단점
    - 여러 개의 작업을 실행해야할 때, 지연된다.
  - 멀티 스레드 장점
    - 프로세스의 자원과 상태를 공유하여 효율적으로 운영이 가능하다.
    - 새로운 프로세스를 생성하는 것보다 기존 프로세스에서 스레드를 생성하는 것이 빠르다.
  - 멀티 스레드 단점
    - 하나의 스레드만 실행중일 때는 실행시간이 오히려 지연될 수 있다.
    - 스레드 스케쥴링을 신경써야 한다.

- `HTTP 🔥`

  - HTTP란 뭔가요?
    - 텍스트 기반의 통신규약으로 인터넷에서 데이터를 주고 받을 수 있는 프로토콜이다.
  - HTTP 프로토콜의 가장 큰 특징은 뭔가요?
    - HTTP 메세지는 HTTP 서버와 HTTP 클라이언트로 의해 해석이 된다.
    - 클라이언트에서 요청을 보냈을 시, 서버는 그 요청에 알맞은 응답을 보낸다.
  - URL은 뭔가요?
  - HTTP/1.1 과 HTTP/2.0의 차이는 뭔가요?
  - HTTPS는 HTTP랑 뭐가 다른가요?
  - 심화) 공개키 (비대칭키) 방식이 뭔가요?

- `CI CD 🔥`

  - CI CD란 뭔가요?
    - CI는 Contiunous Integration의 약자로, 지속적 통합을 의미하는데, 프로그래머들이 각자가 만든 코드를 통합하는 단계를 말하기도 한다.
    - CD는 Continuous Deployment의 약자로, 지속적 배포를 의미한다. 소프트웨어를 코딩한 결과를 최종 사용자에게 실행 가능하도록 하는 단계를 말하기도 한다.

- `웹팩 🔥`

  - 웹팩이란?
    - 여러개로 나누어져 있는 파일들을 하나의 자바스크립트 코드로 압축하고 최적화하는 라이브러리
  - 모듈이란?
    - 개발하는 애플리케이션이 크기가 커지면서 확장성과 유지보수를 위하여 파일을 여러개로 분리해야하는데, 이 때 각 파일 하나하나를 모듈이라고 부른다.
    - 모듈은 보통 클래스 하나 혹은, 특정 목적을 가지는 복수의 함수 구성을 뜻하기도 한다.
  - 모듈 번들링이란?
    - 세분화 되어 분리된 모듈들을 묶어주는 것을 의미한다
  - 웹팩이 등장한 이유 웹팩 사용 시에 이점
    - 파일 단위의 모듈 관리 필요성
    - 애플리케이션의 빠른 로딩 속도와 높은 성능
  - 바벨이란?
    - 입력과 출력 모두 자바스크립트 코드인 컴파일러를 의미한다.
  - 웹팩의 주요 속성 4가지
    - Entry : 빌드를 할 대상 파일 정의
    - Output : 빌드를 한 후(=웹팩으로 변환 후)의 결과물에 대한 정보를 저장
    - Loader(모듈) : entry -> output 단계에서 개입
    - Plugins

- `타입과 인터페이스 🔥`
  - 타입스크립트를 왜 쓰나요? (본인이 느낀점)
    - 유연한 자바스크립트가 잡아내지 못 하는 에러를 타입스크립트에선 타입만 지정해주면 빠르게 확일 할 수 있기 때문에
  - 타입과 인터페이스의 차이를 아나요?
    - 타입은 선언 병합이 불가능하고, 인터페이스는 가능하다.
  - 프로젝트 진행 시에 어떤 상황에서 타입을 쓰고 어떤 상황에서 인터페이스를 썼나요?
    - 절대적으로 하나의 type만 존재해야할 때는 타입을 사용했지만, 인터페이스는 새로운 속성을 추가할 시, 편리하게 사용하였다.

<br/>
<br/>

### Javascript

- `프로그래밍 🔥`

  - 프로그래밍이란 뭐라고 생각하나요?
    - 특정목적을 위하여 컴퓨터가 처리하는 일 순서를 컴퓨터가 이해할 수 있는 언어로 작성하는 작업
  - 컴파일러는 뭐고 인터프리터는 뭔가요?
    - 프로그래밍 언어로 작성된 코드를 컴퓨터가 이해할 수 있게 컴퓨터 언어로 변환해주는 변환기
    - 컴파일러 : 작성된 프로그램 전체를 목적 프로그램으로 번역한 후, 링킹 작업을 통해 컴퓨터에서 실행 가능한 실행 프로그램을 생성
    - 인터프리터 : 작성된 프로그램을 한 줄 단위로 받아들여 번역하고, 번역과 동시에 프로그램을 한 줄 단위로 즉시 실행시키는 프로그램
  - 자바스크립트란 🔥
    - 웹페이지를 풍부하게 만들어주는 스크립트 혹은 프로그래밍 언어이다.
  - 자바스크립트의 특징은 뭐가 있나요?
    - 객체기반 언어이지만 상속과 클래스 개념은 존재하지 않는다.
    - 컴파일 과정이 없기 때문에 다른 언어들에 비해 빠른 시간안에 코드를 작성할 수 있다.
    - HTML문서 내에 기술되고 HTML 문서와 함께 수행된다.

- `변수 🔥`

  - 변수란 무엇인가요?
    - 하나의 값을 저장할 수 있는 저장공간을 변수라고 한다.
  - 식별자란 무엇인가요? fire
    - 자바스크립트에서 이름을 붙일 때 사용하는 단어
  - 변수를 선언한다는 것은 어떤 것을 의미하나요?
    - 저장공간이라는 변수에 이름을 붙임으로써 지정된 값을 대입해 주는 것을 의미한다.
  - var 키워드는 뭔가요?
    - 변수 중복 선언 허용
    - var 키워드 생략 허용
    - 함수 레벨 스코프로 인해 함수 외부에서 선언한 변수는 모두 전역 변수로 된다.
  - 호이스팅이 뭔가요? firefirefirefire
    - 변수 선언이 어디에 있든 상관없이 다른 코드보다 먼저 실행되는 특징을 호이스팅이라고 한다.
  - var, let, const 차이점
    - var vs let, const : 중복 선언이 불가능 하다 / 모든 코드 블록을 지역 스코프로 인정하는 블록 레벨 스코프를 따른다.
    - let vs const : let은 선언 단계와 초기화 단계가 분리되어 진행되지만 const는 동시에 진행된다.
  - TDZ firefirefire
    - 선언 단계와 초기화 단계 사이를 일시적 사각 지대라고 부른다.
  - 식별자 네이밍 규칙은 어떤 것들이 있나요?
    - 식별자는 특수문자를 제외한 문자, 숫자, 언더스코어(\_), 달러 기호($)를 포함할 수 있다.
    - 단, 식별자는 특수문자를 제외한 문자, 언더스코어(\_), 달러 기호($)로 시작해야 한다. (숫자 X)
    - 예약어는 식별자로 사용할 수 없다.
  - 네이밍 컨벤션은 어떤 것들이 있나요?
    - 하나 이상의 영어 단어로 구성된 식별자를 만들 때 가독성 좋게 단어를 한눈에 구분하기 위해 규정한 명명 규칙
    - Camel Case / Pascal Case
  - 리터럴이 뭔가요?
    - 데이터(값) 그 자체를 뜻한다. 즉, 변수에 넣는 변하지 않는 데이터를 의미
    - const a = 1일 때 1이 리터럴이다.

- `데이터 타입 🔥`

  - 데이터 타입의 종류는 어떤 것들이 있나요? fire
    - 기본형 : number, undefined, string, boolean, null 등
    - 참조형 : array, object, funtion, date 등
  - 심벌 타입은 뭐죠?
    - ES6에서 도입된 데이터 타입으로 변경 불가능한 원시 타입의 값
  - 데이터 타입은 왜 필요할까요? fire
    - 값을 저장할 때 확보해야 하는 메모리 공간의 크기를 결정하기 위해
    - 값을 참조할 때 한 번에 읽어 들여야 할 메모리 공간의 크기를 결정하기 위해
  - 정적 타이핑이 뭔가요?
    - 코드를 작성할 때 컴퓨터적 구조를 명시해주는 것을 정적 타이핑
  - 동적 타이핑이 뭔가요?
    - 따로 코드에 데이터 타입을 명시하지 않아도 컴퓨터가 알아서 해석하는 것을 동적 타이핑

- `타입변환과 단축 평가 🔥`

  - 명시적 타입 변환이 뭔가요?
    - 개발자가 의도적으로 데이터 타입을 바꾸는 것
  - 명시적 타입 변환 함수를 예를 들어볼 수 있나요?
    - toString(1) -> '1'
  - 암묵적 타입 변환이 뭔가요?
    - 자바스크립트 엔진이 자동으로 데이터 타입을 변환시키는 것
  - truthy / falsy 한 값이 뭔가요?
    - truthy : falsy한 값 그 이외의 것들
    - falsy : 0 / Nan / undefined / '' / null / false

- `배열 🔥`

  - 자바스크립트의 배열은 자료구조의 배열과 같나요?
    - 다르다. 엄연히 말하자면 자바스크립트의 배열은 일반적인 배열 동작을 흉내낸 특수 객체이다.
  - 배열의 메서드는 어떤 종류가 있나요?
    - pop, push, unshift, shift, splice, slice, concat 등등
  - 고차 함수에 대해서 아나요?
    - 함수를 인자로 전달 받거나, 함수를 반환하는 함수를 고차함수라고 한다.
  - forEach 메서드와 map메서드의 차이점에 대해 알고 있나요?
    - forEach : 배열의 요소마다 한 번씩 주어진 함수를 실행 시킨다.
    - map : 배열 내의 모든 요소 각각에 대하여 주어진 함수를 호출한 결과를 모아 새로운 배열을 반환한다.

- `객체 리터럴 🔥`

  - 자바스크립트에서 객체란 뭘까요?
    - key와 value로 구성된 property
  - 함수와 메서드의 차이점에 대해 알고 계신가요?
    - 함수는 메서드를 포함하는 개념이라고 볼 수 있다.
    - 메서드는 객체의 키값이 함수인 것을 메서드라고 한다.
  - 자바스크립트에서 객체를 생성하는 방법은 어떤 것들이 있나요?
    - 기본 객체의 생성자 함수 이용 : new Object()
    - 객체 리터럴 이용 : const test = {a : 1, b : 2}
    - 생성자 함수 이용 : 함수를 만들어서 this를 빈 객체에 바인딩하기

- `원시 값과 객체 비교 🔥`

  - 값에 의한 전달이 뭔가요?
    - 인수로 전달되는 변수가 가지고 있는 값을 함수 내의 매개변수에 복사하는 방식 (깊은 복사)
  - 참조에 의한 전달이 뭔가요?
    - 인수로 변수의 값을 전달하는 것이 아닌, 해당 변수의 주소값을 전달하는 방식 (얕은 복사)

- `함수 🔥`

  - 자바스크립트에서 함수를 정의하는 방법은 몇가지가 있나요?
    - 함수 선언식 / 함수 표현식
  - 함수 선언문과 함수 표현식은 어떤 차이가 있나요?
    - 함수 선언식은 호이스팅에 영향을 받지만, 함수 표현식은 호이스팅에 영향을 받지 않는다.

- `스코프 🔥`

  - 스코프가 뭔가요? firefirefire
    - 유효범위 : 어느 범위까지 참조 하는지를 뜻한다.
  - 스코프에는 어떤 종류가 있죠? firefire
    - 전역 스코프 : 스크립트 전체에 참조되는 것
    - 지역 스코프 : 정의된 함수 내에서만 참조 되는 것
  - 렉시컬 스코프를 아나요? 안다면 렉시컬 스코프는 무엇을 의미하나요? fire
    - 함수를 어디서 선언하였는지에 따라 상위 스코프를 결정하는 것
  - 전역 변수로 변수를 선언하면 생기는 문제점은 무엇이 있을까요?
    - 파일이 분리되어있다 하더라도 하나의 전역 스코프를 공유하기 때문에 다른 파일 내에서 동일한 전역 변수나 함수를 사용할 시, 예상치 못한 결과를 야기할 수 있다.

- `생성자 함수에 의한 객체 생성 🔥`

  - 생성자 함수가 뭔가요?
    - 객체를 생성하는 함수 -> new 연산자를 통해서 객체를 생성
  - 객체 리터럴로 만들 때와는 무슨 차이가 있죠? 왜 생성자 함수를 사용하나요?
    - 객체 리터럴은 본체에 필요한 물품을 끼워넣는 것
    - 생성자 함수는 같은 객체를 생성하기 위한 큰 틀 같은 것
    - 객체 리터럴과 달리 생성자 함수는 동일한 프로퍼티와 메소드를 가지는 객체를 생성할 때 유용하게 사용할 수 있기 때문에
  - 생성자 함수가 객체(인스턴스)를 생성하는 과정에 대해 간략하게 설명해줄 수 있나요?

    - const Car = (color) => {
      this.color = color;
      }

    const testCar = new Car('red');

- `함수와 일급 객체 🔥`

  - 일급 객체가 뭔가요?
    - 다른 객체들에 일반적으로 적용 가능한 연산을 모두 지원하는 객체
  - 자바스크립트에서 함수가 일급 객체라면, 일급 객체로 뭘 할 수 있나요?
    - 고차함수를 만들 수 있다.
    - 콜백을 할 수 있다.
  - 꼬리 질문) 함수형 프로그래밍이 뭔가요? firefire
    - 외부의 요인에 영향을 받지 않기 때문에 언제나 같은 아웃풋이 철저한 프로그래밍
  - 꼬리 질문) 순수 함수가 뭔가요? 일반 함수와는 어떤 차이가 있죠? firefire
    - 외부 요인에서부터 철저히 독립적인 성격 때문에 변질되는 것 없이 예상되는 값이 나오는 함수를 의미한다.
    - 일반 함수는 변이 되는 요인이 있을 때, 함수의 성질이 변질 될 수 있다.

- `프로토타입 🔥`

  - 객체지향 프로그래밍은 무엇을 의미하나요? fire
    - 프로그래밍에서 필요한 데이터를 추상화시켜 상태와 행위를 가진 객체를 만들고 그 객체들 간의 유기적인 상호작용을 통해 로직을 구성하는 프로그래밍 방법
    - 상태와 행위를 가진 객체들을 레고 블럭처럼 조립해서 하나의 프로그램을 만드는 것
  - 객체지향 프로그래밍의 특징에 대해 말해볼 수 있나요? fire
    - 추상화
    - 캡슐화
    - 상속
    - 다형성
  - 자바스크립트는 객체지향 프로그래밍 언어인가요?
    - 자바스크립트 객체를 생성하는 생성자 함수를 제공하고 있기 때문에 객체지향 프로그래밍 언어라고도 불리지만 정확히는 프로토타입 기반의 프로그래밍 언어라고들 많이 얘기한다.

- `strict mode 🔥`
  strict mode가 뭔가요?
  strict mode를 통해 무엇을 예방할 수 있죠?

- `빌트인 객체 🔥`
  빌트인 객체가 뭔가요? 종류는 어떤게 있죠?
  래퍼 객체에 대해서 알고 있나요?

- `this 🔥`
  this가 뭔가요? fire
  this 바인딩이란? fire
  this는 동적으로 바인딩이 된다고 하는데 바인딩되는 객체가 어떻게 다르나요?

- `실행 컨텍스트 🔥`
  실행 컨텍스트에 대해 말해보세요 firefire

- `클로저 🔥`
  클로저에 대해서 아나요? firefirefire
  클로저를 사용하면 뭐가 좋죠? firefire
  클로저를 어떻게 생성하나요? fire

- `클래스 🔥`
  자바스크립트에서 클래스가 생기기 전에는 어떤 방식으로 객체지향 패턴을 구현했나요?
  그럼 생성자 함수와 클래스는 어떤 차이가 있나요?
  클래스 정의
  클래스의 상속

- `스프레드 문법 🔥`
  spread 문법이 뭔가요?
  어떤 상황에서 사용할 수 있죠?

- `구조 분해 할당 🔥`

구조 분해 할당이 뭔가요?
구조 분해 할당은 크게 어떤 종류가 있나요?

- `브라우저 렌더링 과정 🔥`
  브라우저의 렌더링 과정에 대해 설명해보세요 fire
  브라우저의 렌더링 과정에 자바스크립트는 어떻게 동작하나요? fire
  <script></script> 태그를 <body></body> 태그 밑에 둬야하는 이유가 있을까요?

- `DOM 🔥`
  DOM이 뭔가요?
  DOM을 구성하는 건 뭐가 있나요?

- `이벤트 🔥`
  마우스 이벤트 타입에는 뭐가 있나요? click 말고 클릭을 대체할 수 있는 이벤트가 있나요?
  그 외에 알고 있는 대표적인 이벤트가 있나요?
  이벤트 핸들러를 등록하는 방식에는 어떤 것들이 있나요?
  이벤트 전파(propagation)에 대해서 알고 있나요?
  이벤트 위임(delegation)에 대해서 알고있나요? fire
  e.preventDefault 에 대해 알고 있나요?
  e.stopPropagation

- `타이머 🔥`
  호출 스케쥴링이 무엇인가요?
  타이머 함수에는 어떤 것들이 있나요?
  이벤트가 과도하게 호출되어 성능에 문제를 일으킬 경우에 할 수 있는 어떤 일을 통해 해결할 수 있나요?
  디바운스에 대해서 알고 있나요?
  쓰로틀에 대해서 알고 있나요?

- `비동기 프로그래밍 🔥`
  동기와 비동기의 차이점에 대해서 설명해줄 수 있나요? firefire
  이벤트 루프와 태스크 큐에 대해서 알고 있나요? firefirefire

마이크로태스크 큐에 대해서 알고 있나요? firefire

태스크 큐와 마이크로태스크 큐 중 어떤 것이 먼저 실행되나요? firefire

<br />

- `Ajax 🔥`
  Ajax가 뭔가요 어떤 것을 담당하고 있죠?
  Ajax를 사용하면 기존 방식과 어떤 차이가 있을까요?
  JSON 이 뭔가요?
  JSON이 제공하는 정적 프로토타입 메서드에 대해 몇가지 말해볼 수 있나요?
  Ajax로 HTTP 요청을 보내기 위해서는 어떤 방법을 사용할 수 있나요?
  XMLHttpRequest와 fetch 메서드의 차이는 무엇이라고 생각하시나요? fire

- `REST API 🔥`
  REST API가 뭔가요?
  REST API의 구성은 어떤 것이 있나요?
  REST API를 설계하는데 중요한 것이 있을까요?
  HTTP 요청 메서드에 대해서 아는대로 얘기해보세요
  HTTP 상태 코드를 아는대로 말해주세요 fire

- `Promise 🔥`
  콜백이란 뭐라고 생각하나요? fire
  프로미스가 뭔가요? fire
  프로미스 생성 방법
  프로미스의 상태를 나타내는 것은 어떤 것들이 있나요? fire
  프로미스 빌트인 객체가 제공하는 정적 메서드에 대해 알고 있나요? fire

- `제너레이터와 async await 🔥`
  제너레이터란 뭔가요? 일반 함수와는 어떤 차이가 있죠?
  제너레이터의 구조
  async/await 가 뭔가요? 기존의 Promise와는 어떤 차이가 있죠? fire
  Promise와 async/await의 차이점 한 줄 요약 fire

- `에러 🔥`
  에러처리를 왜 해야 하나요? fire
  자바스크립트에서 에러를 처리하는 방법에는 뭐가 있을까요?
