---
layout: page
title: Java
subtitle: Java Spring Framework
summary: Spring 마이크로 서비스 배우기 
categories: Language
tags: Java
featured-img: emile-perron-190221
mathjax: true
comments: Spring All in One
---

# Introducing Java !!
##### (Universal Language)

---

## Overview

> 자바(영어: Java, 문화어: 자바)는 썬 마이크로시스템즈의 제임스 고슬링(James Gosling)과 다른 연구원들이 개발한 객체 지향적 프로그래밍 언어이다.  
> <small> *1991년 그린 프로젝트(Green Project)라는 이름으로 시작해 1995년에 발표했다.* </small>

---

## Contents

### Table of Contents

|No|Titile|Remarks|
|--:|:-:|:--|
|0|[환경설정](#install)|환경설정|
|1|[강의내용](#syllabus)|강의내용|

---

## Get Started(`Java`)

<a name="install"/>

* [OpenJDK9](http://jdk.java.net/java-se-ri/9)
* [IJava](https://github.com/SpencerPark/IJava)

> Jupyter에 Java Kernel을 설치하는 방법
> IJava는 JDK >= 9 로 되어 있으나 실제 JDK=9에서만 돌아가는 것으로 보인다.
> 설치하는 방법도 python 컴파일 방법으로는 잘 동작하지 않으니 실제 binary파일을 받고 설치하는것이 좋다.
> jupyter kernelspec list

* [IJava release](https://github.com/SpencerPark/IJava/releases)

```python
# Pass the -h option to see the help page
python3 install.py -h

# Otherwise a common install command is
python3 install.py --sys-prefix
```

---

## Data & Source

### Table of Data & Source

|No|Title|Remarks|
|--:|:-:|:--|
|0|[jsoup.ipynb](https://github.com/shpimit/shpimit.github.io/tree/master/blog/Java/src/jsoup.ipynb)|WebCrawling|

---

### 2. Syllabus

<a name="syllabus"/>

1. 지난 학습 정리
* 코딩을 배워야 하는 이유(동영상)
* 미래의 언어 코딩(동영상)
2. 날짜와 시간 & 형식
3. 컬렉션
4. 지네릭스, 열거형, 어노테이션
* Junit
* 성능비교, 자바성은 튜닝
5. 쓰레드
6. 람다와 스트림
* 음수표현, 메모리 디버깅
7. 입출력 I/O
8. Networking
* Restful API GET 실습
* Neural Network 예측(아라한 문서)
* 링크 소프트웨어 세상(동영상)