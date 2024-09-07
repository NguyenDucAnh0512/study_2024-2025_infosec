---
## Front matter
title: "Отчёт по лабораторной работе №1"
subtitle: "Установка и конфигурация операционной системы на виртуальную машину"
author: "Нгуен Дык Ань"

## Generic otions
lang: ru-RU
toc-title: "Содержание"

## Bibliography
bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl

## Pdf output format
toc: true # Table of contents
toc-depth: 2
lof: false # List of figures
lot: false # List of tables
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
  - \usepackage[T2B]{fontenc}
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# I.Цель работы

Получить навыки установок операционной системы на виртуальную машину и настроить минимально необходимых для дальнейшей работы сервисов.

# II. Задание

1. Установить операционную систему Linux на виртуальную машину VirtualBox

2. Настроить систему для работы сервисов

3. Познакомиться с операционной системой командой "dmesg"

# III. Выполнение задания

## 1. Установить операционную систему Linux (дистрибутив Rocky) на виртуальную машину VirtualBox

- Создать новую виртуальную машину, укажать называние и тип операционной системы — Linux, RedHat.

![Окно «Называние машины и тип ОС»](https://drive.google.com/uc?id=1h1jlRdL19VZGcLUiDxCezIA1KuDIzQRI)

- Укажать размер основной памяти виртуальной машины - 4096 МБ, и количество процессора - 2.

![Окно конфигурация оборудования](https://drive.google.com/uc?id=1US4h11eIQ3cxZeUd38BLAf_jK1bdYCPL)

- Задавать размер диска — 60 ГБ.

![Окно конфигурация виртуального жесткого диска](https://drive.google.com/uc?id=1vee94XxeN5NHtXf_dueZddLxM8hYhI_j)

- Добавить новый привод оптических дисков.

![Окно «Носители» виртуальной машины](https://drive.google.com/uc?id=1mwu0-HvMZo3HXp-WFkhDxqlo12KQLpKB)

## 2. Настроить систему для работы сервисов

- Мы настроим систему для работы сервисов по следующему рисунку:

![Окно настройки установки: выбор программ](https://drive.google.com/uc?id=19koVVDR9E6kAwAmgo5lx2xoM3wpU4EFo)

![Отключить KDUMP](https://drive.google.com/uc?id=14PEqZRdfZTLxCD7_l8-n9ePIhKePv5re)

![Включить сетевое соединение и в качестве имени узла укажать danguen.localdomain](https://drive.google.com/uc?id=1JMw1-mtim3WrwerHyGZaK9qCtoPxrcV6)

![Установить пароль для root](https://drive.google.com/uc?id=1WQOZIDbF3J0gEKvuOLjPTePj0QYn6apf)

![Установить пароль для пользователя с правами администратора](https://drive.google.com/uc?id=164ui4Rh7OfjA4VKZW61FTLpz0zIFX8Gj)

- После этого, мы перезапустим виртуальную машину.

![Интерфейс Rocky Linux](https://drive.google.com/uc?id=1cEu-k9euuiyLvEz_8OtiyMso6kxk5goe)

- Затем подключить образ диска дополнений гостевой ОС и корректно перезагрузить виртуальную машину.

## 3. Познакомиться с операционной системой командой "dmesg"

- **dmesg** - команда, используемая в UNIX‐подобных операционных системах для вывода буфера сообщений ядра в стандартный поток вывода (по умолчанию на экран).

- Можно использовать поиск с помощью **grep** для получения следующей информаций:

![Версия ядра Linux](https://drive.google.com/uc?id=1Op1gXBk8dXv09aYEJbJt2jyWRFYQ4we3)

![Частота процессора](https://drive.google.com/uc?id=12i3X0tDlIvkmUATB-OzulGxbBpnDXv2z)

![Модель процессора](https://drive.google.com/uc?id=1rnZgldQajcS-HBMviKT4nUYJNH-haxK5)

![Объем доступной оперативной памяти](https://drive.google.com/uc?id=1b9xpWNR1luYNJRSPDPYb-EHv5WNIZvGT)

![Тип обнаруженного гипервизора](https://drive.google.com/uc?id=1UblkoNTL40cwQ7wDmhxqagD_b0Qdhzdm)

![Тип файловой системы корневого раздела](https://drive.google.com/uc?id=16X29qW9bAuDKizNXAzefepbSwJjtXxir)

![Последовательность монтирования файловых систем](https://drive.google.com/uc?id=1KyrQE5dxWP4vMjfu3N-vaAy7FwaJd39F)

# IV. Вывод

После лаборатоной работы я получил навыки установок и настройки операционной системы на виртуальную машину для дальнейшей работы сервисов.
