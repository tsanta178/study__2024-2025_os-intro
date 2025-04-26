---
## Front matter
title: "Отчёт по лабораторной работе No11"
subtitle: "Операционные системы"
author: "Ракутуманандзара Цантамписедрана С."

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
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase,Scale=0.9
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

Познакомиться с операционной системой Linux. Получить практические навыки работы с редактором Emacs

# Задание

1. Основные команды emacs

2. Научиться использовать команды по перемещению курсора.

3. Управление буферами

4. Управление окнами.

5. Режим поиска

# Выполнение лабораторной работы

**1. Основные команды emacs**

Я открываю emacs и создаю файл lab07.sh с помощью комбинации Ctrl-x Ctrl-f (C-x C-f)(рис.1)

![создание файла](image/01.png){#fig:001 width=70%}

Я записываю текст в только созданный файл. Потом я сохраняю файл с помощью комбинации Ctrl-x Ctrl-s (C-x C-s)(рис.2)

![запись в файле](image/03.png){#fig:001 width=70%}

Я вырезаю одной командой целую строку(С-k)(рис.3)

![выразание строки](image/04.png){#fig:001 width=70%}

Я вставлю эту строку в конец файла с помощью С-у(рис.4)

![вставление строки](image/05.png){#fig:001 width=70%}

Я выделяю область текста с помощью С-space(рис.5)

![выделение текста](image/07.png){#fig:001 width=70%}

Я скопирую область в буфер обмена (M-w) и вставливаю область в конец файла(рис.6)

![копирование текста](image/08.png){#fig:001 width=70%}

Я ещё раз выделяю эту область и на этот раз вырезаю её(С-w)(рис.7)

![выделение и вырезание текста](image/09.png){#fig:001 width=70%}

Потом я отменяю последнее действие(рис.8)

![отменение последнее действие](image/10.png){#fig:001 width=70%}

**2. Научиться использовать команды по перемещению курсора.**

Сначала я перемещаю курсор в начало строки с помощью С-а(рис.9)

![перемешение курсора в начало строки](image/11.png){#fig:001 width=70%}

После этого я перемещаю курсор в конец строки(С-е)(рис.10)

![перемешение курсора в конец строки](image/12.png){#fig:001 width=70%}

Затем я перемещаю курсор в начало буфера с помощью M(alt)-<(рис.11)

![перемешение курсора в начало буфера](image/13.png){#fig:001 width=70%}

Потом я перемещаю курсор в конец буфера(M->)(рис.12)

![перемешение курсора в конец буфера](image/14.png){#fig:001 width=70%}

**3. Управление буферами**

Я выведу список активных буферов на экран (C-x C-b)(рис.13)

![список активных буферов](image/15.png){#fig:001 width=70%}

Я перемещаю во вновь открытое окно "(C-x) o" со списком открытых буферов и переключаюсь на другой буфер(рис.14)

![перемешение на буфером](image/16.png){#fig:001 width=70%}

После этого я закрываю это окно (C-x 0)(рис.15)

![закрытие окна](image/17.png){#fig:001 width=70%}

Открываю другой буфер без вывода их списка на экран с помощью C-x b(рис.16)

![Открытие другого буфера](image/24.png){#fig:001 width=70%}

**4. Управление окнами.**

Я поделяю фрейм на 4 части: разделяю фрейм на два окна по вертикали (C-x 3), а затем каждое из этих окон на две части по горизонтали (C-x 2)(рис.17)

![разделение фрейма](image/18.png){#fig:001 width=70%}

В каждом из четырёх созданных окон, я открываю новый буфер (файл) и введу несколько строк текста(рис.18)

![открытие и запись в файла](image/19.png){#fig:001 width=70%}
 
**5. Режим поиска**

Я переключаюсь в режим поиска (C-s) и наиду несколько слов, присутствующих в тексте(рис.19)

![поиск слова](image/20.png){#fig:001 width=70%}

Я выхожу из режима поиска, нажав C-g(рис.20)

![выход из режима поиска](image/21.png){#fig:001 width=70%}

Перехожу в режим поиска и замены с помощью M-%, ввожу какое слово хочу заменить, затем ввожу на какое хочу заменить(рис.21)

![Замена слова](image/26.png){#fig:001 width=70%}

С помощью M-s о перехожу в другой режим поиска. Он отличается от предыдущего тем, что выводит результат в отдельном окне от окна буфера и даёт полную строку где слова содержить(рис.22)

![Режим поиска](image/27.png){#fig:001 width=70%}

# Выводы

Выполняя эту лабораторную работу познакомилася с операционной системой Linux и получила практические навыки работы с редактором Emacs

# Список литературы{.unnumbered}

лабораторная работа No11
