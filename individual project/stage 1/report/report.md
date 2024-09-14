---
## Front matter
title: "Отчёт по Индивидуальному проекту"
subtitle: "Этап 1. Установка Kali Linux"
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

Установить операционную систему на виртуальную машину.

# II. Выполнение задания

- Создать новую виртуальную машину, укажать называние и тип операционной системы — Linux, Debian.

![Окно «Называние машины и тип ОС»](img1/1.png)

- Укажать размер основной памяти виртуальной машины - 4096 МБ, и количество процессора - 2.

![Окно конфигурация оборудования](img1/2.png)

- Задавать размер диска — 25 ГБ.

![Окно конфигурация виртуального жесткого диска](img1/3.png)

- Добавить новый привод оптических дисков.

![Окно «Носители» виртуальной машины](img1/4.png)

- Мы настроим систему для работы по следующему рисунку:

![Выбрать вариант графической установки](img1/5.png)

![В разделе «Настройка сети» вводить имя хоста системы](img1/6.png)

![Вводить доменное имя](img1/7.png)

![Создать учетную запись пользователя, указав его полное имя и имя пользователя](img1/9.png)

![Создать пароль для учетной записи пользователя](img1/10.png)

![Выбрать способ разбиения жесткого диска](img1/11.png)

![Выбрать диск, который использовать для разбиения](img1/12.png)

![Выбрать схему разбиения](img1/13.png)

- Затем выбрать опцию "Finish partitioning and write changes to disk option", потом начинаю установку Kali

![Выбрать среду рабочего стола и инструменты](img1/14.png)

![Установить загрузчик GRUB на жесткий диск](img1/15.png)

![Выбрать устройство загрузчика, чтобы убедиться, что вновь установленная система является загрузочной](img1/16.png)

- Когда установка Kali завершится, появится сообщение «Установка завершена». Нажать «Продолжить», чтобы перезагрузить виртуальную машину.

![Интерфейс Rocky Linux](img1/17.png)

# IV. Вывод

После лабораторной работы я установил операционную систему Kali Linux на виртуальную машину.
