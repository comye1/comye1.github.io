---
layout: post
title: 파이썬-장고(python-Django)-배운-내용-대충-정리중
description: 파이썬 장고 
author: comye1
category: Misc
tags: python Django Web Backend
finished: true
---

### 1. 데이터구조 정의하기(모델링)
> model 정의 -> make migration -> migrate

### 2. 관리자 및 페이지 생성 
> createsuperuser
>admin.py -> register
> admin.ModelAdmin 클래스 커스터마이징

### 3. 템플릿
> Template -- 렌더, HTML 보여줌

### 4. 경로 만들기 
> view.py에 함수 추가
> template 폴더 내에 html 파일 생성
> render
> url.py에 경로 추가

### 5. 링크 만들기
> include->app의 자체 urls 파일에서 경로 관리

> 링크 {% url "app:name" %}

### 6. 템플릿 사용(상속, block)
> html 템플릿 -> template > base.html
> settings.py -> TEMPLATES에 경로 지정

> base.html
> {% block content %}
> {% endblock %}

> main.html
> {% extends 'base.html' %}

> 들어갈 내용을
> {% block content %}
> {% endblock %}
> 로 감싼다

### 7. CSS 입히기
> STATIC_URL
> STATICFILES_DIRS
> ==> 공통 css, js,,
> {% load static %}
> href = "{% static 'css/project.css' %}"
