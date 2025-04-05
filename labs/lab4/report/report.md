---
## Front matter
title: "Отчёт о лабораторной работе"
subtitle: "Лабораторная работа 4"
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

Получение практических навыков работы в консоли с расширенными атрибутами файлов

# Выполнение лабораторной работы

Для начала посмотрим расширенные атрибуты файла file1 и убедимся, что их нет. Поставим права на запись и чтение для владельца, после чего попробуем добавить расширенный атрибут, что закончится неудачей (рис. [-@fig:001]).

![Расширенный атрибут](image/1.png){#fig:001}

Расширенный атрибут -a можно поставить только от лица супер-пользователя (рис. [-@fig:002]).

![Успешное добавление атрибута](image/2.png){#fig:002}

Убедимся в том, что атрибут добавлен. После этого попробуем что-нибудь дозаписать в файл. Операция успешна (рис. [-@fig:003]).

![Дозапись в файл](image/3.png){#fig:003}

Однако, при перезаписи операция не дозволена. Кроме того, недозволено переименование и изменение прав (рис. [-@fig:004]).

![Недозволенные операции](image/4.png){#fig:004}

Уберём атрибут (рис. [-@fig:005]).

![Удаление атрибута](image/5.png){#fig:005}

Теперь все действия доступны (рис. [-@fig:006]).

![Теперь дозволенные операции](image/6.png){#fig:006}

Добавим атрибут -i (рис. [-@fig:007]).

![Добавление атрибута -i](image/7.png){#fig:007}

Попробуем сделать те же операции. Как видим, они все запрещены (рис. [-@fig:008]).

![Недозволенные операции](image/8.png){#fig:008}

# Выводы

В результате выполнения лабораторной работы были получены навыки работы с расширенными атрибутами

# Список литературы{.unnumbered}

::: {#refs}
:::
