---
## Front matter
title: "Отчет по индивидуальному проекту этап 5"
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


# Задание

1. Сделайте записи для профессиональных проектов.

2. Сделайте пост по прошедшей неделе.

3. Добавить пост на тему по выбору.

# Выполнение лабораторной работы

Оформеляеи файл  с записями рофессиональных проектов.

![рофессиональных проектов](image/1.png){#fig:001 width=70%}

Мы вносим изменения на сервер

![изменения](image/2.png){#fig:002 width=70%}

Давайте напишем пост о прошлой неделе.

![пост о прошлой неделе.](image/3.png){#fig:003 width=70%}

Выкладываем на сайт. 

![.](image/4.png){#fig:004 width=70%}

Делаем пост на тему 

![Языки научного программирования](image/5.png){#fig:005 width=70%}

Выкладываем на сайт. 

![Языки научного программирования](image/6.png){#fig:006 width=70%}


# Выводы

Добавлены необходимые изменения на сайт,

# Список литературы{.unnumbered}

::: {#refs}
:::
