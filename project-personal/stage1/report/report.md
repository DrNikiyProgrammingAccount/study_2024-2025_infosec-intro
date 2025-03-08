---
## Front matter
title: "Отчёт о лабораторной работе"
subtitle: "Проект стадия 1"
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

Установить Kali Linux

# Выполнение лабораторной работы

Выделим память и процессоры (рис. [-@fig:001]).

![Выделение памяти и процессоров](image/1.png){#fig:001}

Выделим диск (рис. [-@fig:002]).

![Выделение диска](image/2.png){#fig:002}

Выберим загрузочный образ и имя VM (рис. [-@fig:003]).

![Выбор образа](image/3.png){#fig:003}

После запуска выберем русский язык (рис. [-@fig:004]).

![Настройка языка](image/4.png){#fig:004}

Настроим клавишу для переключения языка (рис. [-@fig:005]).

![Клавиша переключения языка](image/5.png){#fig:005}

ВЫберем имя для компьютера (рис. [-@fig:006]).

![Имя компьютера](image/6.png){#fig:006}

Выберем имя домена (рис. [-@fig:007]).

![Имя домена](image/7.png){#fig:007}

Выберем имя пользователя (рис. [-@fig:008]).

![Имя пользователя](image/8.png){#fig:008}

Настроим пароль (рис. [-@fig:009]).

![Пароль](image/9.png){#fig:009}

Настроим часовой пояс (рис. [-@fig:010]).

![Часовой пояс](image/10.png){#fig:010}

Сделаем авто разметку дисков (рис. [-@fig:011]).

![Разметка дисков](image/11.png){#fig:011}

Выберем диск для установки (рис. [-@fig:012]).

![Диск для установки](image/12.png){#fig:012}

Подтвердим разметку (рис. [-@fig:013]).

![Подтверждение разметки](image/13.png){#fig:013}

Настроим дополнительные параметры установки (рис. [-@fig:014]).

![Дополнительные параметры установки](image/14.png){#fig:014}

Укажем раздел установки для grub (рис. [-@fig:015]).

![Grub](image/15.png){#fig:015}

Завершение установки (рис. [-@fig:016]).

![Завершение установки](image/16.png){#fig:016}

# Выводы

В результате выполнения лабораторной работы был установлен kali linux

# Список литературы{.unnumbered}

::: {#refs}
:::
