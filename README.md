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

***3) Как доказать строгое включение класса P в P/poly?***

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

***6) Можно ли заменить в теореме Кука КНФ-выполнимость на тождественную ложь?***

**Ответ:** Теорема 9.2

***7) Определение сложности в худшем случае для НМТ и ОМТ***

**Ответ:** Дается через общее определение лсожности в худшем, накладывается на определения сложностей НМТ, ОМТ. В нмт - минимум по всез отгадам по данному условию. ОМТ - аналогично МТ, тк к оракулу за такт обращаемся

***8) Привести пример Алгоритмически неразрешимых задач***

**Ответ:**

***9) Теорема о соотношении МТ и НАМ***

**Ответ:**

***10) Можно ли дать определение оракульной машины Тьюринга используя язык предикатов?***

**Ответ:** (можно сделать (что-то в направлении функцию представить как предикат, можно использовать кванторы, существует два состояния, обратится в любой момент времени, это неверно, но направление правильно))

***11) Теорема о соотношении НАМ и МТ***

**Ответ:**

***12) Как связана сложность МТ и количество команд в ней***

**Ответ:** Никак, так как сложность МТ это количество тактов ее работы, которое не связано с множеством команд.

***13) Пример сводимости по Тьюрингу***

**Ответ:**

***14) Почему PSPACE лежит в EXPTIME ?***

**Ответ:**

***15) Всегда ли в базисе {кон, диз, отриц} наименьшая сложность СФЭ для функции f - это функция, реализующаяся её минимальной ДНФ?***

**Ответ:** Нет, так как можно использовать КНФ. Зависит от количества 0 и 1 в таблице.

***16) Дать определение класса P/Poly при помощи исчисления предикатов? (Определить понятие P/Poly с использованием языка предикатов?)***

**Ответ:** 1) *Определение:* **P/poly** - множество предикатов таких, что набор функций, получаемые от этих предикатов, реализуется за полиномиальные схемы от n, где n - количество переменных в функции.

2) *Определение:* **P/poly** - множество предикатов вида P, таких, что функции f1, f2,..., fn,... реализуют СФЭ полиномиальной сложности по n. (Существует P - предикат, который определен на множестве всех двоичных последовательностей длины от 1 до бесконечности f1(x1)=P1, f2(x1,x2)=P2, ... fn(x1, ..., xn)=Pn,  Pn - это функция он n переменных.)

3) *Определение:* **P/poly** - A(x1,x2...): f1(x1),f2(x1,x2) и тд реализуются за P(n), где A-предикаты, P(n)-полином

4) *Определение (из введений Гордеева):* Класс булевых функций, для которых существуют схемы полиномиальной сложности обозначим через **P/poly**.


***17) Привести пример алгоритмически неразрешимой проблемы с доказательством.***

**Ответ:**

***18) Вопрос на исследование формулы***

**Ответ:**

***19) Теорема Ланднера***

**Ответ:**

***20) Мини вопрос: Может ли CoNP лежать в NP (да может, есть пересечение (класс P))***

**Ответ:**
