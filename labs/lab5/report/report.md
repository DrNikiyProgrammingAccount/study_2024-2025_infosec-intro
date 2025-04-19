---
## Front matter
title: "Отчёт о лабораторной работе"
subtitle: "Лабораторная работа 5"
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

Изучение механизмов изменения идентификаторов, применения
SetUID- и Sticky-битов. Получение практических навыков работы в консоли с дополнительными атрибутами. Рассмотрение работы механизма смены идентификатора процессов пользователей, а также влияние бита Sticky на запись и удаление файлов

# Выполнение лабораторной работы

Для начала создадим файл с кодом (рис. [-@fig:001]).

![Создание файла](image/1.png){#fig:001}

И запишем туда следующий код (рис. [-@fig:002]).

![Код](image/2.png){#fig:002}

Скомпилируем программу и запустим её. Как видим, она практически идентична команде id (рис. [-@fig:003]).

![Тестирование программы](image/3.png){#fig:003}

Создадим новую программу (рис. [-@fig:004]).

![Код новой программы](image/4.png){#fig:004}

также скомпилируем её и запустим (рис. [-@fig:005]).

![Запуск программы](image/5.png){#fig:005}

Теперь поменяем для скомпилированной программы владельца и установим suid (рис. [-@fig:006]).

![Смена владельца и suid](image/6.png){#fig:006}

убедимся, что изменения успешны и запустим программу. Как видим, теперь вывод e_uid равен 0, так как программа теперь запускается от имени root (рис. [-@fig:007]).

![Запуск программы](image/7.png){#fig:007}

Теперь сменим группу и установим sgid (рис. [-@fig:008]).

![Смена владельца-гуппы и sgid](image/8.png){#fig:008}

Убедимся в успешном изменении и запустим программу. Теперь e_gid равен 0, так как программу запускается от имени группы root (рис. [-@fig:009]).

![Запуск программы](image/9.png){#fig:009}

Создадим новый файл, и напишем туда код (рис. [-@fig:010]).

![Код](image/10.png){#fig:010}

Сменим для файла исходного кода владельца и уберём права для посторонних пользователей (рис. [-@fig:011]).

![Смена прав и владельца](image/11.png){#fig:011}

Скомпилируем программу и попробуем открыть исходный код (рис. [-@fig:012]).

![Компиляция и попытка открытия исходника](image/12.png){#fig:012}

Как видим, чтение запрещено (рис. [-@fig:013]).

![Отказ в чтении](image/13.png){#fig:013}

Теперь сменим для исполняемого файла владельца и установим suid (рис. [-@fig:014]).

![Смена владельца и suid](image/14.png){#fig:014}

Попробуем с помощью программы прочитать исходный код, и это успешно получается (рис. [-@fig:015]).

![Успешное чтение файла](image/15.png){#fig:015}

Попробуем прочитать файл /etc/shadow, что успешно получается (рис. [-@fig:016]).

![Чтение /etc/shadow](image/16.png){#fig:016}

Теперь посмотрим, есть ли на папке /tmp stickybit. После этого создадим отлица пользователя guest файл, куда запишем 1 слово и позволим для посторонних чтение и запись (рис. [-@fig:017]).

![Stickybit](image/17.png){#fig:017}

От лица другого пользователя пытаемся дозаписать что-то в файл, записать что-то в файл и удалить этот файл. Все операции неуспешны (рис. [-@fig:018]).

![Неуспешные операции](image/18.png){#fig:018}

Снимем Stickybit и попробуем повторить эти операции. Теперь получилось удалить файл (рис. [-@fig:019]).

![Операции без Stickybit](image/19.png){#fig:019}

# Выводы

В результате выполнения лабораторной работы были получены знания механизмов изменения идентификаторов, применения
SetUID- и Sticky-битов

# Список литературы{.unnumbered}

::: {#refs}
:::
