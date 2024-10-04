# Встроенные типы данных, представление чисел в памяти, строки
1. Что такое идентификаторы?

# Преобразования типов (явные и неявные)
# Структуры и объединения
1. Что такое объединение (union)?
2. Что такое структура?
   
# Указатели
1. Что такое указатель?
2. Можно ли удалять нулевой указатель?
3. Можно ли удалять указатель дважды?
4. Что значит указатель стрелочка?
   
# Массивы
1. Что такое массив?
   
# Устройство памяти, сегменты
1. Что такое статическая память?
2. Что такое куча?
3. Что такое стековая память?
4. На какие проблемы может указывать Segmentation Fault?
   
# Стек вызова функций

# Ссылки
1. Какие характеристики у lvalue ссылок?
   
# Перегрузка функций
1. Что такое аргументы по умолчанию?
   
# namespace
1. Что такое namespace? Зачем оно нужно?
2. Что такое unnamed namespace?
3. Что такое namespace alias?
   
# Компиляция, этапы, ошибки компиляции
1. Почему программы состоят из отдельных файлов? Какие есть файлы для кода в C++?
2. Три основных этапа трансляции
3. Что такое declaration и definition?
4. Что должно содержаться в заголовочном файле?
5. Характеристики препроцессора
6. Что такое макрос?
7. Что такое стражи?
8. Что такое pragma pack?
9. Характеристики компиляции
10. Характеристики линковки

# ООП (абстракция, инкапсуляция, наследование, полиморфизм)
1. Определение абстракции
2. Определение инкапсуляции
3. Определение инварианта
4. Что такое константаный метод?
5. Что такое правило 3? Почему оно такое?
6. Что такое правило 5? Почему оно такое?
7. Что такое правило 0? Почему оно такое?
8. Определение полиморфизма
9. Что такое проблема ромба?
10. Что такое виртуальное наследование? Как работает таблица виртуальных функций?
11. Виртуальные функции значат, что есть динамический полиморфизм?
12. Зачем нужно ключевое слово override?
13. В какой памяти обычно лежит vtable?
14. Что содержится в vtable?
15. Зачем нужен виртуальный деструктор?
16. Что такое virtual friend function idiom?
17. Что значит friend у оператора?
18. Что делает protected?
19. Что такое type erasure idiom?

# Классы. Специальные методы
   
# Перегрузка операторов

# Шаблоны функций,классов. Частичная и полная специализация
1. Что такое инстанциация шаблона?
2. Какие есть два самых популярных умных указателя? Чем они отличаются?
3. Устройство умного указателя

# STL. Контейнеры, алгоритмы, Функциональные объекты, адаптеры. итераторы. аллокаторы

# Исключения
1. В чём заключается идиома RAII?
2. Перечислить 4 типа гарантий и пример кода
3. Что будет, если в деструкторе выдетит исключение? Как избежать этой проблемы?
4. Какие бывают ошибки?
5. Что такое assert? Когда он применим?
6. Чем assert отличается от static_assert?
7. В чём сходство и отличие std::abort и std::terminate?
8. Что такое errno?
9. Что такое throw?
10. Чем throw отличается от assert?
11. Что такое std::runntime_error?
12. Что такое what()?
13. Что такое try-catch? В чём его преимущества?
14. В чём недостаток try-catch?
15. Объяснить механизм stack unwinding в контексте обработки исключений
16. Что такое Automatic Storage Duration?
17. Какие ещё есть типы хранения?
18. Будут ли уничтожены автоматически объекты на куче при stack unwinding?
19. Что такое noexcept?
20. Какие правила применимы к std::exception?
21. Почему исключение принято кидать по значению, а ловить по ссылке?
22. Что такое std::expected?
23. В чём разница между исключениями, кодами возврата и std::expected?
24. Что такое std::unexpected<E>?
25. Что такое std::bad_expected_access?

# Преобразования, CRTP
1. Что такое const_cast?
2. Что такое static_cast?
3. Что такое dynamic_cast?
4. Что такое RTTI?
5. Что такое reinterpret_cast?
6. Что такое C-style cast?
7. Что такое CRTP?
8. Как сделать метод шаблонного классом с аргументом T, который будет возвращать новый объект типа T, копируя данные из текущего объекта, предполагая, что это базовый класс в CRTP?

# Move-семантика, value-categories
1. Какие есть типы value?
2. Что такое объект и lvalue по Кернигану-Ритчи в языке Си?
3. Что такое rvalue?
4. Какой тип значения имеет правый операнд при присваивании?
5. В чём отличаются lvalue и rvalue?
6. Что такое glvalue?
7. Что такое prvalue?
8. Что такое xvalue?
9. glvalue - это любое значение?
10. Из каких value состоит множество rvalue?
11. Можно ли сделать умный указатель от xvalue?

# Lambda - expression

# Variadic templates
1. Написать шаблонную функцию с шаблонным аргументом T, которая имеет аргумент T и возвращает это значение в виде строки, используя строковый поток
2. Написать variadic template функцию, которая будет с помощью предыдущей функции преобразовывать несколько значений любого типа в строки и вернуть вектор строк. Реализация через рекурсию. Как это можно было бы решить в одну строчку?
3. Что такое parameter pack?
4. Написать функцию, которая принимает произвольное число элементов произвольного типа и выводит их (гарантируется, что у них перегружен оператор вывода)
5. Как узнать число элементов в пакете аргументов?
6. Что такое if constexpr?
7. Что такое fold expressions?
8. Арифметические операции с помощью fold expressions. Какой правильный порядок у операндов?
9. Привести пример кода с std::tuple, демонстрирующего его функциональность
10. Реализация NaiveTuple из лекции
    
# Metaprogramming, type traits


Вот бы было ЕГЭ по борьба
