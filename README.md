# МЛиТА экзамен (вопросы и ответы)

***1) Как доказать общезначимость формулы без кванторов?***

**Ответ:**
1) *Определение (из введений Гордеева):* Формула логики предикатов называется **логически общезначимой**, если она истинна в любой интерпретации.
(Простым языком: Логическая общезначимость формулы означает, что какую бы ни выбирали область интерпретации и какие бы соответствия не задавали, мы всегда будем получать истинные отношения или высказывания)

2) Построим таблицу, в которой A и B - предикаты, F - конечная данная формула. Предполагаем, что в какой-то интерпретации каждая из формул A и B - истинна или ложна. Если конечная формула F - истинна при любых входях подформулах, то F - общезначима.

***2) Как переформулировать задачу в оптимизационной форме в задачу в форме распознавания хелпанитет? (Можно ли переформировать задачу в форме оптимизации в форму распознавания, и значит ли это что NP трудная задача переформулируется в NP полную?) (Как переформулировать задачу из формы оптимизации в форму распознавания? Следует ли из этого, что np-hard в форме оптимизации всегда можно переформулировать в npc в форме распознавания?)***

(Я привёл пример задачи комивояжера в двух формах (он принял), а про второй вопрос он сказал, что я ответил не на тот)
**Ответ:** На счёт оптимизации
можно поставить какие- нибудь пороги
типа если у тебя оптимизация перехходит порог - то есть, если не переходит, то нет
грубо говоря, нужно проверить 
есть ли а графе ГЦ
А у тебя задача по оптимизации: цикл опр длины
порогом будет - число вершин
попробуй так
Если непонятно - могу другими словами попытаться
А нельзя просто поменять вопрос «какой?» на «существует ли?»

***3) Как из нестрогого включения п в п поли получить строгое? (строгое включение P в P/Poly)***

(тема алгоритмически неразрешим задач)

**Ответ:** сказать о существовании алгоритмически неразрешимых задач.
В вопросе про строгое включение P в P/Poly он в основном говорит об алгоритмически неразрешимых задачах и их отношению к P/ Poly
Он хотел бы услышать про функцию натурального аргумента... (см. Стр 80 старого конспекта)
Про общезначимость вариант навесить кванторы всеобщности - неправильно. 
Про определение ОМТ через предикаты, он отметил минимальную логику в том, чтобы представить функцию предикатом и использование кванторов всеобщеости и существования
Правильных ответов он не дал специально, по его словам

P/poly-мн-во предикатов таких, что набор функций, получаемые от этих предикатов, реализуются за полиномиальные схемы от n, где n-количество переменных в функции
P/poly - A(x1,x2...): f1(x1),f2(x1,x2) и тд реализуются за P(n), где A-предикаты
видимо как-то так
P(n)-полином

***4) V - Любой
Е - Существует
VxA(x) -> (Ex не C(x) -> Ex не (A(x) -> C(x)))
Исследовать на выполнимость и тд***

**Ответ:** не общезначима
UPD: кирпич сломался, формула общезначима и это доказано на семинаре
Определение сложности в худшем случае для НМТ и ОМТ

***5) VxEy A общезначима
ExVy A не выполнима
Сущестаует ли формула А для которой вот это верно?***

**Ответ:**

***6) Можно ли заменить в теореме Кука КНФ-выполнимость на тождественную ложь?
Проверьте ответ пожалуйста. Если NP=Co-NP, то можно.
Норм логика?***

**Ответ:** Теорема 9.2.  Если NP=Co-NP, то можно, тк первый аункт теоремы Кука - доказать, что задача принадлежит NP. Данная задача(с тождественной ложью) принадлежит coNp, отсюда и ответ, полученный выше.

***7) Можно ли дать определение ОМТ с помощью языка исчисления предикат ?***
**всё скаанное ниже - непроверенные догадки. автор будет отвечать в случае чего так, но ответственности не несёт**

**Ответ:** Да, можно.  По сути, мы подаём на НМТ некий вход, условия, далее ОМТ что-то делает и даёт на выходе ответ. Рассуждения далее только для задач в форме распознования, где возможен бинарный ответ.
Пусть есть двумесный(? может ещё что-то засунуть в условия, типа язык, пустой символ и тд, то, что в фигурных скобках при определении МТ) предикат. Мы подаём на вход оракульную функцию(функция может быть термом), наш вход(и по желанию - алфавит и тд и тп из прошлых скобок, пока не решила надо или нет). Далее предикат выдаёт 1, если ответ "да", и 0, если ответ "нет"

