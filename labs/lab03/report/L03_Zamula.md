---
## Front matter
title: "Отчёт по лабораторной работе 3"
subtitle: "Дисциплина: операционная система"
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

Научиться оформлять отчёты с помощью легковесного языка разметки Markdown.

# Задание

- Сделайте отчёт по предыдущей лабораторной работе в формате Markdown.
- В качестве отчёта просьба предоставить отчёты в 3 форматах: pdf, docx и md (в архиве, поскольку он должен содержать скриншоты, Makefile и т.д.


# Выполнение лабораторной работы

1. Установка редакторов , таких как pandoc и texlive

![установка редакторов](https://github.com/egorzam21/study_2023-2024_os-intro/blob/master/labs/lab03/report/image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202024-02-25%2023-40-21.png?raw=true){#fig:001 width=70%}

2. Наглядно показваю как редактирую

![Редактирую мд файл](https://github.com/egorzam21/study_2023-2024_os-intro/blob/master/labs/lab03/report/image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202024-02-25%2023-41-15.png?raw=true){#fig:002 width=70%}

3. Показваю как отредактировал файл

![Отредактированный файл](https://github.com/egorzam21/study_2023-2024_os-intro/blob/master/labs/lab03/report/image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202024-02-25%2023-41-44.png?raw=true){#fig:003 width=70%}

4. Конвертирую файл в docx и pdf

![Конвертирую файлы](https://github.com/egorzam21/study_2023-2024_os-intro/blob/master/labs/lab03/report/image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202024-02-25%2023-42-58.png?raw=true){#fig:004 width=70%}

5. Наглядно показваю , что файл docx создан

![Демонстрирую файлы](https://github.com/egorzam21/study_2023-2024_os-intro/blob/master/labs/lab03/report/image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202024-02-25%2023-43-08.png?raw=true){#fig:005 width=70%}

6. Отредактированный файл по лабораторной работе №2 
![Лабораторная работа №2](https://github.com/egorzam21/study_2023-2024_os-intro/blob/master/labs/lab03/report/image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202024-02-25%2023-43-32.png?raw=true){#fig:006 width=70%}

# Выводы

Научился использовать язык разметки markdown.

# Список литературы{.unnumbered}

::: {#refs}
:::
