---
# 3 :: 파일 이름 2019-12-05-XXXXXXX  
layout: post # 양식 
title: Spring Boot Annotation # 1 :: 글제목
tags: [SpringBoot]  # 분류
---


## Spring Boot Annotation

- ### Spring Annotation
  - `@SpringBootTest`
    - ㅇ


- ### JPA

  - `@Entity`
    - 테이블과 링크될 클래스

  - `@Id`
    - 테이블의 Primary Key

  - `@GeneratedValue`
    - Primary Key의 생성 방식 설정

  - `@Column`
    - 테이블의 컬럼
    - 기본값이 아닌 필요한 옵션이 있을경우 사용

  - `@Transactional`
    - 

- ### Lombok Annotation

  - `@Builder`
    - 해당 클래스의 빌더 생성
  
  - `@NoArgsConstructor`
    - 기본 생성자 자동 추가
    - ( = `public Post(){}` )
  
  - `@RequiredArgsConstructor`
    - 초기화 되지않은 `final` 필드나, `@NonNull` 이 붙은 필드에 대해 생성자를 생성 
  
  - `@Getter`
    - 모든 필드에 대한 `getter` 함수 생성
  
  - `@Setter`
    - 모든 필드에 대한 `setter` 함수 생성


- ### Test Annotation

  - `@RunWith(SpringRunner.class)`
    - JUnit에 내장된 Runner 대신 지정한 클래스에서 테스트 시작이 가능

  - `@Before`
    - Junit 에서 단위 테스트가 시작되기 직전마다 수행되는 메소드
  
  - `@After`
    - Junit 에서 단위 테스트가 끝날 때마다 수행되는 메소드


