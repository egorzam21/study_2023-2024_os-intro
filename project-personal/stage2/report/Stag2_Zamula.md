---
## Front matter
title: "Индивидуальный проект"
subtitle: "Часть 2"
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

Изменить наш сайт (добавить фото, имя и два поста)

# Выполнение лабораторной работы

1. Добавили фото в папку admin и начинаем изменять файл _index.md

![Добавление фото](https://github.com/egorzam21/study_2023-2024_os-intro/blob/master/project-personal/stage2/report/image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202024-03-15%2012-11-45.png?raw=true){#fig:001 width=70%}

2. Изменеённый файл _index.md
![Готовый файл](https://github.com/egorzam21/study_2023-2024_os-intro/blob/master/project-personal/stage2/report/image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202024-03-15%2012-16-43.png?raw=true){#fig:002 width=70%}

3. Создаем два поста через терминал

![Добавоение постов](https://github.com/egorzam21/study_2023-2024_os-intro/blob/master/project-personal/stage2/report/image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202024-03-15%2012-18-45.png?raw=true){#fig:003 width=70%}

4. Проверяем , создались ли папки с постами (да, создались)

![Проверка](https://github.com/egorzam21/study_2023-2024_os-intro/blob/master/project-personal/stage2/report/image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202024-03-15%2012-19-21.png?raw=true){#fig:004 width=70%}

5. Пишем сам пост в файле _index.md

![Пишем пост](https://github.com/egorzam21/study_2023-2024_os-intro/blob/master/project-personal/stage2/report/image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202024-03-15%2012-25-57.png?raw=true){#fig:005 width=70%}

6. Прописываем команду hugo 

![Hugo](https://github.com/egorzam21/study_2023-2024_os-intro/blob/master/project-personal/stage2/report/image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202024-03-15%2012-27-17.png?raw=true){#fig:006 width=70%}

7. Отправиили файлы на сервер

![Отправка файлов](https://github.com/egorzam21/study_2023-2024_os-intro/blob/master/project-personal/stage2/report/image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202024-03-15%2012-29-20.png?raw=true){#fig:007 width=70%}


# Выводы

Изменили сайт под себя.

# Список литературы{.unnumbered}

::: {#refs}
:::
