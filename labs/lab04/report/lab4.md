---
## Front matter
title: "Отчёт по лабораторной работе 4"
subtitle: "Архитектура Компьютера и Операционные системы"
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
listingTitle: "Листинг"
lofTitle: "Список иллюстраций"
lolTitle: "Листинги"
## Misc options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Цель данной работы является получением навыков правильной работы с репозиториями git.

# Задание

1. Выполнить работу для тестового репозитория.
2. Преобразовать рабочий репозиторий в репозиторий с git-flow и conventional commits.


# Выполнение лабораторной работы

## Установка git-flow

Gitflow Workflow предполагает выстраивание строгой модели ветвления с учётом выпуска проекта. Сначала я включаю репозиторий copr:

![включение copr](image/1.png){#fig:001 width=70%}

Используя dnf install скачаю gitflow:

![dnf install gitflow](image/2.png){#fig:002 width=70%}

## Установка Node.js

Для семантического версионирования и общепринятых коммитов я устанавливаю Nodejs и pnpm:

![Установка Node.js](image/3.png){#fig:003 width=70%}

![Установка pnpm](image/4.png){#fig:004 width=70%}

## Настройка Node.js

Запуская pnpm setup я добавляю каталог с исполняемыми файлами, устанавливаемыми yarn для работы с Node.js в переменную PATH:

![Запуск pnpm](image/5.png){#fig:005 width=60%}

Далее перелогинуюсь и выполняю source ~/.bashrc:

![~/.bashrc](image/6.png){#fig:006 width=60%}

## Общепринятые коммиты

Для помощи в форматировании коммитов добавляю программу commitizen:

![Добавление commitizen](image/7.png){#fig:007 width=60%}

Добавляю standard-changelog для помощи в создании логов:

![добавление standard-changelog](image/8.png){#fig:008 width=60%}

Создаю репозиторий на GitHub назову его git-extended:

![Создание git-extended](image/9.png){#fig:009 width=60%}

Я клонирую его в каталог git-extended:

![клонирование git-extended](image/10.png){#fig:0010 width=60%}

Создаю и добавляю файл README.md: 

![Добавление readme.md](image/11.png){#fig:0011 width=60%}

Делаю первый коммит и выкладываю на github:

![Первый коммит](image/12.png){#fig:0012 width=60%}

Я инициализирую pnpm:

![Инициализирование pnpm](image/13.png){#fig:0013 width=60%}

Заполняю несколько параметров пакета (файл package.json):

![Заполнение пакетов](image/14.png){#fig:0014 width=60%}

Добавляю новые файлы и выполняю коммит (указиваю тип коммит (feat)) и отправляю на гит:

![Добавление новых файлов](image/15.png){#fig:0015 width=60%}

Инициализирую git-flow и указываю ветки:

![Инициализирование git-flow](image/16.png){#fig:0016 width=60%}

Преверяю что я на ветке develop с промощью git branch:

![Проверка ветки](image/17.png){#fig:0017 width=60%}

Загружаю весь репозиторий в хранилище с помощью git push --all:

![Загрузка репозиторий](image/18.png){#fig:0018 width=60%}

Установливаю внешнюю ветку как вышестоящую для этой ветки (develop):

![установка внешней ветки](image/19.png){#fig:0019 width=60%}

Создаю релиз с версией 1.0.0 и журнал изменений (standard-changelog)::

![Создание релиза](image/20.png){#fig:0020 width=60%}

Добавляю журнал изменений в индекс:

![Добавление журнала изменений](image/21.png){#fig:0021 width=60%}

Залью релизную ветку в основную ветку:

![Замена ветки](image/23.png){#fig:0022 width=60%}

Отправляю данные на github:

![Отправка на гит](image/23.png){#fig:0023 width=60%}

Создаю релиз на github. Для этого использую утилиты работы с github gh (gh release create):

![Создание релиза](image/24.png){#fig:0024 width=60%}

Создаю ветку для новой функциональности:

![Создание ветки feature_branch](image/25.png){#fig:0025 width=60%}

Далее, продолжаю работу c git как обычно. Создаю релиз с версией 1.2.3:

![Создание релиза с версией 1.2.3](image/26.png){#fig:0026 width=60%}

Обновляю номер версии в файле package.json в 1.2.3:

![Обновление номера версии](image/27.png){#fig:0027 width=60%}

Создаю журнал изменений (standard-changelog):

![Создание нового журнала изменений](image/28.png){#fig:0028 width=60%}

Добавляю журнал изменений в индекс:

![Добавление журнала](image/29.png){#fig:0029 width=60%}

Залью релизную ветку в основную ветку:

![Замена ветки](image/30.png){#fig:0030 width=60%}

Отправляю данные на github:

![Отправка данных](image/31.png){#fig:0031 width=60%}

Создаю релиз на github с комментарием из журнала изменений:

![Cоздание релиза](image/32.png){#fig:0032 width=60%}

# Выводы

При Выполнение лабораторной работы я получила навыки правильной работы с репозиториями git.

# Список литературы{.unnumbered}

::: {#refs}
:::
