# Javascript의 함수형프로그래밍이란?

## 개요

주변 동료 개발자 또는 누군가가 나에게 함수형프로그래밍이 뭐야? 라고 묻는다면 나는 정확하게 설명을 할 수 없을 것 같다.

뭔가 함수형프로그래밍에 대해 어떻다라고 느낌은 알고 있지만, 이것에 대해 정확한 정의를 설명 할 수 없다면, 모르는 것이지 않을까? 라는 생각이 든다.

그렇기에 나는, 함수형프로그래밍에 대해 정확하게 설명을 할 수 있도록, 공부한 내용을 적어보고자 한다.

전공시간에 배운 객체지향프로그래밍에 대해서는 배웠고, 개발을 했더라면 이에 대한 내용은 많이 들어 봤을 것이다.

함수형프로그래밍에 대해 알아보기전에 간단하게, 객체지향 프로그래밍에 대한 정의를 살펴보자.

### 객체지향 프로그래밍 (OOP)

객체 지향 프로그래밍은 컴퓨터 프로그래밍 패러다임 중 하나로, 프로그래밍에서 필요한 데이터를 추상화시켜 상태와 행위를 가진 객체를 만들고 그 객체들 간의 유기적인 상호작용을 통해 로직을 구성하는 프로그래밍 방법이다.

그렇다면 객체지향프로그래밍의 장단점이 무엇일까?

### 객체지향 프로그래밍의 장단점

#### 장점

- 코드 재사용이 용이하다.
누군가가 만든 클래스형의 코드를 가져와서 사용할 수 있고 또한, 상속을 통해 확장해서 사용할 수 있다.

- 유지보수가 쉽다.
객체 지향 프로그래밍에서는 수정해야 할 부분이 클래스 내부에 멤버 변수혹은 메서드로 존재하기 때문에 해당 부분만 수정하면 된다.

- 프로젝트의 규모가 커질수록 장점 극대화
클래스 단위로 모듈화시켜서 개발할 수 있으므로, 대형 프로젝트처럼 여러 명, 여러 회사에서 프로젝트를 개발할 때 업무 분담하기 쉽다.

#### 단점

- 객체가 많으면 용량이 커지므로 속도에 영향을 준다.
- 설계 시 많은 시간과 노력이 필요로 한다.

### 객체지향 프로그래밍의 주요기능

- 클래스 + 인스턴스(객체)
- 추상화
- 캡슐화
- 상속
- 다형성

위와 같이 객체지향 프로그래밍의 주요기능이다.

사실 이번 포스트에서는 함수형프로그래밍에 대한 주제를 다룰 것이기 때문에, 이를 비교하기 위해, 객체지향 프로그래밍에 대해서는 상세히 다루지 않을 것이다.

추가로, 주요기능에 대해서 조금만 더 알아보자.

#### 1. 클래스, 인스턴스(객체)

클래스 : 어떤 문제를 해결하기 위한 데이터를 만들기 위해 추상화를 거쳐 집단에 속하는 속성(attribute)과 행위(behavior)를 변수와 메서드로 정의한 것으로 객체를 만들기 위한 메타정보라고 볼 수 있다.

인스턴스(객체) : 클래스에서 정의한 것을 토대로 실제 메모리에 할당된 것으로 실제 프로그램에서 사용되는 데이터

#### 2. 추상화

공통의 속성이나 기능을 묶어 이름을 붙이는 것이다.

#### 3. 캡슐화

캡슐화란 코드를 수정 없이, 재사용하는것과 접근 제어자를 통한 정보은닉을 말한다.

#### 4. 상속

부모클래스의 속성과 기능을 그대로 이어받아 사용할 수 있게하고, 기능의 일부분을 변경해야 할 경우 상속받은 자식클래스에서 해당 기능만 다시 수정(정의)하여 사용할 수 있게 하는 것이다.

#### 5. 다형성

오버라이딩 및 오버로딩이 가능하다.

오버라이딩이란, 부모클래스의 메서드와 같은 이름, 매개변수를 재정의 하는것이다.

