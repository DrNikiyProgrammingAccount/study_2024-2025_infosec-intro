---
## Front matter
title: "Отчёт о лабораторной работе"
subtitle: "Лабораторная работа 1"
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

Целью данной работы является приобретение практических навыков установки операционной системы на виртуальную машину, настройки минимально необходимых для дальнейшей работы сервисов.

# Выполнение лабораторной работы

Для начала укажем имя виртуальной машины и укажем загрузочный диск (рис. [-@fig:001]).

![Первичная настройка машины](image/1.png){#fig:001}

Укажем 4096мб оперативной памяти и 8 ядер процессора (рис. [-@fig:002]).

![Задача виртуальных ресурсов](image/2.png){#fig:002}

Создадим виртуальный жёсткий диск размером 40гб (рис. [-@fig:003]).

![Установка виртуального жёсткого диска](image/3.png){#fig:003}

Запустим ВМ, и выберем способ установки как Server with GUI и установим development tools (рис. [-@fig:004]).

![Способ установки ВМ](image/4.png){#fig:004}

Выберем диск для установки диск (рис. [-@fig:005]).

![Выбор диска](image/5.png){#fig:005}

Далее настроим Network (рис. [-@fig:006]).

![Настройка Network](image/6.png){#fig:006}

Создадим пользователя с правами администратора (рис. [-@fig:007]).

![Создание пользователя](image/7.png){#fig:007}

И отключим kdump (рис. [-@fig:008]).

![Отключение kdump](image/8.png){#fig:008}

Зададим пароль для root (рис. [-@fig:009]).

![Пароль для root](image/9.png){#fig:009}

После этого установим систему. После перезагрузки установим vbox guest additions (рис. [-@fig:010]).

![Установка vbox guest additions](image/10.png){#fig:010}

С помощью dmesg посмотрим на версию ядра (рис. [-@fig:011]).

![dmesg](image/11.png){#fig:011}

С его же помощью посмотрим частоту процессора, модель процессора, кол-во оперативной памяти, гипервизор, и типы файловых систем и их порядок загрузки (рис. [-@fig:012]).

![dmesg](image/12.png){#fig:012}

# Выводы

В результате выполнения лабораторной работы была установлена и настроена виртуальная машина

# Список литературы{.unnumbered}

::: {#refs}
:::
