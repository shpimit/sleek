---
layout: page
title: Microservice OAuth2
summary: Microservice OAuth2 is space to learn with OAuth2.
categories: Java
tags: Java
featured-img: microservice
comments: 마이크로 서비스 (with OAuth2)
---

# Introducing Microservice OAuth2 !!

#####  Microservice OAuth2 is space to learn with OAuth2.

---

## Contents

### Table of Contents

|No|Title|Remarks|
|-:|:--:|:--|
|0|[환경설정](#get-started)|OAuth2환경셋팅|
|1|[실습](#practice)|실습|

---

## Learning

### Table of Learning

|No|구분|Title|Day|Remarks|
|-:|:-:|:--:|:-:|:--|
|1|블로그|Spring Boot로 만드는 OAuth2 시스템|2021.03.01|`Spring Security`|

---

## Get Started(`OAuth2`)

### 목적 : OAuth2 서버를 만드는 목적

> 규모 있는 회사 및 공공기관에서 OAuth2 형태로 인증시스템을 구현하게 되면 보통 회사에서 사용하는 인증시스템(LDAP 또는 조금 다르지만 SSO등) 보다 연동하여 개발하기가 훨씨 더 수월하고 관리하기 쉬워진다. 그리고 다른 인증시스템과 다르게 권한도 가지고 있다.
> 

##### [Go to Contents](#contents)

---

## Practice

### 1. 대칭키 생성 방법

```shell
$ keytool -genkeypair -alias oauth2jwt -keyalg RSA -keypass oauth2jwtpass -keystore oauth2jwt.jks -storepass oauth2jwtpass

이름과 성을 입력하십시오.
  [Unknown]:
조직 단위 이름을 입력하십시오.
  [Unknown]:
조직 이름을 입력하십시오.
  [Unknown]:
구/군/시 이름을 입력하십시오?
  [Unknown]:
시/도 이름을 입력하십시오.
  [Unknown]:
이 조직의 두 자리 국가 코드를 입력하십시오.
  [Unknown]:
CN=Unknown, OU=Unknown, O=Unknown, L=Unknown, ST=Unknown, C=Unknown이(가) 맞습니까?
  [아니오]:  y
```
### 2. Public.key 생성 방법

```shell
keytool -list -rfc --keystore oauth2jwt.jks | openssl x509 -inform pem -pubkey
키 저장소 비밀번호 입력:  oauth2jwtpass
```

---

## Reference

### Spring OAuth2

* [아빠 SpringBoot2로 OAuth2 서버 만들기](https://daddyprogrammer.org/post/1239/spring-oauth-authorizationserver/)
* [Authorization Server(인증서버) 구축하기](https://lemontia.tistory.com/927#recentEntries)
* [OAuth2 테스트: Spring Boot with OAuth2 - 1. OAuth2 Server 구현](https://parandol.tistory.com/4)
* [Spring Security OAuth2 Login Flow](https://jyami.tistory.com/121)
* [AuthenticationProvider](https://dkyou.tistory.com/20?category=877213)
* [Spring Boot로 만드는 OAuth2 시스템](https://brunch.co.kr/@sbcoba/1)
* [Spring Boot Validation을 사용하여 요청 값 검증하기](https://shinsunyoung.tistory.com/43)

### Keycloak

* [Keycloak을 통해 Spring Boot에서 개별 리소스 보호](https://recordsoflife.tistory.com/465)
* [Custom Provider](https://www.baeldung.com/java-keycloak-custom-user-providers)
* [Java SPI](https://www.baeldung.com/java-spi)
* [MSA 인증 서비스 Keycloak User Storage SPI](https://subji.github.io/posts/2020/07/24/keycloak3)
* [Keycloack Custom Login](https://www.baeldung.com/keycloak-custom-login-page)
* [Customizing Themes for Keycloak](https://www.baeldung.com/spring-keycloak-custom-themes#customization-example)
* [How to run Keycloak in HA on Kubernetes](https://blog.sighup.io/keycloak-ha-on-kubernetes/)
* [Baeldung Resource](https://www.baeldung.com/spring-security-oauth-resource-server)
* [MSA 인증 서비스 Keycloak 소개](https://subji.github.io/posts/2020/07/08/keycloak1)
* [Keycloak & Springboot 적용기](https://dkyou.tistory.com/54?category=877212)
* [버전 걱정 없는 SSO 구현 번역해보기](https://dkyou.tistory.com/45?category=877213)
* [Keycloak 공식문서 따라해보기](https://dkyou.tistory.com/48?category=877212)
* [Keycloak Embedded in a Spring Boot Application](https://www.baeldung.com/keycloak-embedded-in-spring-boot-app)
* [Keycloak Embedded in a Spring Boot Application: Github](https://github.com/Baeldung/spring-security-oauth/tree/master/oauth-rest/oauth-authorization-server)
* [Keycloak과 Jenkins연결](https://tech.osci.kr/2020/04/04/91699412/)
* [Keycloak를 이용한 SSO 구축(web + wifi + ssh)](https://tech.socarcorp.kr/security/2019/07/31/keycloak-sso.html)

### SSO

* [백엔드-개발자-로드맵-따라가기-10.-OAuth2.0](https://velog.io/@skysoo/백엔드-개발자-로드맵-따라가기-10.-OAuth2.0)
* [aop를 이용한 oauth2 캐시 적용하기](https://woowabros.github.io/experience/2019/03/05/aop-oauth2-redis.html)
* [스프링부트 SSO](https://kimseungjae.tistory.com/15)
* [JWT 토큰은 어디에 저장하는게 좋을까?](https://lazyhoneyant.tistory.com/7)
* [https://brunch.co.kr/@springboot/491](https://brunch.co.kr/@springboot/491)
* [여러개의 Client에서 Resource서버 접근하게 하기](https://myeongjae.kim/blog/2020/02/01/spring-oauth-2-resource-server-handle-multiple-auth-server-tokens)
* [thymeleaf 로그인 화면](https://blog.neonkid.xyz/237)
* [https://velog.io/@yaytomato/프론트에서-안전하게-로그인-처리하기](https://velog.io/@yaytomato/프론트에서-안전하게-로그인-처리하기)

### Spring Session

* [이중화된 시스템 Redis를 통한 Spring security session관리](https://recordsoflife.tistory.com/31)
* [Spring Session and Spring Security](https://velog.io/@devsh/Spring-Session-Data-Redis-적용하기)
* [https://velog.io/@devsh/Spring-Session-Data-Redis-적용하기](https://velog.io/@devsh/Spring-Session-Data-Redis-적용하기)
* [Redis-Lettuce를-이용한-간단한-API-제작](https://ozofweird.tistory.com/entry/Spring-Boot-Redis-Lettuce를-이용한-간단한-API-제작)
* [Jedis 보다 Lettuce 를 쓰자](https://jojoldu.tistory.com/418)
* [Spring Boot + Redis로 Session Clustering 구성하기](https://sup2is.github.io/2020/07/15/session-clustering-with-redis.html)
* [Spring 라이브러리를 이용한 세션 관리](https://androids.tistory.com/54)
* [Spring MVC session](https://androids.tistory.com/54)
* [spring session](https://github.com/eugenp/tutorials/tree/master/spring-security-modules/spring-session)
* [다중 서버 환경에서 Session은 어떻게 공유하고 관리할까](https://hyuntaeknote.tistory.com/8)
* [서버가 여러대면 로그인 정보는 어디에 저장할까?](https://tjdrnr05571.tistory.com/3)
* [https://velog.io/@ehdrms2034/Spring-Security-JWT-Redis를-통한-회원인증허가-구현](https://velog.io/@ehdrms2034/Spring-Security-JWT-Redis를-통한-회원인증허가-구현)
* [https://sup2is.github.io/2020/07/15/session-clustering-with-redis.html](https://sup2is.github.io/2020/07/15/session-clustering-with-redis.html)

### Kafka

* [logback-kafka](https://ckddn9496.tistory.com/90)

### Fluentd

* [Windows에 Ruby 설치](https://park-jongseok.github.io/languages/ruby/2019/10/03/installing-ruby.html)
* [Fluentd를 이용한 로그 수집 -1.Fluentd란?](https://dev-life.tistory.com/2)

### Spring Batch

* [https://github.com/jojoldu/spring-batch-in-action/blob/master/2_Job생성.md](https://github.com/jojoldu/spring-batch-in-action/blob/master/2_Job생성.md)

### Webflux

* [WebClient 사용해보기](https://akageun.github.io/2019/06/23/spring-webflux-4-webclient.html)
* [RestTemplate 말고 WebClient](https://juneyr.dev/2019-02-12/resttemplate-vs-webclient)
* [스프링 부트 RestTemplate, WebClient](https://engkimbs.tistory.com/808)
* [RestTemplate 활용 1 - 응답 타입 일반화](https://preamtree.tistory.com/167)
* [spring web security를 이용한 로그인 처리 - 로그인과 로그아웃 처리](https://bin-repository.tistory.com/129)
* [RestTemplate (정의, 특징, URLConnection, HttpClient, 동작원리, 사용법, connection pool 적용)](https://sjh836.tistory.com/141)
* [쿠키 저장 및 조회 from JAVA](https://androi.tistory.com/356)

### RestAPI

* [REST API](https://meetup.toast.com/posts/92)
  
##### [Go to Contents](#contents)

$ keytool -genkeypair -alias oauth2jwt -keyalg RSA -keypass oauth2jwtpass -keystore oauth2jwt.jks -storepass oauth2jwtpass

$ keytool -list -rfc --keystore oauth2jwt.jks | openssl x509 -inform pem -pubkey
키 저장소 비밀번호 입력:  oauth2jwtpass
-----BEGIN PUBLIC KEY-----
MIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEArJerQDKo7Vwl2an9UEZD
9npx8vXoB+setdeZn5OKEntdpdXMdc1KE07Q8aejXnEdzTHqeWxfdctyJ0FZzphX
PSfw8IzjjElmi4GoM5Aqh0ecPUjRrSHrE3EXwxagfoRy1igfD5ALCH7VIOvf3erU
QKhAY+ARdQzNn2+d1V9y6atnPPwbjflm2Ke+S9K+Q+dvIpIbotRG7rJqO9RSn89Q
E6CcNP0LhaL6FFt9mtCEtOAlZyJHLO/CJ51XQzfGP4cYXCUQT5TC0yRKmPlRuurE
gfgmiAYl6XD1o3iui3vEJzNLN9nrbte4rjc+Rqv3aE23hu3f8QImNzdSZo6HJhQC
NwIDAQAB
-----END PUBLIC KEY-----
-----BEGIN CERTIFICATE-----
MIIDdzCCAl+gAwIBAgIEJg3+SjANBgkqhkiG9w0BAQsFADBsMRAwDgYDVQQGEwdV
bmtub3duMRAwDgYDVQQIEwdVbmtub3duMRAwDgYDVQQHEwdVbmtub3duMRAwDgYD
VQQKEwdVbmtub3duMRAwDgYDVQQLEwdVbmtub3duMRAwDgYDVQQDEwdVbmtub3du
MB4XDTE5MDQyNjE1MjAzMloXDTE5MDcyNTE1MjAzMlowbDEQMA4GA1UEBhMHVW5r
bm93bjEQMA4GA1UECBMHVW5rbm93bjEQMA4GA1UEBxMHVW5rbm93bjEQMA4GA1UE
ChMHVW5rbm93bjEQMA4GA1UECxMHVW5rbm93bjEQMA4GA1UEAxMHVW5rbm93bjCC
ASIwDQYJKoZIhvcNAQEBBQADggEPADCCAQoCggEBAKyXq0AyqO1cJdmp/VBGQ/Z6
cfL16AfrHrXXmZ+TihJ7XaXVzHXNShNO0PGno15xHc0x6nlsX3XLcidBWc6YVz0n
8PCM44xJZouBqDOQKodHnD1I0a0h6xNxF8MWoH6EctYoHw+QCwh+1SDr393q1ECo
QGPgEXUMzZ9vndVfcumrZzz8G435ZtinvkvSvkPnbyKSG6LURu6yajvUUp/PUBOg
nDT9C4Wi+hRbfZrQhLTgJWciRyzvwiedV0M3xj+HGFwlEE+UwtMkSpj5UbrqxIH4
JogGJelw9aN4rot7xCczSzfZ627XuK43Pkar92hNt4bt3/ECJjc3UmaOhyYUAjcC
AwEAAaMhMB8wHQYDVR0OBBYEFGwU4l85+ogUly2Gv+cuzzRUvOs1MA0GCSqGSIb3
DQEBCwUAA4IBAQBaL58pMhDpSebvZFQeQkyDfc95lo/9b/+e109ryORIoX3zzbNO
O1v8By2qhjj11QS3skTv2jNE4h1wDxlF+EK6uom3Vc+yHH85/cRP6Ec9bK3+Vab7
BxE/r713L3I7rGbM0DMnTeDEDaCytN6TmwxeqJiUMePfWdKAZUV/WZeKTZxePfUf
ZK9J+FFEaua3hay2iY7s+eGPZ93rcNfrudARARdn34/coWx4lD8kh6At/K1qJrM2
7/QGMJeFP2zwBhhEhAwAN2ogad7cXOoy6OwcM0sMuZ+y5Vt2WKFLbHtRPj1V5mhk
Nq/ACKliqWctpd8P5M/4Oat+zdyR3YjnU3+r
-----END CERTIFICATE-----

$ keytool -genkeypair -alias oauth2jwt -keyalg RSA -keypass oauth2jwtpass -keystore oauth2jwt.jks -storepass oauth2jwtpass
이름과 성을 입력하십시오.
  [Unknown]:
조직 단위 이름을 입력하십시오.
  [Unknown]:
조직 이름을 입력하십시오.
  [Unknown]:
구/군/시 이름을 입력하십시오?
  [Unknown]:
시/도 이름을 입력하십시오.
  [Unknown]:
이 조직의 두 자리 국가 코드를 입력하십시오.
  [Unknown]:
CN=Unknown, OU=Unknown, O=Unknown, L=Unknown, ST=Unknown, C=Unknown이(가) 맞습니까?
  [아니오]:  y


  https://www.tutorialsbuddy.com/keycloak-secure-spring-boot-rest-api
  https://sultanov.dev/blog/migrate-from-spring-security-oauth-to-keycloak/
  https://github.com/anarsultanov/examples/blob/master/spring-boot-oauth2-keycloak/keycloak-server/pom.xml