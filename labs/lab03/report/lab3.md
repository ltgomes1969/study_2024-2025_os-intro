---
## Front matter
title: "Отчёт по лабораторной работе 3"
subtitle: "Операционные системы"
author: "Гомес Лопес Теофания"

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

Максимально упростить подготовку отчётов по лабораторным работам и познакомиться с основными возможностями разметки Markdown.


# Задание

Готовить отчёт по лабораторной работе 2

# Выполнение лабораторной работы

## Готовка отчёта по лабораторной работе №2

Сначала открываю терминал и перехожу в каталог lab02/report:

![Каталог lab03/report](image/1.png){#fig:001 width=70%}

Далее копирую файл report.md с новым названием LabWork2. Затем я редактирую файл LabWork2 с помощью gedit:

![Копирование файла](image/2.png){#fig:002 width=70%}

![Редатирование](image/3.png){#fig:003 width=70%}

Копирую файл LabWork2 в файл LabWork2.md и с помощью командой make создаю LabWork2.docx и LabWork2.pdf:

![Создание abWork2.docx и LabWork2.pdf](image/4.png){#fig:004 width=70%}

# Выводы

При выполнение данной работы я познакомилась с основными возможностями разметки Markdown.

# Список литературы{.unnumbered}

::: {#refs}
:::
