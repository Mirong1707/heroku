\hypertarget{ux43eux431ux449ux435ux435}{%
\section{Общее}\label{ux43eux431ux449ux435ux435}}

\begin{itemize}
\tightlist
\item
  В билете написано почти всё, что надо рассказать.
\item
  Для каждой синтаксической конструкции должен быть приведён
  содержательный пример, когда это требуется или делает код
  проще/удобнее.
\item
  Вас могут активно спрашивать вокруг билета: если вы сказали, что надо
  писать \texttt{Foo(bar)}, вас могут сразу же спросить, что будет при
  написании \texttt{Foo(\&bar)}, вы должны ответить.
\item
  ``Не было'' --- не было на лекции, знать не надо, не спрашивают. Даже
  если было на практике.
\end{itemize}

\hypertarget{ux43eux431ux44fux437ux430ux442ux435ux43bux44cux43dux44bux435-ux437ux43dux430ux43dux438ux44f}{%
\section{Обязательные
знания}\label{ux43eux431ux44fux437ux430ux442ux435ux43bux44cux43dux44bux435-ux437ux43dux430ux43dux438ux44f}}

Если вы не знаете какие-то термины что-то из списка ниже, это
автоматический неуд.

\hypertarget{ux442ux435ux440ux43cux438ux43dux44b}{%
\subsection{Термины}\label{ux442ux435ux440ux43cux438ux43dux44b}}

\begin{itemize}
\tightlist
\item
  Свободная функция, функция-член
\item
  Время жизни объекта: автоматическое, динамическое, статическое
\item
  Undefined behavior: что может произойти, примеры:

  \begin{itemize}
  \tightlist
  \item
    Неинициализированная переменная: почему у неё нет никакого значения.
  \item
    Выход за границы массива.
  \item
    Dangling reference (висячая ссылка) при возврате из функции, при
    инвалидации в стандартном контейнере.
  \item
    Разыменование \texttt{nullptr}.
  \end{itemize}
\end{itemize}

\hypertarget{ux43fux435ux440ux435ux43cux435ux43dux43dux44bux435}{%
\subsection{Переменные}\label{ux43fux435ux440ux435ux43cux435ux43dux43dux44bux435}}

\begin{itemize}
\tightlist
\item
  статическая типизация
\item
  тип переменной
\item
  размер переменной, размер типа
\item
  типы int, char: типичные размеры. Например, на архитектуре x86\_64 под
  Linux в компиляторе GCC.
\end{itemize}

\hypertarget{ux43eux441ux43dux43eux432ux43dux44bux435-ux43aux43eux43dux441ux442ux440ux443ux43aux446ux438ux438-ux44fux437ux44bux43aux43eux432-c-ux438-c}{%
\subsection{Основные конструкции языков C и
C++}\label{ux43eux441ux43dux43eux432ux43dux44bux435-ux43aux43eux43dux441ux442ux440ux443ux43aux446ux438ux438-ux44fux437ux44bux43aux43eux432-c-ux438-c}}

\begin{itemize}
\tightlist
\item
  объявления переменных
\item
  выражения и операторы:

  \begin{itemize}
  \tightlist
  \item
    арифметические (\texttt{+}, \texttt{-}, \texttt{*}, \texttt{/},
    \texttt{\%}, \texttt{+=}, \texttt{-=}, \texttt{*=}, \texttt{/=},
    \texttt{\%=}, \texttt{++}, \texttt{-\/-})
  \item
    булевы (\texttt{\textless{}}, \texttt{\textless{}=},
    \texttt{\textgreater{}}, \texttt{\textgreater{}=}, \texttt{==},
    \texttt{!=}, \texttt{\&\&}, \texttt{\textbar{}\textbar{}},
    \texttt{!})
  \item
    на минимальную оценку необязательно знать: отличия постфиксных и
    префиксных операторов
  \end{itemize}
\item
  условный оператор \texttt{if}
\item
  циклы \texttt{for}, \texttt{while}
\end{itemize}

\hypertarget{ux444ux443ux43dux43aux446ux438ux438}{%
\subsection{Функции}\label{ux444ux443ux43dux43aux446ux438ux438}}

\begin{itemize}
\tightlist
\item
  объявление и определение функции, требуется отличать между собой
  (можно случайно перепутать, но после вопроса исправиться)
\item
  вызов функции (синтаксис, не нужно знать mangling, конвенции вызовов)
\item
  возвращаемое значение
\item
  рекурсивный вызов
\end{itemize}

\hypertarget{ux43eux441ux43dux43eux432ux43dux44bux435-ux43aux43eux43dux441ux442ux440ux443ux43aux446ux438ux438-c}{%
\subsection{Основные конструкции
C++}\label{ux43eux441ux43dux43eux432ux43dux44bux435-ux43aux43eux43dux441ux442ux440ux443ux43aux446ux438ux438-c}}

\begin{itemize}
\tightlist
\item
  синтаксис \texttt{static\_cast}
\item
  синтаксис объявления пространств имён, обращения к элементу внутри
  пространства имён
\item
  \texttt{auto} для объявления переменных
\item
  range-based for, в том числе с \texttt{auto\&} и
  \texttt{const\ auto\&}
\item
  синтаксис шаблонов, достаточный для написания минимального адаптера
  \texttt{stack\textless{}T\textgreater{}} поверх \texttt{deque}
\end{itemize}

\hypertarget{ux43aux43bux430ux441ux441ux44b}{%
\subsection{Классы}\label{ux43aux43bux430ux441ux441ux44b}}

\begin{itemize}
\tightlist
\item
  определение класса, конструктор, деструктор, методы
\item
  специальные методы (пять штук), правило нуля, правило пяти
\item
  приватные/публичные поля и методы
\end{itemize}

\hypertarget{const-correctness}{%
\subsection{Const correctness}\label{const-correctness}}

