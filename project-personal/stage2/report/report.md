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



# Выполнение лабораторной работы

 (рис. [-@fig:001]).

![](image/1.png){#fig:001}

 (рис. [-@fig:002]).

![](image/2.png){#fig:002}

 (рис. [-@fig:003]).

![](image/3.png){#fig:003}

 (рис. [-@fig:004]).

![](image/4.png){#fig:004}

 (рис. [-@fig:005]).

![](image/5.png){#fig:005}

 (рис. [-@fig:006]).

![](image/6.png){#fig:006}

 (рис. [-@fig:007]).

![](image/7.png){#fig:007}

 (рис. [-@fig:008]).

![](image/8.png){#fig:008}

 (рис. [-@fig:009]).

![](image/9.png){#fig:009}

 (рис. [-@fig:010]).

![](image/10.png){#fig:010}

 (рис. [-@fig:011]).

![](image/11.png){#fig:011}

 (рис. [-@fig:012]).

![](image/12.png){#fig:012}

 (рис. [-@fig:013]).

![](image/13.png){#fig:013}

 (рис. [-@fig:014]).

![](image/14.png){#fig:014}

 (рис. [-@fig:015]).

![](image/15.png){#fig:015}

 (рис. [-@fig:016]).

![](image/16.png){#fig:016}

# Выводы



# Список литературы{.unnumbered}

::: {#refs}
:::
