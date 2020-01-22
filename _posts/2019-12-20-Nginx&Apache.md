---
# 3 :: 파일 이름 2019-12-05-XXXXXXX  
layout: post # 양식 
title: Nginx & Apache # 1 :: 글제목
bigimg: /img/2019-12-20-Nginx&Apache/Nginx.png # 4 :: 제목부분에 넓게 추가되는 이미지
tags: [Web] # 분류
---


![explain](/img\2019-12-20-Nginx&Apache\2019-web-server-survey.png)

# Nginx
- 가벼움과 높은 성능을 목표로 하는 웹 서버 소프트웨어
- 러시아의 프로그래머 이고르 시쇼브(Игорь Сысоев)가 Apache의 C10K 문제를 극복하기 위해 만듬
    - C10K 문제 : 10,000개 이상의 소켓을 열게 되면 하드웨어 성능이 충분함에도 불구하고 I/O 처리 방식의 문제 때문에 프로세스가 제대로 처리하지 못하는 것
- 비동기 Event-Driven 기반의 구조로 작동
    - 다수의 연결을 효과적으로 처리가능
![event-driven-programming](/img\2019-12-20-Nginx&Apache\event-driven-programming.gif)

# Apache
- 아파치 소프트웨어 재단에서 관리하는 웹 서버 소프트웨어
- 톰캣(Tomcat), Resin 등의 웹 어플리케이션 서버와 같이 사용할 수 있다.
- Thread / Process 기반 구조
    - 요청 하나당 스레드 하나가 처리하는 구조
    - 사용자가 많으면 많은 스레드 생성, 메모리 및 CPU 낭비가 심함 ( C10K 문제 )

![thread-programming](/img/2019-12-20-Nginx&Apache/thread-programming.gif)






#### Reference
[https://medium.com/sjk5766/%EB%84%8C-%EB%AD%90%EB%8B%88-nginx-9a8cae25e964](https://medium.com/sjk5766/%EB%84%8C-%EB%AD%90%EB%8B%88-nginx-9a8cae25e964)
[https://m.blog.naver.com/jhc9639/220967352282](https://m.blog.naver.com/jhc9639/220967352282)
[https://ko.wikipedia.org/wiki/%EC%95%84%ED%8C%8C%EC%B9%98_HTTP_%EC%84%9C%EB%B2%84](https://ko.wikipedia.org/wiki/%EC%95%84%ED%8C%8C%EC%B9%98_HTTP_%EC%84%9C%EB%B2%84)
[https://ko.wikipedia.org/wiki/Nginx](https://ko.wikipedia.org/wiki/Nginx)
[https://news.netcraft.com/archives/category/web-server-survey/](https://news.netcraft.com/archives/category/web-server-survey/)