\begin{itemize}
\tightlist
\item
  синтаксис константных ссылок, применение при передаче аргументов
\item
  невозможность изменять константные объекты и их поля
\item
  const-qualifier у методов (const member function), перегрузка по
  const-qualifier (const overloading)
\end{itemize}

\hypertarget{ux438ux441ux43fux43eux43bux44cux437ux43eux432ux430ux43dux438ux435-move-ux441ux435ux43cux430ux43dux442ux438ux43aux438}{%
\subsection{Использование
move-семантики}\label{ux438ux441ux43fux43eux43bux44cux437ux43eux432ux430ux43dux438ux435-move-ux441ux435ux43cux430ux43dux442ux438ux43aux438}}

\begin{itemize}
\tightlist
\item
  эффективная инициализация полей класса из аргументов, принятых по
  значению или по rvalue-ссылке
\item
  moved-from состояние у объектов: может быть не определено, может быть
  невозможно обнаружить, пример ошибки
\item
  отсутствие необходимости \texttt{move} из результата функции,
  возвращённого по значению
\item
  необходимость move для явной передачи владения \texttt{unique\_ptr}
\item
  почему \texttt{std::move} не выполняет никакого кода
\end{itemize}

\hypertarget{stl}{%
\subsection{STL}\label{stl}}

\begin{itemize}
\tightlist
\item
  использование \texttt{vector} как динамического массива фиксированной
  длины, push\_back и emplace\_back
\item
  использование \texttt{map} со стандартным компаратором, особенность
  operator{[}{]} (создаёт значение даже при чтении)
\end{itemize}

\hypertarget{ux431ux438ux43bux435ux442ux44b}{%
\section{Билеты}\label{ux431ux438ux43bux435ux442ux44b}}

\hypertarget{ux431ux430ux437ux43eux432ux44bux439-ux441ux438ux43dux442ux430ux43aux441ux438ux441}{%
\subsection{1. Базовый
синтаксис}\label{ux431ux430ux437ux43eux432ux44bux439-ux441ux438ux43dux442ux430ux43aux441ux438ux441}}

\begin{itemize}
\item
  Отличия и примерные границы значений встроенных типов (``на
  контесте''):

  \begin{itemize}
  \tightlist
  \item
    \texttt{int}, \texttt{double} (почему
    \texttt{0.1\ +\ 0.2\ !=\ 0.3}), \texttt{bool}.
  \item
    Знаковость и беззнаковость типов.
  \end{itemize}
\item
  Литералы: целочисленный и вещественный (в том числе
  \texttt{10\textquotesingle{}000} с C++14), символьный.
\item
  Строковые литералы: обычный, raw string literal, экранирование
  (escaping).
\item
  Склейка подряд написанных строковых литералов.
\item
  \texttt{static\_cast\textless{}\textgreater{}}: пример избавления от
  переполнения при умножении \texttt{int}'ов.
\item
  Разница между \texttt{i++} и \texttt{++i}.
\item
  Составные операторы присваивания (compound assignment operator) вроде
  \texttt{*=}, \texttt{/=}.
\item
  Expression и statement, что такое тип expression.
\item
  Синтаксис: \texttt{for} (включая объявление переменной в
  \texttt{init}), \texttt{while}, \texttt{if}, где expression и
  statement.
\item
  Range-based \texttt{for}, в том числе с использованием (константных)
  ссылок и \texttt{auto}, где возникают копирования.
\item
  Порядок вычислений: https://notes.algoprog.ru/cpp/additional.html\#id4

  \begin{itemize}
  \tightlist
  \item
    Внутри выражений: аргументы функции, операнды операторов.
  \item
    При инициализации нескольких переменных.
  \item
    При инициализации при помощи \texttt{\{\}}.
  \item
    Что изменилось в C++17, почему в \texttt{a\ =\ b} важно сначала
    вычислить \texttt{b}, потом \texttt{a}.
  \end{itemize}
\end{itemize}

\hypertarget{ux43eux431ux44aux44fux432ux43bux435ux43dux438ux435-ux43eux431ux44aux435ux43aux442ux43eux432-ux432ux43dux443ux442ux440ux438-ux43eux434ux43dux43eux433ux43e-ux444ux430ux439ux43bux430}{%
\subsection{2. Объявление объектов внутри одного
файла}\label{ux43eux431ux44aux44fux432ux43bux435ux43dux438ux435-ux43eux431ux44aux435ux43aux442ux43eux432-ux432ux43dux443ux442ux440ux438-ux43eux434ux43dux43eux433ux43e-ux444ux430ux439ux43bux430}}

\begin{itemize}
\tightlist
\item
  Допустимые имена переменных, функций, констант, классов:

  \begin{itemize}
  \tightlist
  \item
    Нельзя начинать с цифры.
  \item
    Где посмотреть ключевые слова.
  \item
    Где можно и нельзя ставить \texttt{\_}:
    https://stackoverflow.com/questions/228783/what-are-the-rules-about-using-an-underscore-in-a-c-identifier
  \item
    Что происходит от некорректного имени в разных случаях.
  \end{itemize}
\item
  Объявление и определение: функции, класса, в том числе шаблонного.
\item
  Взаимная рекурсия для: функций, классов, методов внутри одного класса,
  методов между классами (\texttt{A::foo()} возвращает \texttt{B} и
  наоборот).
\item
  Пространства имён: глобальное, вложенное, синтаксис для объявления
  вложенных namespace с C++11.

  \begin{itemize}
  \tightlist
  \item
    Почему нельзя просто сделать класс со статическими членами?
  \end{itemize}
\item
  Обращение к вложенному namespace, к глобальному namespace.
\item
  Псевдонимы типов: \texttt{typedef}, \texttt{using},
  \texttt{template\textless{}\textgreater{}\ using}.
