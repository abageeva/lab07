---
# Front matter
lang: ru-RU
title: 'Отчёт'
subtitle: 'по лабораторной работе 7'
author: 'Агеева Анастасия Борисовна'

# Formatting
toc-title: 'Содержание'
toc: true # Table of contents
toc_depth: 2
lof: true # List of figures
lot: true # List of tables
fontsize: 12pt
linestretch: 1.5
papersize: a4paper
documentclass: scrreprt
polyglossia-lang: russian
polyglossia-otherlangs: english
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase
indent: true
pdf-engine: lualatex
header-includes:
  - \linepenalty=10 # the penalty added to the badness of each line within a paragraph (no associated penalty node) Increasing the value makes tex try to have fewer lines in the paragraph.
  - \interlinepenalty=0 # value of the penalty (node) added after each line of a paragraph.
  - \hyphenpenalty=50 # the penalty for line breaking at an automatically inserted hyphen
  - \exhyphenpenalty=50 # the penalty for line breaking at an explicit hyphen
  - \binoppenalty=700 # the penalty for breaking a line at a binary operator
  - \relpenalty=500 # the penalty for breaking a line at a relation
  - \clubpenalty=150 # extra penalty for breaking after first line of a paragraph
  - \widowpenalty=150 # extra penalty for breaking before last line of a paragraph
  - \displaywidowpenalty=50 # extra penalty for breaking before last line before a display math
  - \brokenpenalty=100 # extra penalty for page breaking after a hyphenated line
  - \predisplaypenalty=10000 # penalty for breaking before a display
  - \postdisplaypenalty=0 # penalty for breaking after a display
  - \floatingpenalty = 20000 # penalty for splitting an insertion (can only be split footnote in standard LaTeX)
  - \raggedbottom # or \flushbottom
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Освоить на практике применение режима однократного гаммирования.

# Задание

Лабораторная работа подразумевает подобрать ключ, чтобы получить сообщение «С Новым Годом, друзья!». Требуется разработать приложение, позволяющее шифровать и дешифровать данные в режиме однократного гаммирования.

# Выполнение лабораторной работы

1. Разработаем приложение, позволяющее шифровать и
дешифровать данные в режиме однократного гаммирования. (рис.1).

   ![рис.1. Программа.](images/1.jpg){ #fig:001 width=60% }

2. Подоберём ключ, чтобы получить сообщение «С Новым Годом Вас!». После ключа текст становится неизменным. (рис.2).

   ![рис.2. Определение ключа.](images/2.jpg){ #fig:002 width=60% }

3. Контрольные вопросы
1) Поясните смысл однократного гаммирования.
Каждый символ попарно с символом ключа складываются по модулю.
2) Перечислите недостатки однократного гаммирования.
Ключ нельзя переиспользовать. Размер ключа должен быть такой же, как и размер текста.
3) Перечислите преимущества однократного гаммирования.
Основные преимущества однократного гаммирования – это симметричность и криптостойкость.
4) Почему длина открытого текста должна совпадать с длиной ключа?
Потому что каждый символ открытого текста должен складываться символом ключа попарно.
5) Какая операция используется в режиме однократного гаммирования, назовите её особенности?
В режиме однократного гаммирования используется сложение по модулю 2.
Её особенность состоит в том, что при сложении чисел с другим получается исходное.Например, 0+0 = 0, 0+1=1, 1+0=1, 1+1=0.
6) Как по открытому тексту и ключу получить шифротекст?
Нужно сложить попарно символы текста с ключом по модулю 2.
7) Как по открытому тексту и шифротексту получить ключ?
Нужно сложить попарно символы открытого текста с символами шифротекста по модулю 2.
8) В чем заключаются необходимые и достаточные условия абсолютной стойкости шифра?
Необходимые и достаточные условия абсолютной стойкости шифра:
а) полная случайность ключа;
б) равенство длин ключа и открытого текста;
в) использование ключа однкратно.

# Выводы

Я приобрела практические навыки применения режима однократного гаммирования.
