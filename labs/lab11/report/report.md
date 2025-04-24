---
## Front matter
title: "Отчёт по лабораторной работе 11"
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

Получить практические навыки работы с редактором Emacs.

# Задание

1. Выполнить основные команды emacs

# Выполнение лабораторной работы

Для данной работы, мне надо была установить Emacs:

![установка Emacs](image/1.png){#fig:001 width=70%}

Выполнив Emacs в командной строке, я открыла текстовый редактор:

![Emacs](image/2.png){#fig:002 width=70%}

С помощью комбинации Ctrl-x Ctrl-f, создала файл lab07.sh:

![Созданный файл](image/3.png){#fig:003 width=70%}

Я написала некоторый текст в этом же файле (lab07.sh). После этого сохранила файл с помощью комбинации Ctrl-x Ctrl-s:

![текст в lab07.sh](image/4.png){#fig:004 width=70%}

Одной командой вырезала целую строку (С-k):

![Вырезание строки](image/5.png){#fig:005 width=70%}

С помощью C-y вставила эту строку в конец файла:

![Перемешение строку в конец файла](image/6.png){#fig:006 width=70%}

Выделила область текста (C-space):

![Выделенный текст](image/7.png){#fig:007 width=70%}

Скопировала область в буфер обмена (M-w) и вставила ее в конец файла:

![копирование и вставка](image/8.png){#fig:008 width=70%}

Выделила эту же область и на этот раз вырезала её (C-w):

![ВЫрезанная область](image/9.png){#fig:009 width=70%}

С помощью C-/ отменила последнее действие:

![отмена действие](image/10.png){#fig:0010 width=70%}

С помощью C-a переместила курсор в начало строки:

![Перемещение курсор в начало строки](image/11.png){#fig:0011 width=70%}

С помощью C-e переместила курсор в конец строки:

![Перемещение курсор в конец строки](image/12.png){#fig:0012 width=70%}

Переместила курсор в начало и конец буфера с помощью M-< и M-> соответственно:

![Перемешение курсор в буфере](image/13.png){#fig:0013 width=70%}

Выводила список активных буферов на экран с помощью C-x C-b:

![Активные буферы](image/14.png){#fig:0014 width=70%}

С помощью C-x o переместилась во вновь открытое окно со списком открытых буферов и переключилась на другой буфер:

![список открытых буферов](image/15.png){#fig:0015 width=70%}

С помощью C-x 0 закрыла окно со списком открытых буферов:

![Закрытие окно](image/16.png){#fig:0016 width=70%}

Без вывода списка буферов, я переключилась между буферами

![Переключение между буферами](image/17.png){#fig:0017 width=70%}

![Новый буфер](image/18.png){#fig:0018 width=70%}

Поделила фрейм на 4 части. Сначала я разделила фрейм на два окна по вертикали (C-x 3), а затем каждое из этих окон на две части по горизонтали (C-x 2):

![Фрейм разделённый на 4 окна](image/19.png){#fig:0019 width=70%}

В каждом из четырёх созданных окон открыла новый буфер: 

![новый буфер](image/20.png){#fig:0020 width=70%}

Переключилась в режим поиска (C-s) и искала Indent:

![Режим поиска](image/21.png){#fig:0021 width=70%}

Переключалась между результатами поиска, нажимая C-s и вышла из режима поиска, нажав C-g:

![Переключение между результатами](image/22.png){#fig:0022 width=70%}

Перешла в режим поиска и замены (M-%), искала слово World, нажмала Enter, и заменила на Planet:

![Режим поиска](image/23.png){#fig:0023 width=70%}

Нажав M-s o, я использовала другой режим поиска. Он отличается от предыдущего тем, что выводит результаты поиска в новом окне:

![другой режим поиска](image/24.png){#fig:0024 width=70%}

![Результаты поиска](image/25.png){#fig:0025 width=70%}


# Выводы

При выполнение данной работы я получила практические навыки работы с Emacs.

# Ответы на котрольные вопросы

1. Emacs — один из наиболее мощных и широко распространённых редакторов, используемых в мире UNIX. Написан на языке высокого уровня Lisp.

2. Большое разнообразие сложных комбинаций клавиш, которые необходимы для редактирования файла и в принципе для работа с Emacs.

3. Буфер - это объект в виде текста. Окно - это область, в которой отображен буфер.

4. Да, можно.

5. Emacs использует буферы с именами, начинающимися с пробела, для внутренних целей. Отчасти он обращается с буферами с такими именами особенным образом — например, по умолчанию в них не записывается информация для отмены изменений.

6. Ctrl + c, а потом | и Ctrl + c Ctrl + |

7. С помощью команды Ctrl + x 3 (по вертикали) и Ctrl + x 2 (по горизонтали).

8. Настройки emacs хранятся в файле . emacs, который хранится в домашней дирректории пользователя. Кроме этого файла есть ещё папка . emacs.

9. Выполняет функцию стереть, думаю можно переназначить.

10. Для меня удобнее был редактор Emacs, так как у него есть командая оболочка. А vi открывается в терминале, и выглядит своеобразно.

# Список литературы{.unnumbered}

::: {#refs}
:::
