---
## Front matter
title: "Отчёт о лабораторной работе"
subtitle: "Проект стадия 2"
author: "Андрюшин Никита Сергеевич"

## Generic otions
lang: ru-RU
toc-title: "Содержание"

## Bibliography
bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl

## Pdf output format
toc: true # Table of contents
toc-depth: 2
lof: true # List of figures
lot: true # List of tables
fontsize: 12pt
linestretch: 1.5
papersize: a4
documentclass: scrreprt
## I18n polyglossia
polyglossia-lang:
  name: russian
  options:
	- spelling=modern
	- babelshorthands=true
polyglossia-otherlangs:
  name: english
## I18n babel
babel-lang: russian
babel-otherlangs: english
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
## Biblatex
biblatex: true
biblio-style: "gost-numeric"
biblatexoptions:
  - parentracker=true
  - backend=biber
  - hyperref=auto
  - language=auto
  - autolang=other*
  - citestyle=gost-numeric
## Pandoc-crossref LaTeX customization
figureTitle: "Рис."
tableTitle: "Таблица"
listingTitle: "Листинг"
lofTitle: "Список иллюстраций"
lotTitle: "Список таблиц"
lolTitle: "Листинги"
## Misc options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Установить DVWA

# Выполнение лабораторной работы

Вводим предложенную на странице гитхаба команду для автоматической установки. Начнётся установка, и сначала установится php-gd (рис. [-@fig:001]).

![Ввод команды](image/1.png){#fig:001}

Далее идёт настройка базы данных. Вводим данные от root (рис. [-@fig:002]).

![Настройка mariaDB](image/2.png){#fig:002}

После этого переходим на предложенный адрес localhost/dvwa и нажимаем на reset database (рис. [-@fig:003]).

![Переход на сайт](image/3.png){#fig:003}

После этого авторизируемся по тем данным, что были выведены на скриншоте 2 (рис. [-@fig:004]).

![Авторизация](image/4.png){#fig:004}

И мы заходим на настроенный сайт (рис. [-@fig:005]).

![Настроенный сайт](image/5.png){#fig:005}

# Выводы

Был настроен dvwa

# Список литературы{.unnumbered}

::: {#refs}
:::