***8) Теорема Ланднера***
**всё скаанное ниже - непроверенные догадки. автор будет отвечать в случае чего так, но ответственности не несёт**

**Ответ:** Саму теорему можно найти в старом конспекте, ctrl+F. Думаю, что её смысл - то, что класс NP неоднороден. Т.е. если P не равно np, то разбить np можно минимум на 3 класса: np-полные(npc), полиномиальные(p) и вот этот класс по середине, существование которого доказывается в этой теореме. Т.е. если есть задача из нп, и она не в нпс и не в п, то это не всегда значит, что просто не смогли доказать один из 2 фактов, возможно, она в 3 классе.

***9) всегда ли в базисе кон диз отр наим сложность сфэ для функции - схаема реализации её мин днф
дайти опр классу п поле с имп языка исчисления предикатов***

**Ответ:** Точно нет. доказательство - примером. функция: НЕ(xy). сложность - 2
её мин днф: НЕ(х)\/НЕ(у), сложность - 3


***10) Определение сложности в худшем случае для НМТ и ОМТ***

(Дается через общее определение лсожности в худшем, накладывается на определения сложностей НМТ, ОМТ. В нмт - минимум по всез отгадам по данному условию. ОМТ - аналогично МТ, тк к оракулу за такт обращаемся)

**Ответ:** и новый, и старый конспекты.

***11) Вопрос на исследование формулы***

**Ответ:** 

***12) Можно ли в теореме Кука заменить КНФ-выполнимость на тождественный ноль
Привести пример Алгоритмически неразрешимых задач
Потомкам. Знайте определения того, что говорите и лучше сразу их выдавать по мере рассказа***

**Ответ:** 1. было ранее, п6
2.

***13) Теорема о соотношении МТ и НАМ
Как доказать общезначимость  ф исчисления предикатов если в ней нет кванторов
Дать определение класса P/poly при помощи исчисления предикатов
Мини вопрос: Может ли CoNP лежать в NP (да может, есть пересечение (класс P))***

**Ответ:**

***14) Можно ли дать определение оракульной машины Тьюринга используя язык предикатов?***

**Ответ:** (можно сделать (что-то в направлении функцию представить как предикат, можно использовать кванторы, существует два состояния, обратится в любой момент времени, это неверно, но направление правильно))

***15) Теорема о соотношении НАМ и МТ***

**Ответ:**

***16) Как связана сложность МТ и количество команд в ней***

**Ответ:**

***17) Пример сводимости по Тьюрингу***

**Ответ:**

***18) Почему PSPACE лежит в EXPTIME ?***

**Ответ:**

***19) Всегда ли в базисе {кон, диз, отриц} наименьшая сложность СФЭ для функции f - это функция, реализующаяся её минимальной ДНФ?***

**Ответ:** Нет, так как можно использовать КНФ. Зависит от количества 0 и 1 в таблице.

***20) Дать определение класса P/Poly при помощи исчисления предикатов? (Определить понятие P/Poly с использованием языка предикатов?)***

**Ответ:** 1) *Определение:* **P/poly** - множество предикатов таких, что набор функций, получаемые от этих предикатов, реализуется за полиномиальные схемы от n, где n - количество переменных в функции.

2) *Определение:* **P/poly** - множество предикатов вида P, таких, что функции f1, f2,..., fn,... реализуют СФЭ полиномиальной сложности по n. (Существует P - предикат, который определен на множестве всех двоичных последовательностей длины от 1 до бесконечности f1(x1)=P1, f2(x1,x2)=P2, ... fn(x1, ..., xn)=Pn,  Pn - это функция он n переменных.)

3) *Определение:* **P/poly** - A(x1,x2...): f1(x1),f2(x1,x2) и тд реализуются за P(n), где A-предикаты, P(n)-полином

4) *Определение (из введений Гордеева):* Класс булевых функций, для которых существуют схемы полиномиальной сложности обозначим через **P/poly**.

из лекции: 

![пполи через предикаты](https://github.com/Medvate/mlita_exam/blob/45/images/%D0%BF%D0%BF%D0%BE%D0%BB%D0%B8%20%D1%87%D0%B5%D1%80%D0%B5%D0%B7%20%D0%BF%D1%80%D0%B5%D0%B4%D0%B8%D0%BA%D0%B0%D1%82%D1%8B.png)

***21) Привести пример алгоритмически неразрешимой проблемы с доказательством.***

**Ответ:** 


***22) Дать определения P поля с использованием исчисления предиката***

**Ответ:** В дискорде Леша прислал из лекции


***23) был про Кука и КНФ-выполнимость/тождественную ложь***

**Ответ:** см ранее

