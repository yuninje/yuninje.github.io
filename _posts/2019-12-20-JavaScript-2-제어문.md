---
layout: post # 양식 
title: JavaScript 2 - 제어문 # 1 :: 글제목
tags: [JavaScript] # 분류
---

### 제어문 ( control flow statements )

- #### 조건문 ( contitional statements )
    - if
        ```js
        if( expression ){
            // statement
        }
        ```
    - if / else
        ```js
        if ( expression ){
            // statement
        } else{
            // statement
        }
        ```
    - if / else if / else
        ```js
        if ( expression ){
            // statement
        } else if ( expression ) {
            // statement
        }else{
            // statement
        }
        ```
    - switch
        ```js
        switch( 조건 값 ){
            case 값1:
                // statement
                break;
            case 값2:
                // statement
                break;
            ...
            default:
                // statement
        }
        ```
- #### 반복문 ( iteration statements )
    - while
        ```js
        while( expression ) {
            // statement
        }
        ```

    - do / while
        ```js
        do{
            // statement
        }while( expression )
        ```

    - for
        ```js
        for(초기식 ; 표현식 ; 증감식){
            // statement
        }
        ```
        
    - for in
        - 객체의 모든 열거 가능한 속성에 대해 반복
        ```js
        for( 변수 in 객체 ) {
            // 실행문
        }
        ```

    - for of
        - `[Symbol.iterator]` 속성을 가지는 컬렉션 전용
        ```js
        for( 변수 of 객체 ) {
            // 실행문
        }
        ```    
- #### 기타 제어문
    - label
        ```js
        l1:
        for(var i = 0; i< 3; i++){
            for(var j = 0; j < 3 ; j++ ){
                if(i == 1 && j == 1){
                    continue l1 // l1 for 문에 대해 continue
                    // break l1 // l1 for 문에 대해 break
                }
                console.log(i + ' ' + j)
            }
        }
        ```
        ```text
        0 0
        0 1
        0 2
        1 0
        2 0
        2 1
        2 2
        ```
    - continue
        ```js
        for(var i = 0 ; i < 3; i ++){
            if( i == 1 ){
                continue
            }
        }
        ```
    - break
        ```js
        for(var i = 0 ; i < 3; i ++){
            if( i == 1 ){
                break
            }
        }
        ```


### Reference
- [http://tcpschool.com/javascript/intro](http://tcpschool.com/javascript/intro)