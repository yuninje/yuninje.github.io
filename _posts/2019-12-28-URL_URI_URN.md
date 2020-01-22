---
# 3 :: 파일 이름 2019-12-05-XXXXXXX  
layout: post # 양식 
title: URL vs URI vs URN # 1 :: 글제목
tags: [Web] # 분류
date : 2019-12-28 20:00:00 +0900
---

### URL vs URI vs URN
- URL ( Uniform Resource Locator )
    - 네트워크 상에 존재하는 자원의 위치
- URI ( Uniform Resource Identifier )
    - 네트워크 상에 존재하는 자원을 구분하는 식별자(ID)
- URN ( Uniform Resourc Name )
    - 자원의 이름
    - 서로 중복되지 않는 유일한 값
  
![url_uri_urn-1](/img/2019-12-28-URL_URI_URN/url_uri_urn-1.png)
![url_uri_urn-2](/img/2019-12-28-URL_URI_URN/url_uri_urn-2.png)

#### URL, URN, URI 예시
- telnet://192.168.0.10:8080/ : 해당 위치로 접근하는 방법인 telnet://을 포함하므로 URL(혹은 URI)로 볼 수 있습니다.
- http://nsinc.tistory.com/ : http:// 때문에 URL(URI)라고 볼 수 있습니다.
- mailto:myname@me.com : mailto 덕분에 URL (URI)으로 볼 수 있습니다.
- urn:isbn:0451450523 : URN으로 1926년에 출간된 the Last Unicorn의 도서식별번호를 가리킵니다.
- urn:oid:2.16.840 : URN으로 미국을 의미하는 OID입니다.

### Reference
- [https://nsinc.tistory.com/192](https://nsinc.tistory.com/192)