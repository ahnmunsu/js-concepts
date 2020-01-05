# Javascript 개념 정리
https://github.com/leonardomso/33-js-concepts을 참고하여 자바 스크립트 개발자가 알아야할 개념을 정리했다.

---

## 목차
1.  **[Call Stack](#call-stack)**
1.  **[Primitive Types](#primitive-types)**
1.  **[Value Types and Reference Types](#value-types-and-reference-types)**
1.  **[Implicit, Explicit, Nominal, Structuring and Duck Typing](#implicit-explicit-nominal-structuring-and-duck-typing)**
1.  **[== vs === vs typeof](#-vs--vs-typeof)**
1.  **[Function Scope, Block Scope and Lexical Scope](#function-scope-block-scope-and-lexical-scope)**
1.  **[Expression vs Statement](#expression-vs-statement)**
1.  **[IIFE, Modules and Namespaces](#iife-modules-and-namespaces)**
1.  **[Message Queue and Event Loop](#message-queue-and-event-loop)**
1.  **[setTimeout, setInterval and requestAnimationFrame](#settimeout-setinterval-and-requestanimationframe)**
1.  **[JavaScript Engines](#javascript-engines)**
1.  **[Bitwise Operators, Type Arrays and Array Buffers](#bitwise-operators-type-arrays-and-array-buffers)**
1.  **[DOM and Layout Trees](#dom-and-layout-trees)**
1.  **[Factories and Classes](#factories-and-classes)**
1.  **[this, call, apply and bind](#this-call-apply-and-bind)**
1.  **[new, Constructor, instanceof and Instances](#new-constructor-instanceof-and-instances)**
1.  **[Prototype Inheritance and Prototype Chain](#prototype-inheritance-and-prototype-chain)**
1.  **[Object.create and Object.assign](#objectcreate-and-objectassign)**
1.  **[map, reduce, filter](#map-reduce-filter)**
1.  **[Pure Functions, Side Effects and State Mutation](#pure-functions-side-effects-and-state-mutation)**
1.  **[Closures](#closures)**
1.  **[High Order Functions](#high-order-functions)**
1.  **[Recursion](#recursion)**
1.  **[Collections and Generators](#collections-and-generators)**
1.  **[Promises](#promises)**
1.  **[async/await](#asyncawait)**
1.  **[Data Structures](#data-structures)**
1.  **[Expensive Operation and Big O Notation](#expensive-operation-and-big-o-notation)**
1.  **[Algorithms](#algorithms)**
1.  **[Inheritance, Polymorphism and Code Reuse](#inheritance-polymorphism-and-code-reuse)**
1.  **[Design Patterns](#design-patterns)**
1.  **[Partial Applications, Currying, Compose and Pipe](#partial-applications-currying-compose-and-pipe)**
1.  **[Clean Code](#clean-code)**

---

## Call Stack
...
**[⬆ 목차](#목차)**

---

## Primitive Types
*  Number
*  String
*  Boolean
*  Null
*  Undefined
*  Ojbect
### Number
#### 정수
```
var decimalNum = 100; // 기본 숫자 리터럴 형식 10진수로 초기화
var octalNum = 010; // 8진수로 초기화
var hexNum = 0x10; // 16진수로 초기화
```
#### 부동소수점
```
var floatNum1 = 3.14;
var floatNum2 = 3.125e7;
```
##### 부동소수점 사칙연산 부정확
0.1 + 0.2 결과는 0.30000000000000004로 아래 코드는 의도대로 동작하지 않는다.
```
var f1 = 0.1;
var f2 = 0.2;

if (f1 + f2 == 0.3) {
    do_something();
}
```
#### 숫자 범위
*  최소값 : Number.MIN_VALUE (5e-324)
*  최대값 : Number.MAX_VALUE (1.7976931348623157e+308)
*  최소, 최대를 벗어나면 양수는 Infinity, 음수는 -Infinity로 변환된다.
#### NaN
*  Not-a-Number의 줄임말
*  값이 숫자가 아님을 뜻한다.
*  숫자를 0으로 나눈 경우 결과 값이 NaN이다.
*  NaN == NaN은 false이다.
*  isNaN 함수를 사용하여 검사한다.
#### 문자열을 숫자로 변환하는 함수
*  Number()
*  parseInt()
*  parseFloat()

### String
*  텍스트 데이터를 나타내는데 사용한다.
*  16비트 부호없는 정수 값 요소들의 집합이다.
*  String 의 길이는 String이 가지고 있는 요소의 갯수이다.
*  문자열이 생성되면, 그 문자열을 수정할 수 없다.
*  기존 문자열을 String.substr(), String.concat() 같은 method나 접합 연산자(+)를 사용해 새로운 문자열을 만든다.
#### 문자열로 변환하는 함수
*  toString() method는 값에 해당하는 문자열을 반환한다.
```
var hundred = 100;
var hundred_string = hundred.toString(); // 문자열 "100"
var is_true = true;
var is_true_string = is_true.toString(); // 문자열 "true"
var hex_num = 10;
var hex_num_string = hex_num.toString(16); // 16진수 문자열 "a"
```
*  String() 함수는 null이나 undefined도 사용 가능하다. (*toString은 불가능*)
```
var im_null = null;
var im_null_string = String(im_null); // 문자열 "null"
var im_undefined = null;
var im_undefined_string = String(im_undefeind); // 문자열 "undefined"
```

### Boolean
### Null
### Undefined
### Symbol
**[⬆ 목차](#목차)**

---

## Value Types and Reference Types
...
**[⬆ 목차](#목차)**

---

## Implicit, Explicit, Nominal, Structuring and Duck Typing
...
**[⬆ 목차](#목차)**

---

## == vs === vs typeof
...
**[⬆ 목차](#목차)**

---

## Function Scope, Block Scope and Lexical Scope
...
**[⬆ 목차](#목차)**

---

## Expression vs Statement
...
**[⬆ 목차](#목차)**

---

## IIFE, Modules and Namespaces
...
**[⬆ 목차](#목차)**

---

## Message Queue and Event Loop
...
**[⬆ 목차](#목차)**

---

## setTimeout, setInterval and requestAnimationFrame
...
**[⬆ 목차](#목차)**

---

## JavaScript Engines
...
**[⬆ 목차](#목차)**

---

## Bitwise Operators, Type Arrays and Array Buffers
...
**[⬆ 목차](#목차)**

---

## DOM and Layout Trees
...
**[⬆ 목차](#목차)**

---

## Factories and Classes
...
**[⬆ 목차](#목차)**

---

## this, call, apply and bind
...
**[⬆ 목차](#목차)**

---

## new, Constructor, instanceof and Instances
...
**[⬆ 목차](#목차)**

---

## Prototype Inheritance and Prototype Chain
...
**[⬆ 목차](#목차)**

---

## Object.create and Object.assign
...
**[⬆ 목차](#목차)**

---

## map, reduce, filter
...
**[⬆ 목차](#목차)**

---

## Pure Functions, Side Effects and State Mutation
...
**[⬆ 목차](#목차)**

---

## Closures
...
**[⬆ 목차](#목차)**

---

## High Order Functions
...
**[⬆ 목차](#목차)**

---

## Recursion
...
**[⬆ 목차](#목차)**

---

## Collections and Generators
...
**[⬆ 목차](#목차)**

---

## Promises
...
**[⬆ 목차](#목차)**

---

## async/await
...
**[⬆ 목차](#목차)**

---

## Data Structures
...
**[⬆ 목차](#목차)**

---

## Expensive Operation and Big O Notation
...
**[⬆ 목차](#목차)**

---

## Algorithms
...
**[⬆ 목차](#목차)**

---

## Inheritance, Polymorphism and Code Reuse
...
**[⬆ 목차](#목차)**

---

## Design Patterns
...
**[⬆ 목차](#목차)**

---

## Partial Applications, Currying, Compose and Pipe
...
**[⬆ 목차](#목차)**

---

## Clean Code
...
**[⬆ 목차](#목차)**

---
