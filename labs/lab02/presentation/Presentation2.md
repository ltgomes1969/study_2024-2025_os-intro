---
## Front matter
lang: ru-RU
title: Отчёт по лабораторной работе 2
subtitle: Операционные Системы
author:
  - .Гомес Лопес Теофания
institute:
  - Российский университет дружбы народов, Москва, Россия
date: 03 марта 2025

## i18n babel
babel-lang: russian
babel-otherlangs: english

## Formatting pdf
toc: false
toc-title: Содержание
slide_level: 2
aspectratio: 169
section-titles: true
theme: metropolis
header-includes:
 - \metroset{progressbar=frametitle,sectionpage=progressbar,numbering=fraction}
---


# Цель работы

Изучение идеалогии, применение средств контроля версий и освоение умения по работе с git.

# Задание

1.Создать базовую конфигурацию для работы с git.
2.Создать ключ SSH.
3.Создать ключ PGP.
4.Настроить подписи git.
5.Зарегистрироваться на Github.
6.Создать локальный каталог для выполнения заданий по предмету.



# Выполнение лабораторной работы

## Создание базовой конфигурации для работы с git.

 Установление git и gh:

![Установление git](./image/1.png){#fig:001 width=70%}

![Установление gh](./image/2.png){#fig:002 width=70%}

В качестве имя и email владельца репозитории задаю свои имя и email и настраиваю utf-8:

![Имя и email владельца](./image/3.png){#fig:003 width=70%}

Задаю имя начальной ветки и паррамеры autocrlf и safecrlf:

![Имя начальной ветки и паррамеры](./image/4.png){#fig:004 width=70%}

## Создание ключ SSH:

Создаю ключи ssh по алгоритму rsa с размером 4096 бит:

![Создание ключ ssh](./image/5.png){#fig:005 width=70%}

## Создание ключ gpg

Генерирую ключ gpg --full-generate-key:

![Создание ключ gpg](./image/6.png){#fig:006 width=70%}

Из предложенных опций выбираю тип RSA and RSA; размер 4096; срок действия 0: 

![Настройки ключ gpg](./image/7.png){#fig:007 width=70%}

## Создание ключ gpg

GPG запросил личную информацию, которая сохранится в ключе Имя и адрес электронной почты:

![личная информация](./image/8.png){#fig:008 width=70%}

У меня уже есть аккаунт на github, поэтому я вхожу в систему:

![аккаунт на git](./image/9.png){#fig:009 width=70%}

Вывожу список ключей:

![список ключей](./image/10.png){#fig:010 width=70%}

## Создание ключ gpg

Установливаю xclip: 

![Установление xclip](./image/11.png){#fig:011 width=70%}

Cкопирую сгенерированный gpg ключ в буфер обмена:

![Копирование ключ gpg](./image/12.png){#fig:012 width=70%}

Далее перехожу в настройки GitHub, нажимаю на кнопку New GPG key и вставляю полученный ключ:

![Добавлен ключ gpg](./image/13.png){#fig:013 width=70%}

## Создание ключ gpg

Используя введёный email, указиваю Git применять его при подписи коммитов:

![указиваю Git](./image/14.png){#fig:014 width=70%}

Начинаю авторизацию в gh используя gh auth login:

![авторизацию в gh](./image/15.png){#fig:015 width=70%}

## Создание ключ gpg

Завершаю авторизацию на броузер:

![Авторизоваться через броузер](./image/16.png){#fig:016 width=70%}

![Завершена авторизация](./image/17.png){#fig:017 width=70%}

## Создание локального каталога для выполнения заданий.

Создаю каталог "mkdir -p ~/work/study/2022-2023/"Операционные системы":

![Создание каталог](./image/18.png){#fig:018 width=70%}

Перехожу в созданный каталог:

![Создание каталог](./image/19.png){#fig:019 width=70%}

Удаляю лишные файлы:

![Удаление файла](./image/20.png){#fig:020 width=70%}

## Создание локального каталога для выполнения заданий.

Создаю еще необходимые каталоги:

![Создани необходимых каталогов](./image/21.png){#fig:021 width=70%}

Отправляю Файлы на сервер:

![Отправление файлы на сервер](./image/22.png){#fig:022 width=70%}

# Выводы

При выполнении лабораторной работы я изучила идеалогию, применение средств контроля версий и освоеила умение по работе с git.
