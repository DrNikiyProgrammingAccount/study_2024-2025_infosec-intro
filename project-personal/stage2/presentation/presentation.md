---
## Front matter
lang: ru-RU
title: Лабораторная работа
subtitle: Проект стадия 2
author:
  - Андрюшин Н. С. 
institute:
  - Российский университет дружбы народов, Москва, Россия
date: 01 января 1970

## i18n babel
babel-lang: russian
babel-otherlangs: english

## Formatting pdf
toc: false
toc-title: Содержание
slide_level: 2
aspectratio: 169
section-titles: true
theme: metropolis
header-includes:
 - \metroset{progressbar=frametitle,sectionpage=progressbar,numbering=fraction}

## Fonts
mainfont: IBM Plex Serif
romanfont: IBM Plex Serif
sansfont: IBM Plex Sans
monofont: IBM Plex Mono
mathfont: STIX Two Math
mainfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
romanfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
sansfontoptions: Ligatures=Common,Ligatures=TeX,Scale=MatchLowercase,Scale=0.94
monofontoptions: Scale=MatchLowercase,Scale=0.94,FakeStretch=0.9
mathfontoptions:
---

# Информация

## Докладчик

:::::::::::::: {.columns align=center}
::: {.column width="70%"}

  * Андрюшин Никита Сергеевич
  * Студент
  * Российский университет дружбы народов

:::
::: {.column width="30%"}


:::
::::::::::::::

## Цель работы

Установить DVWA

## Ввод команды

Вводим предложенную на странице гитхаба команду для автоматической установки. Начнётся установка, и сначала установится php-gd 

![Ввод команды](image/1.png){height=60%}

## Настройка mariaDB

Далее идёт настройка базы данных. Вводим данные от root 

![Настройка mariaDB](image/2.png){height=60%}

## Переход на сайт

После этого переходим на предложенный адрес localhost/dvwa и нажимаем на reset database 

![Переход на сайт](image/3.png){height=60%}

## Авторизация

После этого авторизируемся по тем данным, что были выведены на скриншоте 2 

![Авторизация](image/4.png){height=60%}

## Настроенный сайт

И мы заходим на настроенный сайт 

![Настроенный сайт](image/5.png){height=60%}

## Выводы

Был настроен dvwa
