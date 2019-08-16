# Словарь-индекс понятий со ссылками

Внимание! Ссылки на видео по каждой теме помещены в соответствующие репозитории.

Оглавление:
- [Базовые понятия](https://github.com/HowProgrammingWorks/Dictionary#Базовые-понятия)
- [Основные понятия](https://github.com/HowProgrammingWorks/Dictionary#Основные-понятия)
- [Вспомогательные материалы](https://github.com/HowProgrammingWorks/Dictionary#Вспомогательные-материалы)
- [Структуры данных](https://github.com/HowProgrammingWorks/Dictionary#Структуры-данных)
- [Расширенные понятия](https://github.com/HowProgrammingWorks/Dictionary#Расширенные-понятия)
- [Примеры кода и комплексного использования технологий](https://github.com/HowProgrammingWorks/Dictionary#Примеры-кода-и-комплексного-использования-технологий)
- [Параллельное программирование](https://github.com/HowProgrammingWorks/Dictionary#Параллельное-программирование)
- [Асинхронное программирование](https://github.com/HowProgrammingWorks/Dictionary#Асинхронное-программирование)
- [Парадигмы программирования](https://github.com/HowProgrammingWorks/Dictionary#Парадигмы-программирования)

## Базовые понятия

- [Абстракция / Abstraction](https://github.com/HowProgrammingWorks/Reusable)
это обобщение, отвлеченное от конкретики с выделением существенных и отсечением
несущественных свойств и связей. Абстрагирование - построение абстракций или
моделей, повышает повторное использование алгоритмов и структур данных.
  - Абстракция - обобщенное решение задачи (в отличие от конкретного решения),
  подходящее для широкого круга задач;
  - Абстракция - модель реального объекта (множества объектов), обобщение
  множества, приближение к реальности, достаточное для решения задачи;
  - Абстракция - множество свойств и связей объекта, относящееся к определенному
  его аспекту, необходимому для решения задачи;
  - [Слои абстракций / Abstraction Layer](https://github.com/HowProgrammingWorks/AbstractionLayers)
- Парадигма программирования / Programming Paradigm
  - Парадигма задает набор идей и понятий, допущений и ограничений, концепций,
  принципов, постулатов, приемов и техники программирования для решения задач
  на ЭВМ;
  - Парадигма предлагает модель резения задач, определенный стиль, шаблоны
  (примеры хороших и плохих решений) применяемых для написания программного кода;
- Синтаксис / Syntax - правила построения программного кода из символов, но не
затрагивающие смысловую (семантическую) нагрузку кода. Синтаксис определяет
только формальную структуру кода.
- Значение / Value - величина, записанная в определенное место памяти в
определенном формате и представляющая данные, которым может манипулировать
программа;
- Тип / Type - множество знанчений и операции, которые могут быть произведены над
этими значениями. Например, в JavaScript тип `Boolean` предполагает два значения
`true` и `false` и логические операции над ними, тип  `Null` предполагает одно
значение `null`, а тип `Number` множество рациональных чисел с дополнительными
ограничениями на минимальное и максимальное значение, а так же ограничения на
точность и математические операции `+ - * ** / % ++ -- > < >= <= & | ~ ^ << >>`.
  - [Типы данных / Data Types](https://github.com/HowProgrammingWorks/DataTypes)
  - `[5, 'Kiev', true, { city: 'Beijing' }, a => ++a ].map(x => typeof x);`
- Литерал / Literal - запись значения в коде программы. Напромер: литералы чисел,
логических значений, null и undefined, строк, массивов, объектов, функций.
Литералы могут иметь различный синтаксис, от очень простого, для записи чисел,
до сложных синтаксических конструкций, для записи объектов.
- Скаляр / Scalar / Primitive / Atomic value - значение примитивного типа данных.
Скаляр копируется при присвоении и передается в функцию по значению.
- Ссылка / Reference указывает на значение ссылочного типа, т.е. не скалярное
значение, для JavaScript это подтипы `Object, Function, Array`.
  - [ссылочные типы](https://github.com/HowProgrammingWorks/DataTypes)
  - [примеры кода по массивам и объектам](https://github.com/HowProgrammingWorks/DataStructures)
- Идентификатор / Identifier - имена переменных, констант, функций, методов,
аргументов, классов, как внутренние, так и импортированные из других модулей и
глобальные.
- [Переменная / Variable](https://github.com/HowProgrammingWorks/DataTypes) -
именованная область памяти (идентификатор), имеющая тип данных, адрес и
значение. Мы можем менять значение переменной в отличие от константы (а для
некоторых языков и тип): `let cityName = 'Beijing';`
- Присвоение / Assignment - связывания значения и идентификатора (например
переменной). Операция присвоения во многих языках возвращает присваиваемое
значение (имеет поведение выражения).
- [Константа / Constant](https://github.com/HowProgrammingWorks/DataTypes) -
идентификатор, с которым связано неизменяемое значение и тип:
`const WATCH_TIMEOUT = 5000;`
- [Структурные типы / Composed types](https://github.com/HowProgrammingWorks/DataTypes) -
композитные типы или структуры состоят из нескольких скалярных значений,
объедиенных в одно таким образом, чтоб над этим объединенным значением можно
выполнять набор операций, например: объект, массив, множество, кортеж.
- [Перечислимые типы / Enumerated types](https://github.com/HowProgrammingWorks/Enum)
- Флаг / Flag - Логическое значение, определяющее состояние чего-либо, например,
признак закрытия соединения, признак завершения поиска по структуре данных и т.д.
Например: `let flagName = false;` Иногда флагами могут называть не логические, а
перечислемые типы.
- Алгоритм / Algorithm - это формальное описанние порядка вычислений для
определенного класса задач за конечное время (способность завершаться для любого
множества входных данных).
- Программа / Programm - программный код и данные, объединенные в одно целое для
вычисления и управления ЭВМ.
- Инструкция / Instruction - один шаг алгоритма вычислений, например инструкция
процессора исполняется CPU.
- Оператор / Statement - наименьшая синтаксическая часть языка программирования,
исполняемая интерпретатором, средой или компилируемая в машинный код.
- Команда / Command - атомарная задача для командного процессора.
- Выражение / Expression - синтаксическая конструкция языка прогаммирования
предназначенная для выполнения вычислений. Выражение состоит из идентификаторов,
значений, операторов и вызова функций. Пример: `(len - 1) * f(x, INTERVAL)`
- Блок кода / Block - логически связанная группа инструкций или операторов.
Блоки создают область видимости. Блоки могут быть вложенными. Примеры: `{}`,
`(+ a b)`, `begin end`, отступы в Python.
- Процедура или подпрограмма / Procedure or Subroutine - логически связанная
группа инструкций или операторов, имеющая имя. Процедура способствует повторному
использованию кода и может быть вызвана из разных частей программы, много раз
и с разными аргументами. Процедура не возвращает значений, в отличие от функций,
но может модифицировать свои аргументы. Во многих языках процедура описывается
при помощи синтаксиса функций (например, типа void).
- Функция / Function - абстракция преобразования значений. Функция однозначно
отображает одно множество значений в другое множество значений. Функция может
быть задана блоком операторов или выражением. Функция имеет набор аргументов.
Функция может быть вызвана по имени или через указатель. Функция способствует
повторному использованию кода и может быть вызвана из разных частей программы,
много раз и с разными аргументами.
- Сигнатура функции / Function signature - имя (идентификатор), количество
аргументов и их типы (а иногда и имена аргументов), тип результата.
- [Метод / Method](https://github.com/HowProgrammingWorks/Function)
  - процедура, связанная с объектным контекстом или программным интерфейсом;
  - `{ a: 10, b: 10, sum() { return this.a + this.b; } }`
- [Цикл / Loop](https://github.com/HowProgrammingWorks/Iteration)
  - многократное исполнение блока операторов
- [Условие / Conditional statements](https://github.com/HowProgrammingWorks/Conditional)
  - синтаксическая конструкция, позволяющая выполнить разные действия или
  возвращающая разные значения (тернарный оператор) в зависимости от логического
  выражения (возвращающего true или false)
- [Рекурсия / Recursion](https://github.com/HowProgrammingWorks/Recursion) -
задание алгоритма вычисления функции через вызов ее самой (прямой или непрямой)
или определение функции, через нее саму.
  - Косвенная (непрямая) рекурсия - когда функция определена или вызывает себя
  не напрямую, а через другую или цепочку функций;
  - Хвостовая - частный случай, когда рекурсивный вызов является последней
  операцией перед возвратом значения, что всегда может быть преобразовано
  в цикл, даже автоматическим способом. Не хвостовая тоже может быть
  преобразована в цикл и оптимизирована, но более сложным способом, обычно
  вручную.
- [Строка / String](https://github.com/HowProgrammingWorks/String)
  - последовательность символов (в большинстве языков к каждому символу можно
  обратиться через синтаксис доступа к элементам массива, например, квадратные
  скобки)
- [Коллекция / Collection](https://github.com/HowProgrammingWorks/Collections) -
структура данных, служащая для хранения набора значений и предоставляющая доступ
к ним по индексам или ключам.
- Массив / Array - коллекция эллементов, доступ к которым осуществляется по
индексам. Пример: `const cities = ['Tehran', 'Yalta', 'Potsdam'];`
- Отладка / Debug - процесс обнаружения и устранения ошибок в программном
обеспечении при помощи вывода сообщений или инструментов: отладчика,
профилировщика, декомпилятора, систем мониторинга ресурсов и логирования,
систем непрерывной интеграции и тестирования.
- ЦП / CPU - центральный процессор / central processing unit - устройство,
выполняющее машинные инструкции.
- АЛУ / ALU - блок ЦП, выполняющий арифметические и логические преобразования
над машинными словами, представляющими целые числа, числа с плавающей точкой,
адресами памяти, строками, логическими величинами.
- Компонент / Component - несколько программных объектов (например: функций,
классов, монад, типов) объединенных и организованных по общему признаку.
- Модуль / Module - целостный, функционально полный, независимый компонент
программной системы имеющий имя, интерфейс, реализацию.
- [Модульность / Modularity](https://github.com/HowProgrammingWorks/Modularity)
  - модульность повышает переиспользование кода, упрощает интеграцию компонентов,
  улучшает компоновку и тестирование программ по частям;
  - ограничения: модули не должны использовать глобальные переменные или
  модифицировать базовые классы/прототипы/функции языка программирования,
  платформы и/или фреймворка; модули должны быть слабо связаны, а
  взаимодействовать друг с другом должны через внешнее API (предпочтительно)
  или шину событий (если система построена на событийной модели, подписке).
- Библиотека / Library - сборник программных объектов (например: функций,
классов, монад, типов) подготовленный для повторного использования (часто
опубликованный). Библиотека это более крупная логическая часть кода, чем
компонент. Иногда библиотеку используют как синоним модуля, а иногда библиотека
состоит из нескольких модулей.
- Сложность / Complexity
  - Вычислительная сложность / Computational complexity
  - Колмогоровская (описательная) сложность / Kolmogorov (descriptive) complexity
  - Если нет циклов, то описательная коррелирует с вычислительной

## Основные понятия

- [Объект или Экземпляр / Object or Instance](https://github.com/HowProgrammingWorks/DataTypes) -
структура данных, содержащая состояние и методы, связанные с этим состоянием.
Объект может быть создан как литерал `{}` или экземпляр класса `new ClassName()`
или как экземпляр прототипа `new PrototypeConstructor()` или возвращен из фабрики.
  - `const person = { name: 'Marcus', city: 'Roma', born: 121 };`
  - `const person = new Person('Marcus', 'Roma', 121);`
- [Класс / Class](https://github.com/HowProgrammingWorks/Prototype) -
программная абстракция, объединяющая состояние и поведение (свойства и методы)
своих экземпляров (инстансов).
  - `class Point { constructor(x, y) { this.x = x; this.y = y; } }`
  - `class Rect { move(x, y) { this.x += x; this.y += y; } }`
  - `class Square extends Rect { constructor(x, y, m) { super(x, y, m, m); } }`
  - `class Point { static from(point) { return new Point(this.x, this.y); } }`
- [Прототип / Prototype](https://github.com/HowProgrammingWorks/Prototype) -
специальный объект, на который ссылаются его экземпляры и наследники. Свойства
прототипа становятся видны у наследников, если эти свойства не переопределены у
наследников. Формируется цепочка прототипов, по которой происходит
последовательный поиск свойств, пока они не будут найдены или пока не будет
достигнут конец цепочки наследования. Иногда под прототипом понимается шаблон,
который клонируется во время инстанциирования (не для JavaScript).
- Инстанциирование / Instantiation - создание объекта (экземпляра) или выделение
памяти для структуры данных.
  - `const rect = new Rectangle(-50, -50, 100, 150);`
  - `const rect = { a: { x: -50, y: -50 }, b: { x: 100, y: 150 } };`
  - `const cities = new Array(1000);`
  - `const cities = ['Tehran', 'Kiev', 'Yalta', 'Beijing', 'Potsdam', 'London'];`
- Область видимости / Scope - часть кода, из которой "виден" идентификатор.
- Лексический контекст / Lexical environment - набор идентификаторов, связанных
с определенными значениями в рамках функции или блока кода (в том числе блоков
циклов, условий и т.д.).
- Объектный контекст функции - объект, связанный со служебным идентификатором
`this`. Все функции, кроме стрелочных, могут быть связаны с объектным контекстом.
Объект связан с `this` если функция являются методами этого объекта, если функция
привязана к менму через `bind` или вызвана через `apply` и `call`.
- Глобальный контекст / Global context - глобальный объект-справочник. Если
идентификатор не находится ни в одном из вложенных лексических контекстов, то
будет выполнен его поиск в глобальном контексте (global, window, sandbox).
- Объявление функции / Function definition - способ объявления функции, который
виден из любого места в лексическом контексте, в котором объявлена функция,
пример: `function sum(a, b) { return a + b; }`
- Функциональное выражение / Function expression - связывание функции с
идентификатором при помощи присвоения, при котором значение будет доступно через
идентификатор не во всем лексическом контексте, а только после места присвоения.
Имеет несколько синтакчических вариантов:
  - функциональное выражение с именованной функцией / Named function expression
    - `const max = function max(a, b) { return a + b; };`
  - анонимное функциональное выражение / Anonymous function expression
    - `const max = function(a, b) { return a + b; };`
  - лямбда-функция / Lambda function
    - `const max = (a, b) => { return a + b; };`
  - лябмда-выражение, Функция-стрелка / Lambda expression, Arrow function
    - `const max = (a, b) => (a + b);`
- [Чистая функция / Pure Function](https://github.com/HowProgrammingWorks/Function)
  - функция, вычисляющая результат только на основе аргументов, не имеющая
  состояния и не обращающаяся к операциям ввода-вывода
  - функция, результат которой всегда детерминированный, т.е. для любого
  аргумента всегда будет один и тот же результат
  - функция, не имеющая побочных эффектов (см. побочный эффект)
- [Замыкание / Closure](https://github.com/HowProgrammingWorks/Closure)
  - если вернуть функцию `g` из функции `f`, то `g` будет видеть контекст
  функции `f`, так же, как и свои аргументы
  - если `f` возвращает `g`, то говорят, что экземпляр `g` замкнул контекст `f`
  - способ, позволяющий связать функцию с контекстом (с данными или
  переменными контекста)
  - замыкание является аналогом свойств в ООП, тоже связывающие свойства с
  методами через объект, по сути объект в ООП сам является контекстом
  связывания
  - при помощи замыкания можно реализовать функциональное наследование
  - `const add = a => b => a + b;`
  - `const hash = (data = {}) => (key, value) => (data[key] = value, data);`
- [Суперпозиция / Superposition](https://github.com/HowProgrammingWorks/Composition)
  - объединение вызова функций в выражения таким образом, что результат одних
  функций становится аргументами других функций
  - `const expr2 = add(pow(mul(5, 8), 2), div(inc(sqrt(20)), log(2, 7)));`
- [Композиция / Composition](https://github.com/HowProgrammingWorks/Composition)
  - `const compose = (f1, f2) => x => f2(f1(x));`
  - `const compose = (...funcs) => (...args) => (funcs.reduce((args, fn) => [fn(...args)], args));`
- [Частичное применение / Partial application](https://github.com/HowProgrammingWorks/PartialApplication)
  - `const partial = (fn, x) => (...args) => fn(x, ...args);`
- [Каррирование / Currying](https://github.com/HowProgrammingWorks/PartialApplication)
  - `const result = curry((a, b, c) => (a + b + c))(1, 2)(3);`
- [Побочные эффекты / Side effects](https://github.com/HowProgrammingWorks/Function)
- [Функция высшего порядка / Higher-order Function](https://github.com/HowProgrammingWorks/HigherOrderFunction)
  - если функция только в аргументах, то это колбек
  - если функция только в результате, то это фабрика функций на замыканиях
  - если возвращаемая функция имеет тот же смысл, что и получаемая в
  аргументах (+ дополнительное поведение), то это обертка
  - очень редко бывает, что возвращаемая функция не связана с функцией из
  аргументов (но пока ни кто не нашел вразумительного примера, где это
  реально нужно)
  - если на выходе класс или функция-конструктор, то это фабрики классов и
  прототипов соответсвенно
- Функциональное наследование / Functional Inheritance
  - при помощи замыканий, ч.п., каррирования, лямбд
- [Обертка / Wrapper](https://github.com/HowProgrammingWorks/Wrapper)
  - функция, которая оборачивает другую функцию (иногда объект, интерфейс или
  функциональный объект), добавляя ему дополнительное поведение
  - можно обернуть целый API интерфейс и даже асинхронную функцию вместе с
  колбеками (если известен контракт)
- [Дженерики / Generics](https://github.com/HowProgrammingWorks/Generics)
  - Обобщенное программирование - парадигма, позволяющая обобщенно описать
  алгоритмы и структуры данных, абстрагируясь от конкретных типов.
- Интерфейс / Interface
  - набор методов (функций) объединенных или общим объектным контекстом или
  применением к структурам данных одной предметной области т.е. смыслом (API)
  - способ определения (спецификации) контракта, по которому связаны
  программные компоненты
  - Набор методов с их именами, аргументами и типами аргументов
- Программный интерфейс / Application Interface, API
  - интерфейс программных компонентов: модулей, слоев абстракции, приложений
- [Синглтон / Singleton](https://github.com/HowProgrammingWorks/Singleton)
  - шаблон проектирования, предполагающий, что в одном пространстве имен
  (процессе, приложении, базе данных) будет только один экземпляр класса
  (или просто один подобный объект) к которому можно обратиться по определенному
  (известному) имени
- [Функция обратного вызова, колбек / Callback](https://github.com/HowProgrammingWorks/Callbacks)
  - функция передаваемая в качестве аргумента в другую функцию (или метод)
  для того, чтобы быть вызванной для возврата значения, ошибки или уведомления
  - функции обратного вызова имеют подтипы:
    - один раз вызываемые (чаще всего)
    - [Событие / Event](https://github.com/HowProgrammingWorks/Callbacks)
    - [Лисенер / Listener](https://github.com/HowProgrammingWorks/Callbacks)
- [Итерирование / Iteration](https://github.com/HowProgrammingWorks/Iteration)
  - многократное повторение одного блока кода или одной функции над различными
  данными: элементами массивов, множеств, списков, коллекций и различными
  значениями переменной цикла
- [Итератор / Iterator](https://github.com/HowProgrammingWorks/Iteration)
  - интерфейс доступа к элементам коллекции: массива, множества, списка
- [Файл / File](https://github.com/HowProgrammingWorks/Files)
- [Поток, Файловый поток / Stream, File Stream](https://github.com/HowProgrammingWorks/Streams)
- [Сокет / Socket](https://github.com/HowProgrammingWorks/Socket)
  - программный интерфейс (или абстракция) для обмена данными между процессами
- [Дескриптор / Handle](https://github.com/HowProgrammingWorks/Files)
  - уникальный идентификатор программного объекта (чаще всего объекта операционной
  системы): файла, сокета, окна, таймера, оединения и т.д.
- Состояние / State - совокупность данных программного компонента (переменных
и структур данных), определяющие его поведение и реакцию на операции с ним.
- Кэш / Cache - место временного хранения данных (буфер, коллекция, область
памяти) для быстрого доступа и оптимизации. Возможно кеширование операций
чтения, вычислений, операций записи (когда запись не может быть поизведена
достаточно быстро) или упрезжающее чтение в буфер (когда можно определить,
какие данные будут запрошены с наибольшей вероятностью).
- Хэширование / Hashing - преобразование данных произвольной длины (буфера,
массива, объекта или структуры данных) в последовательность битов определенной
длины (хеш) при помощи хеш-функции (при изменении хоть 1 бита в данных хеш
меняется существенно).
- [Функциональный объект](https://github.com/HowProgrammingWorks/Functor) -
объект функционального типа, который является функцией и объектом одновременно.
Другими словами, функциональный объект может быть вызван, как функция и может
иметь свойства и методы, как объект.
- [Функтор / Functor](https://github.com/HowProgrammingWorks/Functor) - это
функциональный объект, который является еще и рекурсивным замыканием. Функтор
хранит в замыкании защищенное значение и позволяющий отобразить это значение
в другой функтор через вызов функции (обычно `map`).
- [Аппликативный функтор](https://github.com/HowProgrammingWorks/Functor) -
функтор, который имеет метод `apply`.
- Монада / Monad - аппликативный функтор, который имеет метод `chain`.
- [Мемоизация / Memoization](https://github.com/HowProgrammingWorks/Memoization) -
обертка, сохраняющая результаты выполнения функции для предотвращения повторных
вычислений.
- [Примесь / Mixin](https://github.com/HowProgrammingWorks/Mixin) - добавление
свойств, методов или поведения к объекту после его инстанциирования. Пример:
`Object.assign(target, { field1, field2 }, { field3 });`
- Декоратор / Decorator - шаблон оборачивания объектов или функций для добавления
новой функциональности без наследования при помощи специального синтаксиса.
- [Наследование / Inheritance](https://github.com/HowProgrammingWorks/Inheritance)
- [Множественное наследование / Multiple Inheritance](https://github.com/HowProgrammingWorks/Inheritance)
- [Непрямое наследование / Indirect Inheritance](https://github.com/HowProgrammingWorks/Inheritance)
- [Генератор / Generator](https://github.com/HowProgrammingWorks/Generator)
- [Итератор / Iterable and Iterator](https://github.com/HowProgrammingWorks/Iterator)
- [Ввод/вывод / I/O, Input-output](https://github.com/HowProgrammingWorks/AsynchronousProgramming)
  - операции, выходящие за рамки CPU и RAM (арифметико-логического устройства
  и памяти), т.е. операции с устройствами ввода вывода: сеть, диск, порты,
  консоль (клавиатура и экран), друге переферийные устройства (взаимодействие
  с которыми на порядки медленнее, чем внутренние операции а АЛУ и памяти)
- [EventEmitter](https://github.com/HowProgrammingWorks/EventEmitter)
  - универсальная абстракция для работы с событиями чере подписку (subscription:
  addListener, on, once) и отправку (emit)
- [Чеининг / Chaining](https://github.com/HowProgrammingWorks/Chaining)
  - цепочный синтаксис вызова функций `total(april)(may)(july)` или методов
  `array.filter(f1).reduce(f2)`
- [Сериализация / Serialization](https://github.com/HowProgrammingWorks/Serialization)
  - преобразование структуры данных (развернутой в памяти) в битовую
  последовательность, обычно в последовательность байтов (бинарная сериализация)
  или в строку (текстовая сериализация)
- [Десериализация / Deserialization](https://github.com/HowProgrammingWorks/Serialization)
  - операция, обратная сериализации, т.е. восстановление структуры данных
  из последовательности битов (чаще байтов или строки)
- Парсинг / Parsing
  - синтаксический анализ текста, результатом чего может являться:
    - для формальной граматики - AST-дерево
    - для слабоструктурированного документа - структура данных, имеющая
    четкую структуру, в которую частично перенесены данные из слабой структуры
    - для других естественных или искуственных языков - информационные модели,
    им соответствующие
- [Регулярные выражения / Regular Expressions](https://github.com/HowProgrammingWorks/RegExp)
  - синтаксическая конструкция, паттерн, формальный язык, определяющий
  порядок парсинга другой синтаксической конструкции
- [Зависимость / Dependency](https://github.com/HowProgrammingWorks/Project)
  - связанность программных компонентов, при которой один компонент (зависимый)
  "знает" другой; это значит, что в нем помещен вызов метода (реализация которого
  содержится в другом) или он слушает событие, которое генерирует другой или
  он "знает" структуры данных, которые могут быть переданы из другого компонента
- Декомпозиция / Decomposition
  - разделение программного компонента на части по принципу функциональности,
  при этом, каждая часть будет решать подзадачу и появится часть кода, которая
  определяет порядок связи всех частей (композицию)
- [Ленивость / Lazy](https://github.com/HowProgrammingWorks/Lazy)
- [Обработка ошибок / Error handling](https://github.com/HowProgrammingWorks/Errors)
- [Фабрика / Factory](https://github.com/HowProgrammingWorks/Factory)
  - функция или метод для инстациирования объектов, функций, структур данных и
  любых других программных абстракций, например, экземпляров класса в обход
  конструктора или функциональных объектов
- Объектный Пул / [Object Pool](https://github.com/HowProgrammingWorks/Pool)
  - Множество заранее инстанциированных объектов (или массивов, сокетов, буферов,
  структур данных и других программных абстракций) из которого мы можем их брать
  инициализированные экземпляры (вместо инстанциирования новых) и отдавать их
  после использования
- [Таймеры / Timers](https://github.com/HowProgrammingWorks/Timers)
- [Адаптер / Adapter](https://github.com/HowProgrammingWorks/Adapter)
  - Паттерн достижения совместимости, позволяющий обернуть класс, функцию или
  другой программный компонент с несовместимым контрактом в программный
  компонент с контрактом, который нам нужен.
- [Стратегия (Strategy)](https://github.com/HowProgrammingWorks/Strategy)
  - Паттерн реализует выбор одного из совместимых и взаимозаменяемых классов,
  которые содержат поведение (алгоритм), аналогичный по функциональности и
  реализующий общий интерфейс. Актуален и для функционального программирования.
- [Фасад / Facade](https://github.com/HowProgrammingWorks/Facade)
  - Паттерн для скрытия сложности. Фасад скрывает несколько инстансов разных
  классов в своих свойствах (иногда приватных, но для JS этого пока нет) и
  предоставляет общий (фасадный) интерфейс для управления ими.
  - Для функционального программирования возможен аналог фасада - функция
  обертка, скрывающая инстансы в своем контексте и предоставляющая доступ
  к ним через возврат функции (с замыканием) или другого инстанса (методы
  которого тоже имеют доступ к скрываемым инстансам через замыкание).

## Вспомогательные материалы

- [Линтер / Linter](https://github.com/HowProgrammingWorks/Tools)
  - статический анализатор кода (без запуска), который может определить и
  предложить стилистические, грамматические или оптимизационное улучшение или
  просто выявить проблему (а иногда и исправить ее автоматически)
- Система контроля версий
- Менеджер пакетов
- Непрерывная интеграция
- Тестирование

## Структуры данных

- [Запись или структура / Struct or Record](https://github.com/HowProgrammingWorks/DataStructures)
- [Массив / Array](https://github.com/HowProgrammingWorks/DataStructures)
- [Буфер / Buffer](https://github.com/HowProgrammingWorks/Buffers)
- [Список / List](https://github.com/HowProgrammingWorks/LinkedList)
  - Односвязный, двусвязный, кольцевой, развернутый список (список массивов)
  - Реализация на объектах, массивах и замыканиях
  - Реализация на синтаксисе прототипов, классов и фабрик
  - Реализация на замыканиях и функциональных объектах
  - Реализация на одной и двух категориях (только узел или список и узел)
- [Стек, очередь, дек](https://github.com/HowProgrammingWorks/Dequeue)
  - Стек / Stack - Список, работающий про принципу LIFO
  - Очередь / Queue - Список, работающий про принципу FIFO
  - [Дек / Dequeue](https://github.com/HowProgrammingWorks/Dequeue)
  двухсторонняя очередь (одновременно LIFO и FIFO)
- [Дерево](https://github.com/HowProgrammingWorks/Trees)
- [Двоичное дерево](https://github.com/HowProgrammingWorks/Trees),
поисковое дерево, красно-черное дерево
- Куча / Heap - древовидная структура данных или область памяти для динамического
  распределения под хранение данных
- [Граф / Graph](https://github.com/HowProgrammingWorks/Graph)
- [Буфер / Buffer](https://github.com/HowProgrammingWorks/Buffers)
  - область памяти для хранения данных (обычно для операций ввода/вывода)
- Типизированные массивы
- [Коллекция / Collection](https://github.com/HowProgrammingWorks/Collections)
  - структура данных, служащая для хранения набора значений и предоставляющая
  доступ к ним по индексам или ключам
- [Множество / Set](https://github.com/HowProgrammingWorks/Set)
  - структура данных, реализующая математическое "множество"
  - структура данных, служащая для хранения однородного набора значений, которые
  не имеют индексов или ключей (но внутри структуры данных они должны иметь
  порядок, например, индекс в массиве, однако, множество абстрагирует нас от
  этой особенности реализации)
- [Ключ-значение, Хешмап / Map, Key-value](https://github.com/HowProgrammingWorks/KeyValue)
  - [класс `Map`](https://github.com/HowProgrammingWorks/Map)

## Расширенные понятия

- [Сборка мусора / Garbage Collection](https://github.com/HowProgrammingWorks/GarbageCollection)
- [Прокси / Proxy](https://github.com/HowProgrammingWorks/Proxy)
- [Символ / Symbol](https://github.com/HowProgrammingWorks/Symbol)
- [Дифер / Deferred](https://github.com/HowProgrammingWorks/Callbacks)
- [Промис / Promise](https://github.com/HowProgrammingWorks/Promise)
- [Необработанные ошибки в промисах на Node.js](https://github.com/HowProgrammingWorks/PromiseError)
- [Фьючер / Future](https://github.com/HowProgrammingWorks/Callbacks)
- [Коллекторы данных / Data and Key Collectors](https://github.com/metarhia/metasync/blob/master/lib/collector.js)
- Неизменяемые данные / Immutable Data
- Изменяемые данные / Mutable Data
- Интроспекция / Introspection
- Рефлексия / Reflection
- Скаффолдинг / Scaffolding
- [Инверсия управления / IoC, Inversion of Control](https://github.com/HowProgrammingWorks/InversionOfControl)
- [Внедрение зависимостей / DI, Dependency Injection](https://github.com/HowProgrammingWorks/DependencyInjection)
- [Межпроцессовое взаимодействие / IPC, Interprocess Communication](https://github.com/HowProgrammingWorks/InterProcessCommunication)
- [Песочница / Sandbox](https://github.com/HowProgrammingWorks/Sandboxes)
- Архитектура / Architecture
- Слой доступа к данным / Data Access Layer
- Курсор / Cursor
- Объектно-реляционное отображение / ORM, Object-relational Mapping
- [Сервер / Server](https://github.com/HowProgrammingWorks/NodeServer)
  - [Приклеивание по IP или идентификатору сессии / IP or Session Sticky](https://github.com/HowProgrammingWorks/NodeServer/tree/master/ip-sticky)
  - Кластеризация / Cluster mode
    - При помощи [cluster](https://github.com/HowProgrammingWorks/NodeServer/tree/master/native-cluster)
    - при помощи [child_process](https://github.com/HowProgrammingWorks/NodeServer/tree/master/native-cp)
  - [Разработка API (клиент и сервер)](https://github.com/HowProgrammingWorks/API)
- Сервер приложений / Application Server
- Тонкий клиент и толстый клиент
- [Проекция данных / Projection](https://github.com/HowProgrammingWorks/Projection)
- [Измерение производительности / Benchmarking](https://github.com/HowProgrammingWorks/Benchmark)
- [Интерфейс командной строки / CLI, Command Line Interface and Console](https://github.com/HowProgrammingWorks/CommandLine)
- [Мониторинг файловой системы / File System Watching](https://github.com/HowProgrammingWorks/FilesystemWatch)
- [Транзакционные объекты/Transaction](https://github.com/HowProgrammingWorks/Transaction)
- [Метаданные / Metadata](https://github.com/HowProgrammingWorks/Metaprogramming)
- [Протокол / Protocol](https://github.com/metarhia/metacom)
- [Динамическая загрузка модулей / Live Code Reload](https://github.com/HowProgrammingWorks/LiveReload)
- Http Request (HTTP, XMLHttpRequest, fetch): [примеры](https://github.com/HowProgrammingWorks/HttpRequest)
- [Неблокирующие итерации](https://github.com/HowProgrammingWorks/NonBlocking)
- [Линзы - функциональные аналоги геттера и сеттера](https://github.com/HowProgrammingWorks/Lenses)
- Состояние гонки / Race Condition - состояние в многопоточкой или конкурентной
программной системе, когда несколько потоков исполнения конкурируюя за общий
ресурс портят данные, приводят к непредусмотренному порядку исполнения,
зацикливаются, и т.д., что приводит к утечке ресурсов, непредсказуемому и
неправильному поведению, уязвимостям, нестабильности работы.
- Взаимная блокировка / Deadlock - состояние в многопроцессовой (распределенной)
системе, когда несколько процессов захватили ресурсы, необходимые для дальнейшей
работы друг друга, заблокировав, тем самым дальнейшую работу.
- Livelock - зацикленная блокировка, бесконечно изменяющея состояние, но не
выполняющая полезной работы.
- Ресурсный голод / Resource starvation - состояние в программной системе (обычно
многопоточной), когда она постоянно запрашивает доступ к ресурсам (обычно
разделяемым), и не может их получить.
- Критическая секция / Critical section - участок исполняемого кода, в котором
производится эксклюзивный доступ к разделяемому ресурсу.

## Примеры кода и комплексного использования технологий

- [Живые электронные таблицы / Live Table](https://github.com/HowProgrammingWorks/LiveTable)
- [Чат на вебсокетах / Websocket Chat](https://github.com/HowProgrammingWorks/WebsocketChat)
- [HTTP сессии на cookies](https://github.com/HowProgrammingWorks/Session)

## Асинхронное программирование

- [1. Асинхронное программирование (обзор)](https://youtu.be/hY6Z6qNYzmc)
- [2. Таймеры, таймауты и EventEmitter](https://youtu.be/LK2jveAnRNg)
  - Таймеры: https://github.com/HowProgrammingWorks/Timers
  - EventEmitter: https://github.com/HowProgrammingWorks/EventEmitter
  - События: https://github.com/metarhia/common/blob/master/lib/events.js
- [3. Асинхронное программирование на callback`ах](https://youtu.be/z8Hg6zgi3yQ)
  - Примеры кода: https://github.com/HowProgrammingWorks/AsynchronousProgramming
  - Библиотека do: https://github.com/metarhia/do
- [4. Неблокирующее асинхронное итерирование](https://youtu.be/wYA2cIRYLoA)
  - Примеры кода: https://github.com/HowProgrammingWorks/NonBlocking
- [5. Асинхронность с библиотекой async.js](https://youtu.be/XQ94wQc-erU)
  - Примеры кода: https://github.com/HowProgrammingWorks/AsynchronousProgramming
  - Библиотека async.js: https://caolan.github.io/async/
- [6. Асинхронность на промисах](https://youtu.be/RMl4r6s1Y8M)
  - Примеры кода: https://github.com/HowProgrammingWorks/Promise
- [7. Асинхронные функции и обработка ошибок](https://youtu.be/Jdf_tZuJbHI)
  - Примеры кода: https://github.com/HowProgrammingWorks/AsyncAwait
- [8. Асинхронные адаптеры: promisify, callbackify, asyncify](https://youtu.be/76k6_YkYRmU)
  - Примеры кода: https://github.com/HowProgrammingWorks/AsyncAdapter
- [9. Асинхронные коллекторы данных](https://youtu.be/tgodt1JL6II)
  - Примеры кода: https://github.com/HowProgrammingWorks/Collector
  - Библиотека: https://github.com/metarhia/metasync
- [10. Необработанные ошибки в промисах](https://youtu.be/1Ml5NE2fsZ8)
  - Примеры кода: https://github.com/HowProgrammingWorks/PromiseError
- [11. Проблема асинхронного стектрейса](https://youtu.be/pfiHTx3j87Y)
  - Примеры кода: https://github.com/HowProgrammingWorks/StackTrace
- [12. Генераторы и асинхронные генераторы](https://youtu.be/kvNm9D32s8s)
  - Генераторы: https://github.com/HowProgrammingWorks/AsyncGenerator
  - Асинхронные генераторы: https://github.com/HowProgrammingWorks/Generator
- [13. Итераторы и асинхронные итераторы](https://youtu.be/rBGFlWpVpGs)
  - Итераторы: https://github.com/HowProgrammingWorks/AsyncIterator
  - Асинхронные итераторы: https://github.com/HowProgrammingWorks/Iterator
- [14. Отмена асинхронных операций](https://youtu.be/T8fXlnqI4Ws)
  - Примеры кода: https://github.com/HowProgrammingWorks/Cancelable
- [15. Асинхронная композиция функций](https://youtu.be/3ZCrMlMpOrM)
  - Примеры кода: https://github.com/HowProgrammingWorks/AsyncCompose
- [16. Thenable и легковесный await](https://youtu.be/DXp__1VNIvI)
  - Примеры кода: https://github.com/HowProgrammingWorks/Thenable
- [17. Конкурентная асинхронная очередь](https://youtu.be/Lg46AH8wFvg)
  - Примеры кода: https://github.com/HowProgrammingWorks/ConcurrentQueue
- [18. Паттерн открытый конструктор (Revealing Constructor)](https://youtu.be/leR5sXRkuJI)
  - Примеры кода: https://github.com/HowProgrammingWorks/RevealingConstructor
- [19. Future: Асинхронность на фьючерах без состояния](https://youtu.be/22ONv3AGXdk)
  - Примеры кода: https://github.com/HowProgrammingWorks/Future
- [20. Deferred: Асинхронность на диферах с состоянием](https://youtu.be/a2fVA1o-ovM)
  - Примеры кода: https://github.com/HowProgrammingWorks/Deferred
- [21. Модель акторов (Actor Model)](https://youtu.be/xp5MVKEqxY4)
  - Примеры кода: https://github.com/HowProgrammingWorks/ActorModel
- [22. Паттерн Наблюдатель (Observer + Observable)](https://youtu.be/_bFXuLcXoXg)
  - Примеры кода: https://github.com/HowProgrammingWorks/Observer
- [23. Асинхронность на RxJS и потоки событий](https://youtu.be/0kcpMAl-wfE)
  - Примеры кода: https://github.com/HowProgrammingWorks/Rx

## Параллельное программирование

- [Потоки / Threads](https://github.com/HowProgrammingWorks/Threads)
  - SharedArrayBuffer
  - worker_threads в Node.js
- [Атомарные операции / Atomics](https://github.com/HowProgrammingWorks/Atomics)
- [Семафор / Semaphore](https://github.com/HowProgrammingWorks/Semaphore)
- [Мьютекс / Mutex](https://github.com/HowProgrammingWorks/Mutex)

## Парадигмы программирования

- [Императивное программирование / Imperative Programming](https://github.com/HowProgrammingWorks/ImperativeProgramming)
  - Неструктурное программирование / Non-structured
  - Структурное программирование / Structured Programming
  - Процедурное программирование / Procedural Programming
  - [Object-oriented programming](https://github.com/HowProgrammingWorks/ObjectOrientedProgramming)
  - [Prototype-oriented programming](https://github.com/HowProgrammingWorks/PrototypeOrientedProgramming)
- [Функциональное программирование / Functional Programming](https://github.com/HowProgrammingWorks/FunctionalProgramming)
  - [примеры разных стилей функционального кода](https://github.com/HowProgrammingWorks/Abstractions)
- Логическое программирование / Logical Programming
- Декларативное программирование / Declarative Programming
- [Программирование управляемое данными / Data-driven Programming](https://github.com/HowProgrammingWorks/DataDrivenProgramming)
- Техники программирования
  - [Асинхронное программирование / Asynchronous Programming](https://github.com/HowProgrammingWorks/AsynchronousProgramming)
  - Реактивное программирование / Reactive Programming
- [Событийное программирование / Event-driven Programming](https://github.com/HowProgrammingWorks/EventDrivenProgramming)
- [Метапрограммирование / Metaprogramming](https://github.com/HowProgrammingWorks/Metaprogramming)