오버로딩이란 같은 이름의 함수를 여러개 정의하고, 매개변수의 타입과 개수를 다르게 하여 매개변수에 따라 다르게 호출할 수 있게 하는 것이다.

여기까지, 메인 주제인 함수형프로그래밍과의 비교를 위해 주로 사용되는 패러다임인 객체지향프로그래밍에 대해 간단히 알아보았다.

이제 함수형 프로그래밍에 대해서 알아보자.

### 함수형 프로그래밍이란?

함수형 프로그래밍은 사실 최근에 생겨진 개념이 아니고 기존에 존재한 소프트웨어 개발의 한 방식이다.

하지만, 최근들어 새롭게 함수형프로그래밍에 대한 중요성이 부각되고 있는 프로그래밍의 한 패러다임이다.

함수형 프로그래밍은 하나의 프로그래밍 패러다임으로 정의되는 일련의 코딩 접근 방식이며, 자료처리를 수학적 함수의 계산으로 취급하고 상태와 가변 데이터를 멀리하는 프로그래밍 패러다임이다.

그렇다면, 함수형 프로그래밍의 장단점은 무엇일까?

### 함수형 프로그래밍의 장단점

#### 장점

- 함수 (기능) 단위의 코드 재사용이 수월하다.
- 불변성을 지향하기 때문에, 프로그램의 동작을 예측하기 쉬워진다.
- 사이드 이팩트가 없다.
- 함수는 입력과 출력만 신경쓰면 되므로, 테스트가 쉬워진다.

#### 단점

- 순수함수를 사용하는것은 쉬울수 있지만, 이를 조합하는 것은 쉽지않다.
- 함수형적으로 사고하지 않는다면, 한눈에 알아보기 힘들다.

위와 같이 함수형 프로그래밍의 장단점에 대해서 알아보았다.

그러면, 함수형 프로그래밍의 주요 특징은 무엇일까?

### 함수형 프로그래밍의 특징

- 순수함수 (Pure Function)
- 불변성 (Immutable)
- 1급 객체
- 고차함수

위와 같은 특징들을 지니고 있는데, 실제로 간단한 코드를 보면서 어떤 특징을 가지고 있는지 상세히 알아보도록 하자.

#### 1. 순수함수 (Pure Function)

순수함수란 함수를 실행 했을 때, 사이드이팩트 (side-effect) 가 없는 상태를 말한다.

함수를 실행 시켜도 외부의 상태, 값에는 절대로 영향을 끼쳐서는 안되고 순수하게 함수 내부에서만 모든 작업이 이루어져야 하는 것이 특징이다.

- 동일한 입력에는 항상 같은 값을 반환한다.
- 함수 실행이 프로그램의 실행에 영향을 끼치지 않아야 한다.
- 함수 내부에서 인자의 값을 변경하거나 프로그램 상태를 변경하는 사이드이팩트가 없어야 한다.

그렇다면, 예제를 통해 조금 더 자세히 알아보자.

```js
let num = 1;

function add(a) {
    return a + num;
}
```

위와 같은 코드는 순수 함수라고 할 수 있을까?

답은 아니다.

위에 설명한 것과 같이 순수 함수는 순수하게 함수 내부에서만 모든 작업이 이루어 져야하므로, 전역 변수인 num을 참조하는 위의 코드는 순수함수라고 볼 수 없다.

그렇다면 순수함수는 다음과 같은 형태를 띄고 있다.

```js
funtion add(a,b) {
    return a + b;
}

const number = add(5,3);
console.log(number); // 8
```

위의 코드는, 프로그램의 실행에 영향을 끼치지 않고, 함수 내부에서 모든 작업이 이루어 지며, 전달 받은 인자의 값에 대해서만 값을 반환 하므로 순수 함수라고 할 수 있다.

그렇기에, 순수 함수는 프로그램의 변화 없이 입력값에 대한 결과를 예상 할 수 있어 테스트가 용이 하다.

#### 2. 불변성

함수형 프로그래밍은 모든 상태는 변하지 않는다는 것을 가정하고 있다. 하지만 Javascript에서는 변수에 값을 할당한 후, 이를 다른 값으로 변경 시 킬 수 있다.