\item
  \texttt{using\ namespace}, где можно и нельзя использовать и почему,
  особенности
  \texttt{using\ namespace\ \textless{}другая-библиотека-вроде-std\textgreater{}}.
\end{itemize}

Тесно связано с: линковка.

\hypertarget{ux43eux431ux44aux44fux432ux43bux435ux43dux438ux435-ux43fux435ux440ux435ux43cux435ux43dux43dux44bux445}{%
\subsection{3. Объявление
переменных}\label{ux43eux431ux44aux44fux432ux43bux435ux43dux438ux435-ux43fux435ux440ux435ux43cux435ux43dux43dux44bux445}}

\begin{itemize}
\tightlist
\item
  Объявление нескольких переменных, указателей, ссылок, в том числе
  константных.
\item
  Создание временного объекта.
\item
  C++17: существование Class Template Argument Deduction, пример.
\item
  Отличия copy initialization и direct initialization.

  \begin{itemize}
  \tightlist
  \item
    Тесно связано с: преобразования (conversions).
  \end{itemize}
\item
  Неинициализированные переменные/поля.
\item
  \texttt{{[}{[}maybe\_unused{]}{]}}
\item
  Инициализация при помощи \texttt{\{\}}:

  \begin{itemize}
  \tightlist
  \item
    Для тривиальных типов.
  \item
    Для нетривиальных типов.
  \item
    Для массивов/векторов, в том числе вложенных.
  \item
    Временных объектов.
  \item
    Не было: точное определение агрегатных классов.
  \end{itemize}
\item
  Пример, где инициализация через \texttt{\{\}} и \texttt{()}
  компилируются и ведут себя по-разному.
\item
  Ссылки.

  \begin{itemize}
  \tightlist
  \item
    Можно ли отличить ссылку от объекта, на который она указывает.
  \item
    Использование константных ссылок.
  \item
    Константная ссылка не обещает, что объект не меняется (если ссылка
    на мутабельный объект).
  \end{itemize}
\item
  \texttt{auto} и его модификации, как выводится тип.

  \begin{itemize}
  \tightlist
  \item
    Конвенция Almost Always Auto, в том числе для шаблонных типов.
  \end{itemize}
\item
  Необходимость слова \texttt{typename} в некоторых случаях.
\item
  Structured binding для пар, простых структур, массивов, со ссылкой.

  \begin{itemize}
  \tightlist
  \item
    Не было: как делать для своих структур, что на самом деле происходит
    внутри, что происходит с временными значениями.
  \end{itemize}
\end{itemize}

Тесно связно с: параметры функций.

\hypertarget{ux444ux443ux43dux43aux446ux438ux438-1}{%
\subsection{4. Функции}\label{ux444ux443ux43dux43aux446ux438ux438-1}}

\begin{itemize}
\tightlist
\item
  Параметры

  \begin{itemize}
  \tightlist
  \item
    Синтаксис (пропущенное имя, значение по умолчанию в
    объявлении/определении)
  \item
    Передача параметров по: значению, \texttt{\&}, \texttt{const\&},
    \texttt{\&\&}. Что выбрать при наличии или отсутствии move-семантики
    и почему.
  \item
    Примеры: \texttt{push\_back}, \texttt{Person(string\ first\_name)}.
  \item
    Передача \texttt{\{\}} в параметры.
  \end{itemize}
\item
  Возвращаемый тип

  \begin{itemize}
  \tightlist
  \item
    Использование \texttt{auto} и \texttt{-\textgreater{}}, удобство при
    определении функций-членов
  \item
    Как выводится просто \texttt{auto} (возможно, с модификаторами), в
    том числе для рекурсии и \texttt{void}.
  \end{itemize}
\item
  Возвращаемое значение

  \begin{itemize}
  \tightlist
  \item
    Возврат по значению, ссылке, константной ссылке.
  \item
    Возврат \texttt{\{\}} и взаимодействие с \texttt{auto}.
  \item
    \texttt{{[}{[}nodiscard{]}{]}}, возможные стратегии применения:
    когда не имеет смысла игнорировать возвращаемое значение, когда
    игнорировать опасно
  \end{itemize}
\item
  Перегрузка функций:

  \begin{itemize}
  \tightlist
  \item
    Что входит в сигнатуру, что не входит.
  \item
    Синтаксис \texttt{=\ delete} с C++11.
  \item
    Проблемы с разделением \texttt{nullptr}, \texttt{NULL}, \texttt{0}.
  \item
    Не было: \texttt{noexcept}.
  \item
    Не было: правил выбора перегрузки точнее ``выбирается перегрузка
    наиболее точная или ambiguous''.
  \end{itemize}
\item
  Указатели на функции: синтаксис, использование.

  \begin{itemize}
  \tightlist
  \item
    Не было: конверсии между указателями, что происходит с перегрузками.
  \end{itemize}
\end{itemize}

Тесно связано с: методы.

\hypertarget{ux436ux438ux437ux43dux44c-ux43eux431ux44aux435ux43aux442ux43eux432}{%
\subsection{5. Жизнь
объектов}\label{ux436ux438ux437ux43dux44c-ux43eux431ux44aux435ux43aux442ux43eux432}}

\begin{itemize}
\tightlist
\item
  Семантика копирования: что ожидается в C++ при переприсваивании
  объекта, передаче в качестве аргумента функции, возврата из функции.

  \begin{itemize}
  \tightlist
  \item
    А если не \texttt{Foo\ a;}, а \texttt{Foo\ \&a\ =\ .....;}?
  \end{itemize}
\item
  Время жизни объектов (storage): автоматическое (automatic),
  ручное/динамическое (dynamic), статическое (static).

  \begin{itemize}
  \tightlist
  \item
    Синтаксис создания/удаления объекта.
  \item
    Когда вызывается конструктор/деструктор и с какими параметрами.
  \end{itemize}
