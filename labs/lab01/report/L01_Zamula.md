---
## Front matter
title: "Отчёт по лабораторной работе №1"
subtitle: "дисциплина: Операционные системы"
author: "Замула Егор Сергеевич"

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

Целью данной работы является приобретение практических навыков установки операционной системы на виртуальную машину, настройки минимально необходимых для дальнейшей работы сервисов.

# Выполнение лабораторной работы

1. Скачал с официального сайта VirtualBox(рис. [-@fig:001])

![Официальный сайт](https://github.com/egorzam21/study_2023-2024_os-intro/blob/master/labs/lab01/report/image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%202024-02-18%20151956.png?raw=true){#fig:001 width=70%}

2. Скачал с офицального сайта дистрибутив fedora(рис. [-@fig:002])

![Официальный сайт fedora](https://github.com/egorzam21/study_2023-2024_os-intro/blob/master/labs/lab01/report/image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%202024-02-18%20152302.png?raw=true){#fig:002 width=70%}

3. Настроил виртуальную машину(рис. [-@fig:003])

![Настройки моей виртуальной машины](https://github.com/egorzam21/study_2023-2024_os-intro/blob/master/labs/lab01/report/image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%202024-02-18%20184958.png?raw=true){#fig:003 width=70%}

4. Начал процесс установки дистрибутива fedora на виртуальную машину(рис. [-@fig:004])

![Начало процесса установки](https://github.com/egorzam21/study_2023-2024_os-intro/blob/master/labs/lab01/report/image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%202024-02-25%20144819.png?raw=true){#fig:004 width=70%}

5. Выбираю язык Русский(Россия)(рис. [-@fig:005])

![Выбор языка](https://github.com/egorzam21/study_2023-2024_os-intro/blob/master/labs/lab01/report/image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%202024-02-25%20144909.png?raw=true){#fig:005 width=70%}

6. Закончил установку и перезапускаю виртуальную машину, чтобы дистрибутив начал работать(рис. [-@fig:006])

![Перезагрузка](https://github.com/egorzam21/study_2023-2024_os-intro/blob/master/labs/lab01/report/image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%202024-02-25%20145037.png?raw=true){#fig:006 width=70%}

7. Удаляю диск с дистрибутивом, чтобы не пришлось еще раз устанавливать его (рис. [-@fig:007])

![Удаление диска](https://github.com/egorzam21/study_2023-2024_os-intro/blob/master/labs/lab01/report/image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%202024-02-18%20190915.png?raw=true){#fig:007 width=70%}

8. Начал настройку ОС(рис. [-@fig:008])

![Настройка ОС](https://github.com/egorzam21/study_2023-2024_os-intro/blob/master/labs/lab01/report/image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%202024-02-25%20145302.png?raw=true){#fig:008 width=70%}

9. Создаю имя согласно регламенту курса(рис. [-@fig:009])

![Создание профиля](https://github.com/egorzam21/study_2023-2024_os-intro/blob/master/labs/lab01/report/image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%202024-02-25%20145402.png?raw=true){#fig:009 width=70%}

10. Устанавливаю пароль (рис. [-@fig:010])

![Установка пароля](https://github.com/egorzam21/study_2023-2024_os-intro/blob/master/labs/lab01/report/image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%202024-02-25%20145449.png?raw=true){#fig:010 width=70%}

11. Проверка работы терминала и удостоверился, что профиль создан(рис. [-@fig:011])

![Проверка профиля](https://github.com/egorzam21/study_2023-2024_os-intro/blob/master/labs/lab01/report/image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%202024-02-25%20145527.png?raw=true){#fig:011 width=70%}

# Выводы

Приобрел парктические наавыки установки виртуальной машины и ОС на нее, а также настройки ее.

# Список литературы{.unnumbered}

::: {#refs}
:::