그렇기에, 이를 다른 값으로 변경하기 위해서는, 원본데이터를 변경하지 않고, 그 데이터의 복사본을 만들어서 일부 데이터를 변경하고, 복사한 데이터를 사용해서 작업을 하기 때문에, 기존에 원본 데이터는 변하지 않는 것이다.

- 함수형 프로그래밍에서는 데이터는 변하지 않는 불변성을 유지해야한다.
- 데이터 변경이 필요한 경우, 원본데이터는 그대로 두고, 복사본을 만들어서, 복사한 데이터를 변경하고, 사용해 작업을 한다.

코드를 살펴보자.

```js
let person = {
    name: "choi",
    age: 28
};

function increase(person) {
    person.age = person.age + 1;
    return person;
}
```

위와 같은 형태는 불변성을 지켜지고 있는 코드 일까?

정답은 아니다.

increase 함수는 전역으로 선언된 person의 age를 변경하므로 불변성을 지키지 못한 코드이다.

그렇다면 불변성을 지키는 코드는 어떠한 형태를 띄고 있을까?

```js
const person = {
    name: "choi",
    age: 28
};

function increase(person) {
    const copyPerson = {
        ...person,
        age: person.age + 1
    };

    return copyPerson
}

const result = increase(person);

console.log(result); // person: {name: "choi", age: 29}
```

위오 같은 형태는, 인자로 전달받은 person에 대해서, copyPerson이라는 복사본을 만들어, age를 변경 하였다.

그렇기 때문에 기존에 전역변수인 person은 값이 변경되지 않고 그대로 원본의 데이터를 유지하고 있기에 불변성을 유지 했다고 할 수 있다.

#### 3. 1급객체

1급 객체란, 매개변수나 리턴값으로 주고받을 수 있는 객체를 말한다. javascript에서 사용되는 모든 값과 함수는 변수에 저장할 수 있으므로 1급 객체에 해당된다.

- 변수나 데이터 구조안에 담을 수 있다.
- 파라미터로 전달할 수 있다.
- return 값으로 사용 할 수 있다.

코드를 살펴보자.

```js
function increase(num) {
    return num + 1;
}

function multiply(num) {
    return num * 2;
}

function transform(num) {
  return num.map(item => {
      return increase(item);
  }).map(item => {
      return multiply(item);
  });
}

const calcArray = transform([1,2,3,4]);
console.log(calcArray); // [4, 6, 8, 10]
```

위의 코드를 살펴보면, transform이라는 함수에서, map으로 반복을 수행 할 때, return의 값으로 함수를 반환 하기 때문에 1급 객체의 특징을 띄고 있다.

#### 4. 고차 함수 (High Order Function)

1급 객체에서, 함수를 변수에 지정할 수 있다고, 설명 하였다. 이러한 함수를 매개변수로 전달받거나, 리턴값을 함수로 반환할 경우 이를 고차 함수 (High Order Function) 이라 부른다.

- 함수를 인자로써 전달 할 수 있어야 한다.
- 함수의 반환 값으로 또 다른 함수를 사용할 수 있다.

그렇다면 고차함수에 대한 코드를 살펴보자.

```js
const addInfo = (name) => {
     return function (age) {
         return name + age;
     }
}
const getInfo = addInfo("choi")
const info = getInfo(28);

console.log(info); // choi28
```

위와 같이 함수의 반환 값으로, 다른 함수를 사용하거나, 또 다른 함수를 사용할 수 있어야 한다.

### 마치며

이번에는, 함수형 프로그래밍 개발 패러다임에 대한, 개념과 주요 특징 그리고 예제코드를 통해 알아보았으며, 함수형 프로그래밍과의 비교를 통해 객체지향 프로그래밍에 대해서도 간단하게 알아보았다.

이로써 나는 누군가가 "함수형 프로그래밍이 뭐야?" 라고 물어본다면 이제는 위에 설명 한 것 처럼, 내가 공부한 내용에 대해 상세히 알려 줄 수 있을 것 같다.

# 블로그 링크

> https://dlsgh120.tistory.com/63