\item
  Время жизни временных объектов.

  \begin{itemize}
  \tightlist
  \item
    Когда создаётся/уничтожается временный объект (``наивный взгляд'' до
    C++14 включительно).
  \item
    Продление жизни временого объекта.
  \item
    Проблема продления жизни в \texttt{std::min()}/\texttt{std::max()}.
  \item
    Проблема продления жизни в range-based-for и цепочке вызовов
    \texttt{foo().bar()}.
  \end{itemize}
\item
  Локальные объекты со static storage duration (локальные статические
  переменные):

  \begin{itemize}
  \tightlist
  \item
    Когда создаётся/уничтожается.
  \item
    Чем инициализируются, можно ли инициализировать параметром функции.
  \end{itemize}
\end{itemize}

Тесно связано с: move-семантика.

\hypertarget{move-ux441ux435ux43cux430ux43dux442ux438ux43aux430}{%
\subsection{6.
Move-семантика}\label{move-ux441ux435ux43cux430ux43dux442ux438ux43aux430}}

\begin{itemize}
\tightlist
\item
  Категории значений: lvalue/xvalue/prvalue; обобщённые glvalue/rvalue.

  \begin{itemize}
  \tightlist
  \item
    Определение в C++11/C++14.
  \item
    Определение в C++17 и позже.
  \end{itemize}
\item
  rvalue-ссылки и lvalue-ссылки: что к чему привязывается
\item
  Почему у move constructor и move assignment именно такая сигнатура,
  как работает разрешение перегрузок, почему не надо добавить
  \texttt{const}.
\item
  \texttt{std::move}: как работает, почему ничего не делает, где
  используется, как реализовать свой.
\item
  Примеры return value optimization, named return value optimization до
  C++17.
\item
  Guaranteed copy elision в C++17: новый смысл prvalue.
\item
  Возврат объектов:

  \begin{itemize}
  \tightlist
  \item
    Возврат неперемещаемых объектов из функции.
  \item
    Когда (не) надо писать \texttt{return\ std::move(foo);}
  \end{itemize}
\end{itemize}

Тесно связано с: функции (как передавать параметры), жизнь объектов.

\hypertarget{ux441ux442ux430ux43dux434ux430ux440ux442ux43dux430ux44f-ux431ux438ux431ux43bux438ux43eux442ux435ux43aux430}{%
\subsection{7. Стандартная
библиотека}\label{ux441ux442ux430ux43dux434ux430ux440ux442ux43dux430ux44f-ux431ux438ux431ux43bux438ux43eux442ux435ux43aux430}}

\begin{itemize}
\tightlist
\item
  Что такое \texttt{namespace\ std}.
\item
  Контейнеры

  \begin{itemize}
  \tightlist
  \item
    \texttt{std::vector}, \texttt{std::string}, \texttt{std::list},
    \texttt{std::map}: когда что использовать
  \item
    Основные операции и время работы:
    \texttt{push\_back}/\texttt{emplace\_back},
    \texttt{front()}/\texttt{back()}, \texttt{operator{[}{]}},
    \texttt{size()}, \texttt{capacity()}, \texttt{resize()},
    \texttt{reserve()}.
  \item
    Особенность \texttt{operator{[}{]}} у \texttt{std::map}: элемент
    всегда создаётся, даже если его не было, почему.
  \item
    Инвалидация итераторов и ссылок на элементы: когда, какие
    последствия.
  \end{itemize}
\item
  Итераторы

  \begin{itemize}
  \tightlist
  \item
    Конвенции с \texttt{begin()}/\texttt{end()}
  \item
    Не было: иерархия итераторов, \texttt{reverse\_iterator}.
  \end{itemize}
\item
  Алгоритмы

  \begin{itemize}
  \tightlist
  \item
    \texttt{sort}, передача своего компаратора.
  \item
    \texttt{lower\_bound}, \texttt{upper\_bound}, точные инварианты.
  \end{itemize}
