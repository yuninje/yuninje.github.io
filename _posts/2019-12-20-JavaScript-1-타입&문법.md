---
layout: post # 양식 
title: JavaScript 1 - 타입 & 문법 # 1 :: 글제목
tags: [JavaScript] # 분류
---

### 문법
- ### 변수 ( varable )
    ```js
    var x = 10
    console.log(x)
    ```
    ```
    10
    ```

- ### 리터럴 ( literal )
    - 직접 표현되는 값

- ### 식별자 ( identifier )
    - 변수나 함수의 이름을 작성할 때 사용되는 이름
    - 작성방식
        - Camel case
        - Underscore case
    ```js
    var fistVar = 10    // Camel Case
    var first_var = 10  // Underscore Case
    ```

- ### 키워드 ( keyword ) or 예약어 ( reserved word)
    - 특별한 용도로 사용하기 위해 미리 예약된 단어
    - 프로그램 내에서 식별자로 사용할 수 없다.

- ### 주석 ( comment )
    - 코드 내에 삽입된 일종의 설명문

    ```js
    // 한줄 주석

    /* 
        주석문
        입니다.
    */
    ```

### 타입 ( type )
- 원시 타입 ( primitive type )
    - 숫자 ( number )
    - 문자열 ( string )
    - 불리언 ( boolean )
    - undefined
    - null
    - 심볼 ( symbol ) : ECMAScript 6부터 제공됨.
        - : 봐도 모르겠음
- 객체 타입 ( object type )
    - 객체 ( object )


### Reference
- [http://tcpschool.com/javascript/intro](http://tcpschool.com/javascript/intro)