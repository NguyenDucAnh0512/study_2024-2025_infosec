---
## Front matter
title: "Отчёт по Индивидуальному проекту"
subtitle: "Этап 2. Установка DVWA"
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
---

# I.Цель работы

Установить и настроить DVWA в систему к Kali Linux.

# III. Выполнение работы

- В консоли перейти в директорию /var/www/html (это директория по умочанью вев-сервера) и клонировать DVWA git-директория.

![](img/1.png)

![](img/2.png)

- Настроить доступ директории DVWA, что DVWA полностью доступным для чтения, записи и исполнения для всех.

![](img/3.png)

- Скопировать файл конфигурации /var/www/html/DVWA/config/config.inc.php.dist на config.inc.php.

![](img/5.png)

- Поменять имя и пароль пользователя в файле конфигурации config.inc.php.

![](img/6.png)

- Запустить базу данных в консоли и проверять статус базы данных.

![](img/7.png)

![](img/8.png)

- После того, войти в базу данных.

![](img/9.png)

- Создать базу данных с именем dvwa.

![](img/10.png)

- Cоздать пользователя и пароль (должны совпадать с именем пользователя и паролем в файле конфигурации).

![](img/11.png)

- Предоставить все привилегии этому пользователю.

![](img/12.png)

- Запустить и проверять статус веб-сервер Apache2.

![](img/13.png)

![](img/14.png)

- Поменять файл конфигурации /etc/php/8.2/apache2/php.ini как следующий.

![](img/15.png)

- Перезагрузить веб-сервер Apache2.

![](img/16.png)

- В браузере войти в ссыльку "127.0.0.1/DVWA" и вводить username и пароль, DVWA готов для использования.

![](img/17.png)

# IV. Вывод

После этой лабораторной работы я установил и настроил DVWA в систему к Kali Linux.