\item
  Ввод-вывод

  \begin{itemize}
  \tightlist
  \item
    \texttt{cin}/\texttt{cout}/\texttt{ifstream}/\texttt{ofstream}/\texttt{istream}/\texttt{ostream}/\texttt{sstream}
  \item
    Какие \texttt{\#include} бывают (2 шт)
  \item
    Синтаксис ввода и вывода.
  \item
    Перегрузка операторов ввода-вывода для своих классов: конвенции,
    почему так работает, когда нужны friend-операторы и зачем.
  \item
    Не было: манипуляторы, свои манипуляторы.
  \end{itemize}
\end{itemize}

Тесно связано с: функторы, лямбда-функции, базовый синтаксис (порядок
вычислений).

\hypertarget{ux443ux43aux430ux437ux430ux442ux435ux43bux438}{%
\subsection{8.
Указатели}\label{ux443ux43aux430ux437ux430ux442ux435ux43bux438}}

\begin{itemize}
\tightlist
\item
  Базовый синтаксис: объявление, разыменование, взятие адреса,
  \texttt{-\textgreater{}}.

  \begin{itemize}
  \tightlist
  \item
    Не было: многоуровневые указатели, aliasing.
  \end{itemize}
\item
  Реализация двусвязного списка, конструкции вроде
  \texttt{a.next-\textgreater{}prev}.
\item
  Нулевой указатель.

  \begin{itemize}
  \tightlist
  \item
    Отличия \texttt{nullptr} от \texttt{0}
  \item
    Проверка на нулевой указатель.
  \item
    Разменование \texttt{nullptr}.
  \end{itemize}
\item
  Ручное управление памятью: \texttt{new}, \texttt{delete},
  \texttt{new{[}{]}}, \texttt{delete{[}{]}}, когда что использовать.

  \begin{itemize}
  \tightlist
  \item
    Не было: разница между \texttt{new\ int;} и \texttt{new\ int();}
  \item
    Утечка памяти: UB ли, какие последствия, как ловить, как читать
    вывод sanitizer и Valgrind с примерами.
  \end{itemize}
\end{itemize}

\hypertarget{ux43aux43bux430ux441ux441ux44b-1}{%
\subsection{9. Классы}\label{ux43aux43bux430ux441ux441ux44b-1}}

\begin{itemize}
\tightlist
\item
  Синтаксис.
\item
  Поля: обычные, константные, ссылки, порядок создание и уничтожения и
  когда он важен.
\item
  Семантика копирования, особенности полей-констант/ссылок при
  копировании и инициализации.
\item
  Конструктор: синтаксис, параметры, когда вызывается, делегирующие
  конструкторы.
\item
  Инициализация полей: когда что можно и нужно использовать, как они
  взаимодействуют между собой и с делегирующим конструктором

  \begin{itemize}
  \tightlist
  \item
    По умолчанию (тривальных и с конструктором по умолчанию)
  \item
    Default member initializer (C++11)
  \item
    Member initialization list
  \item
    Переприсваивание в конструкторе
  \end{itemize}
\item
  Приватные/публичные поля и методы

  \begin{itemize}
  \tightlist
  \item
    Кто к кому может обращаться в том числе не у \texttt{this}
  \item
    Паттерн: геттеры и сеттеры для поддержания инвариантов
  \item
    Не было: \texttt{protected}, наследование.
  \end{itemize}
\item
  Отличия \texttt{struct}/\texttt{class}.
\item
  Агрегатная инициализация простых классов через \texttt{\{\}}

  \begin{itemize}
  \tightlist
  \item
    Не было: строгое определение ``простого класса'' и его отличия между
    стандартами C++11, C++14, C++17, C++20.
  \end{itemize}
\end{itemize}

\hypertarget{ux444ux443ux43dux43aux446ux438ux438-ux447ux43bux435ux43dux44b-ux43cux435ux442ux43eux434ux44b}{%
\subsection{10. Функции-члены
(методы)}\label{ux444ux443ux43dux43aux446ux438ux438-ux447ux43bux435ux43dux44b-ux43cux435ux442ux43eux434ux44b}}

\begin{itemize}
\tightlist
\item
  Синтаксис объявления и вызова через \texttt{.} или
  \texttt{-\textgreater{}}.
\item
  Ключевое слово \texttt{this}

  \begin{itemize}
  \tightlist
  \item
    Где его можно не писать, зачем писать хоть где-то.
  \item
    Чем метод отличается от свободной функции.
  \item
    Захват \texttt{this} в лямбды: \texttt{{[}{]}}, \texttt{{[}={]}},
    \texttt{{[}\&{]}}, \texttt{{[}this{]}}, \texttt{{[}*this{]}}.
  \end{itemize}
\item
  Ключевое слово \texttt{template} при вызове некоторых методов.
\item
  Const correctness: ограничение доступа к полям (в том числе ссылочным
  и указателям) при константном \texttt{this}.

  \begin{itemize}
  \tightlist
  \item
    Когда возникает константный \texttt{this}.
  \item
    Const qualifier и ограничения внутри такого метода.
  \item
    Перегрузка по const qualifier, когда нужна.
  \end{itemize}
\item
  Ref qualifier \texttt{\&} в терминах категорий значений, когда нужен.

  \begin{itemize}
  \tightlist
  \item
    Не было: ref qualifier \texttt{\&\&}.
  \end{itemize}
\item
  Определение методов внутри и снаружи класса, неявный \texttt{inline} и
  зачем.
\item
  Удобство \texttt{auto\ foo()\ -\textgreater{}\ Foo} при определении
  методов снаружи класса.
\end{itemize}

\hypertarget{ux441ux442ux430ux442ux438ux447ux435ux441ux43aux438ux435-ux447ux43bux435ux43dux44b-ux43aux43bux430ux441ux441ux430}{%
\subsection{11. Статические члены
класса}\label{ux441ux442ux430ux442ux438ux447ux435ux441ux43aux438ux435-ux447ux43bux435ux43dux44b-ux43aux43bux430ux441ux441ux430}}

\begin{itemize}
\tightlist
\item
  Статические поля: объявление, определение, когда что необходимо и где,
  обращение изнутри класса и снаружи, отличие от глобальных переменных.
\item
  Статические константы: объявления, определение, когда что нужно и где
  (для тривиальных и нетривиальных типов).

  \begin{itemize}
  \tightlist
  \item
    Не было: \texttt{constexpr}, \texttt{char{[}{]}}.
  \end{itemize}
\item
  Статические методы, отличие от свободных функций.
\item
  Паттерн: статический метод как конструктор с именем.
\end{itemize}

Тесно связано с: линковка.

\hypertarget{ux441ux43fux435ux446ux438ux430ux43bux44cux43dux44bux435-ux43cux435ux442ux43eux434ux44b}{%
\subsection{12. Специальные
методы}\label{ux441ux43fux435ux446ux438ux430ux43bux44cux43dux44bux435-ux43cux435ux442ux43eux434ux44b}}

\begin{itemize}
\tightlist
\item
  Деструктор, конструктор копирования/перемещения, оператор
  присваивания/перемещения.

  \begin{itemize}
  \tightlist
  \item
    Когда что вызывается: разная инициализация (copy, direct), передача
    как аргумента, возврат из функции.
  \end{itemize}
\item
  Реализация \texttt{unique\_ptr} и \texttt{shared\_ptr} (без deleter и
  массивов).
\item
  Правило пяти: формулировка.

  \begin{itemize}
  \tightlist
  \item
    Проблемы с самоприсваиванием.

    \begin{itemize}
    \tightlist
    \item
      Не было: корректность self-move, считаем, что не отличается от
      self-assignment.
    \end{itemize}
  \item
    Copy-swap-idiom превращает в правило четырёх.
  \end{itemize}
\item
  ``Нарушение'' правила пяти: когда деструктор может быть тривиальным, а
  копирование нетривиальным (list-heap и обобщение).
\item
  Как писать специальные методы в шаблонных классах.
\end{itemize}

\hypertarget{ux434ux440ux443ux437ux44cux44f-ux438-ux43fux435ux440ux435ux433ux440ux443ux437ux43aux430-ux43eux43fux435ux440ux430ux442ux43eux440ux43eux432}{%
\subsection{13. Друзья и перегрузка
операторов}\label{ux434ux440ux443ux437ux44cux44f-ux438-ux43fux435ux440ux435ux433ux440ux443ux437ux43aux430-ux43eux43fux435ux440ux430ux442ux43eux440ux43eux432}}

\begin{itemize}
\tightlist
\item
  Друзья-классы (в том числе шаблонные).
\item
  Друзья-функции (шаблонные --- в отдельном билете).

  \begin{itemize}
  \tightlist
  \item
    Определение внутри класса, снаружи класса.
  \item
    Объявление до класса, внутри класса.
  \end{itemize}
\item
  Виды перегружаемых операторов

  \begin{itemize}
  \tightlist
  \item
    Унарные, постфиксные/префиксные (как отличить при перегрузке?),
    бинарные, составное присваивание, сравнение.
  \item
    \texttt{operator*}, \texttt{operator-\textgreater{}} (в том числе
    вызов по цепочке).
  \item
    \texttt{operator()}.
  \item
    \texttt{operator{[}{]}}.
  \end{itemize}
\item
  Для каждого вида:

  \begin{itemize}
  \tightlist
  \item
    Что через кого выражать для минимизации лишних копирований и кода.
  \item
    Конвенция для типов параметров, типа возвращаемого значения.
  \item
    Делать оператор свободной функцией или членом, последствия для
    преобразований (conversions).
  \end{itemize}
\item
  Отличия \texttt{a\ +\ b}, \texttt{a.operator+(b)},
  \texttt{a.operator+()}.
\item
  Проблемы с самоприсваиванием и самомодификацией (пример простой
  некорректной реализации \texttt{/=} для класса рациональной дроби
  \texttt{Ratio}).
\item
  Не было: \texttt{operator\textless{}=\textgreater{}}
\end{itemize}

\hypertarget{ux43fux440ux435ux43eux431ux440ux430ux437ux43eux432ux430ux43dux438ux44f}{%
\subsection{14.
Преобразования}\label{ux43fux440ux435ux43eux431ux440ux430ux437ux43eux432ux430ux43dux438ux44f}}

\begin{itemize}
\tightlist
\item
  Конструкторы для преобразований и операторы преобразования.

  \begin{itemize}
  \tightlist
  \item
    Зачем два способа.
  \item
    Что когда выбирается, когда возникают неоднозначности.
  \end{itemize}
\item
  Допустимые цепочки преобразований: не более одного пользовательского,
  но числовые можно.
\item
  Где вызывается явное преобразование (explicit), а где неявное
  (implicit).

  \begin{itemize}
  \tightlist
  \item
    В том числе в \texttt{static\_cast\textless{}\textgreater{}}.
  \item
    В том числе при работе с функциями (параметры, возвращаемое
    значение) и комбинировании с \texttt{\{\}}. Например,
    \texttt{return\ \{\}}.
  \item
    В том числе для \texttt{bool}, но не других числовых типов. Не было:
    safe bool idiom.
  \end{itemize}
\item
  Ключевое слово \texttt{explicit}, зачем нужно для конструкторов с
  несколькими параметрами или с нулём параметров.
\end{itemize}

\hypertarget{ux448ux430ux431ux43bux43eux43dux44b-ux43aux43bux430ux441ux441ux43eux432}{%
\subsection{15. Шаблоны
классов}\label{ux448ux430ux431ux43bux43eux43dux44b-ux43aux43bux430ux441ux441ux43eux432}}

\begin{itemize}
\tightlist
\item
  Шаблоны классов.

  \begin{itemize}
  \tightlist
  \item
    Синтаксис объявления.
  \item
    Параметры шаблона: типы (разница \texttt{typename}/\texttt{class}),
    значения простых типов (без строго определения ``простоты'').
  \item
    Параметры по умолчанию, отсутствие имени у параметра.
  \item
    Параметры-шаблоны, передача в них шаблонов с параметрами по
    умолчанию.
  \item
    Ключевые слова \texttt{typename}, \texttt{template} для обращения
    внутрь зависимых типов.
  \end{itemize}
\item
  Отличие шаблона \texttt{Foo} и инстанцирования шаблона с параметрами
  по умолчанию \texttt{Foo\textless{}\textgreater{}}, когда что

  \begin{itemize}
  \tightlist
  \item
    Когда можно писать \texttt{Foo} вместо
    \texttt{Foo\textless{}T\textgreater{}}, удобство с
    \texttt{auto\ Foo\textless{}T\textgreater{}::foo()\ -\textgreater{}\ Foo}.
  \end{itemize}
\item
  Инстанцирование

  \begin{itemize}
  \tightlist
  \item
    Независимость по методам.
  \item
    Когда происходит неявное инстанцирование.
  \item
    Когда тип шаблона может быть incomplete, а когда не может.
  \item
    Не было: явное инстанцирование.
  \end{itemize}
\item
  Независимость инстанциаций шаблона.
\item
  Определение методов и статических членов шаблонного класса внутри и
  вне класса.
\end{itemize}

\hypertarget{ux43fux440ux43eux447ux438ux435-ux448ux430ux431ux43bux43eux43dux44b}{%
\subsection{16. Прочие
шаблоны}\label{ux43fux440ux43eux447ux438ux435-ux448ux430ux431ux43bux43eux43dux44b}}

\begin{itemize}
\tightlist
\item
  Шаблоны функций.

  \begin{itemize}
  \tightlist
  \item
    Автовывод параметров шаблона, когда не сработает.
  \item
    Базовое взаимодействие с перегрузками, синтаксис
    \texttt{foo\textless{}\textgreater{}(10);}.
  \end{itemize}
\item
  Шаблонные методы/конструкторы в обычных и шаблонных классах.

  \begin{itemize}
  \tightlist
  \item
    Определение внутри и вне класса.
  \end{itemize}
\item
  Автовывод параметров шаблона класса (Class Template Argument
  Deduction) из конструкторов: при инициализации переменных, при
  создании временных объектов.
\item
  Шаблоны переменных (C++17).
\end{itemize}

\hypertarget{ux441ux43fux435ux446ux438ux430ux43bux438ux437ux430ux446ux438ux438}{%
\subsection{17.
Специализации}\label{ux441ux43fux435ux446ux438ux430ux43bux438ux437ux430ux446ux438ux438}}

\begin{itemize}
\tightlist
\item
  Полные и частичные специализации шаблона класса: синтаксис,
  независимость специализаций.
\item
  Использование для метапрограммирования: \texttt{is\_void},
  \texttt{is\_reference}, \texttt{is\_same}, \texttt{is\_vector},
  \texttt{conditional}.
\item
  Полные специализации функций.

  \begin{itemize}
  \tightlist
  \item
    Ограничения по сравнению со полными специализациями шаблонов класса.
  \item
    Влияение на автовывод типов.
  \item
    Отличия от перегрузки.
  \end{itemize}
\item
  Как использовать \texttt{std::swap}, чтобы работали сторонние
  контейнеры.

  \begin{itemize}
  \tightlist
  \item
    Запрет на добавление перегрузок в \texttt{namespace\ std} и
    необходимость частичной специализации.
  \item
    Костыль через \texttt{using\ std::swap;} и ADL (Argument-Dependent
    Lookup).
  \item
    Не было: детальных правил ADL.
  \end{itemize}
\end{itemize}

\hypertarget{ux448ux430ux431ux43bux43eux43dux43dux44bux435-ux434ux440ux443ux437ux44cux44f}{%
\subsection{18. Шаблонные
друзья}\label{ux448ux430ux431ux43bux43eux43dux43dux44bux435-ux434ux440ux443ux437ux44cux44f}}

\begin{itemize}
\tightlist
\item
  Про всех рассказывать и показать примеры: когда работает, когда нет, к
  чему у кого есть доступ.

  \begin{itemize}
  \tightlist
  \item
    Будьте осторожны с багами GCC и Clang при демонстрации.
  \end{itemize}
\item
  Шаблонные друзья нешаблонных классов:

  \begin{itemize}
  \tightlist
  \item
    Класс-друг: общий случай, полные специализации.
  \item
    Функция-друг: общий случай, полные специализации.
  \end{itemize}
\item
  Нешаблонные друзья шаблонных классов:

  \begin{itemize}
  \tightlist
  \item
    Класс-друг.
  \item
    Функция-друг, реализация внутри и снаружи класса, с зависимостью от
    параметров шаблона и без.
  \end{itemize}
\item
  Шаблонные друзья шаблонных классов:

  \begin{itemize}
  \tightlist
  \item
    Класс-друг: общий случай, полные специализации.
  \item
    Функция-друг: общий случай, полные специализации, реализация внутри
    и снаружи класса, с зависимостью от параметров шаблона и без.
  \end{itemize}
\item
  Стандартные проблемы и решение:

  \begin{itemize}
  \tightlist
  \item
    Multiple definition при определении шаблонной функции-друга внутри
    шаблонного класса, причём функция не зависит от параметров класса.
  \item
    Пример реализации
    \texttt{Ratio\textless{}int\textgreater{}::operator+=(Ratio\textless{}int\textgreater{}\&)}
    (увеличение рациональной дроби с числителем и знаменателем типа
    \texttt{int}) внутри класса и вне класса, отличия.
  \end{itemize}
\end{itemize}

\hypertarget{ux444ux443ux43dux43aux442ux43eux440ux44b-ux438-ux43bux44fux43cux431ux434ux44b}{%
\subsection{19. Функторы и
лямбды}\label{ux444ux443ux43dux43aux442ux43eux440ux44b-ux438-ux43bux44fux43cux431ux434ux44b}}

\begin{itemize}
\tightlist
\item
  Реализация своих функторов.

  \begin{itemize}
  \tightlist
  \item
    Перегрузка \texttt{operator()}, когда нужен const qualifier.
  \item
    Как использовать с \texttt{std::sort}, \texttt{std::set}, в том
    числе функтор без конструктора по умолчанию.
  \item
    Использование указателя на функцию как функтор.
  \item
    Конвенция стандартной библиотеки C++ про отсутствие состояния у
    функторов, \texttt{std::ref}.
  \end{itemize}
\item
  Использование функторов.

  \begin{itemize}
  \tightlist
  \item
    Передача в качестве аргумента функции.
  \item
    Сохранение в поле класса.
  \end{itemize}
\item
  Лямбда-функции (C++11):

  \begin{itemize}
  \tightlist
  \item
    Синтаксис и expression для создания, во что превращается лямбда.
  \item
    Возвращаемый тип: неявный вывод, явное указание.
  \item
    Независимость типов у разных лямбда-функций, почему нельзя запихнуть
    лямбду в \texttt{set}.
  \item
    Неявное преобразование лямбда-функции без захватов в указатель на
    функцию.
  \item
    Захваты: отсутствие, по значению, по ссылке, всех по значению, всех
    по ссылке, \texttt{*this} (C++17), с инициализацией (C++14).
  \item
    Ключевое слово \texttt{mutable}.
  \item
    Шаблонные лямбды.
  \end{itemize}
\end{itemize}

\hypertarget{ux43fux440ux435ux43fux440ux43eux446ux435ux441ux441ux43eux440}{%
\subsection{20.
Препроцессор}\label{ux43fux440ux435ux43fux440ux43eux446ux435ux441ux441ux43eux440}}

\begin{itemize}
\tightlist
\item
  Как пользоваться \texttt{\#ifdef\ DEBUG}, \texttt{\#define} и ключом
  \texttt{-DDEBUG} (в случае GCC/Clang).
\item
  Что делает \texttt{\#include}, в том числе
  \texttt{\#include\ \textless{}iostream\textgreater{}} и
  \texttt{\#include\ \textless{}iosfwd\textgreater{}}.
\item
  Проблемы с \texttt{assert(v\ ==\ std::vector\{1,\ 2,\ 3\})} и как их
  решать.
\item
  Проблемы с \texttt{operator,} и вызовом макросов: как добиться, чтобы
  \texttt{assert(true),\ assert(false);} работало.
\item
  Как использовать \texttt{\#macro\_arg}, \texttt{\_\_FILE\_\_},
  \texttt{\_\_LINE\_\_} для создания своего макроса \texttt{CHECK} в
  тестовом фреймворке.
\item
  Возможность писать в макросах лишь куски корректного кода.

  \begin{itemize}
  \tightlist
  \item
    Общая идея создания фреймворка для автотестов с авторегистрацией
    тестов: \texttt{TEST\_CASE("hi")\ \{\ CHECK(1\ ==\ 2);\ \}}.
  \item
    Не было: точный код, макросная магия для генерации уникальных имён
    тестов, склейка токенов через \texttt{\#\#}.
  \end{itemize}
\end{itemize}

\hypertarget{ux43fux440ux43eux433ux440ux430ux43cux43cux44b-ux438ux437-ux43dux435ux441ux43aux43eux43bux44cux43aux438ux445-ux444ux430ux439ux43bux43eux432}{%
\subsection{21. Программы из нескольких
файлов}\label{ux43fux440ux43eux433ux440ux430ux43cux43cux44b-ux438ux437-ux43dux435ux441ux43aux43eux43bux44cux43aux438ux445-ux444ux430ux439ux43bux43eux432}}

\begin{itemize}
\tightlist
\item
  Мотивация.
\item
  Единицы трансляции и файлы.
\item
  Как из одного файла заиспользовать глобальную/переменную/класс/функцию
  из другого (нешаблонные)?
\item
  External linkage/internal linkage.

  \begin{itemize}
  \tightlist
  \item
    Слово \texttt{static} и anonymous namespace, где применять.
  \end{itemize}
\item
  Формулировка One Definition Rule, пример ошибок линковщика: multiple
  definition, undefined reference.
\item
  Требования к совпадению определений классов.
\item
  Типичный заголовочный файл.

  \begin{itemize}
  \tightlist
  \item
    Конвенция именования заголовочных файлов.
  \item
    Include guards: зачем, как правильно, осторожно с \texttt{\_}.
  \item
    Опастность неявного включения, концепция include what you use,
    примеры из стандартной библиотеки вашего компилятора.
  \item
    Запрет на реализацию функций.
  \end{itemize}
\item
  Взаимная рекурсия между заголовками и forward header.
\item
  Что обычно (не) пишут в своих заголовочных файлах (в том числе
  forward); \texttt{using\ namespace\ std;}.
\item
  Где объявляются/определяются шаблонные функции/классы/константы.
\end{itemize}

\hypertarget{one-definition-rule}{%
\subsection{22. One Definition Rule}\label{one-definition-rule}}

\begin{itemize}
\tightlist
\item
  One Definition Rule (ODR).

  \begin{itemize}
  \tightlist
  \item
    Как можно нарушить и получить IFNDR (Ill-Formed, No Diagnostic
    Required) и ошибку компиляции.
  \item
    Как можно нарушить и получить IFNDR, но не ошибку компиляции: для
    переменной, для функции, для класса.
  \end{itemize}
\item
  Ситуации, где нельзя гарантировать единственное определение (шаблоны,
  inline-функции, пример из фреймворка для автотестов).
\item
  Использование \texttt{inline}-переменных/функций/методов для обхода
  ODR.

  \begin{itemize}
  \tightlist
  \item
    Требования к нескольким определениям.
  \end{itemize}
\item
  Отличия \texttt{inline} от \texttt{static}/anonymous namespace.
\end{itemize}

\hypertarget{static-initialization-order-fiasco}{%
\subsection{23. Static initialization order
fiasco}\label{static-initialization-order-fiasco}}

\begin{itemize}
\tightlist
\item
  Глобального состояние программы: когда можно избавиться, когда
  необходимо.
\item
  Создание и уничтожение объектов со статическим временем жизни.

  \begin{itemize}
  \tightlist
  \item
    У кого статическое время жизни? В том числе у некоторых локальных
    переменных.
  \item
    Гарантии про порядок создания и уничтожения объектов.
  \end{itemize}
\item
  Пример static initialization order fiasco.

  \begin{itemize}
  \tightlist
  \item
    Когда существует некорректный порядок инициализации.
  \item
    Когда не существует корректного порядка инициализации.
  \item
    Когда происходит UB (выглядящий как утечка памяти), при этом в
    программе используется только \texttt{std::string}.
  \end{itemize}
\item
  Решение: идиома construct on first use.

  \begin{itemize}
  \tightlist
  \item
    Отличия решения с автоматическим временем жизни и с динамическим.
  \end{itemize}
\end{itemize}
