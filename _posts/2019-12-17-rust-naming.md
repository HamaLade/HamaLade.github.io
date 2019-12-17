---
title: "Rust naming"
date: 2019-12-17 20:56:00 -0400
categories: Rust Naming
---
### 명명법 종류

-snake_case : 단어를 전부 소문자로 적고 언더바로 구분함.  
-SCREAMING_SNAKE_CASE : 단어를 전부 대문자로 적고 언더바로 구분함.  
-CamelCase : 단어의 첫 문자만 대문자로 적으며 구분자 없음.  
   -UUID같은 약어는 한 단어로 취급하므로 Uuid로 적어야 합니다.  


### 명명 규칙

-Crates : snake_case (단어 하나만 쓰는걸 권장)  
-Modules(모듈) : snake_case  
-Types(타입) : CamelCase  
-Traits : CamelCase (타동사, 명사, 형용사를 사용하며 '-able'과 같은 접미사를 피하라)  
-Enum(열거형) : CamelCase  
-Functions, Methods(함수, 메소드) : snake_case  
    -Conversions(변환) : as_OOO, to_OOO, into_OOO  
            -as : 비용이 싸며 원본 객체에 영향이 없음.  
            -to : 비용이 비싸며 원본 객체에 영향이 없음.  
            -into : 원본 객체를 소모(Consume)함.  
-General constructors(일반 생성자) : new, new_with_OOO  
-Conversion constructors(변환 생성자) : from_OOO  
-Local variables(지역 변수) : snake_case  
-Static variables(정적 변수) : SCREAMING_SNAKE_CASE  
-Type parameters(타입 매개변수) : 대문자 하나 (예로 T, U 등)  
-Lifetimes(수명) : 짧은 소문자 (예로 'a, 'b 등)

    
[Ref](https://neurowhai.tistory.com/69)
