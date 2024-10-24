# Указатели
1. Что такое указатель?
2. Можно ли удалять нулевой указатель?
3. Можно ли удалять указатель дважды?
   
# Устройство памяти, сегменты
1. Что такое статическая память?
2. Что такое куча?
3. Что такое стековая память?
   
# Стек вызова функций
1. На какие проблемы может указывать Segmentation Fault?
2. Дана рекурсивная функция вычисления факториала. Найти при каком наибольшем n стек не переполнится. Редактировать можно только тот же main.cpp, без бинпоиска по запускам
```
int factorial(int n) {
   if (n == 0) {
      return 1;
   }
   return n * factorial(n - 1);
}
```

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
1. Формальные определения абстракции, инкапсуляции, полиморфищма
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

# Шаблоны функций,классов. Частичная и полная специализация
1. Что такое инстанциация шаблона?
2. Что такое template argument deduction?
3. Какие есть два самых популярных умных указателя? Чем они отличаются?
4. Характеристики shared_ptr и unique_ptr
5. Устройство умного указателя внутри
6. Tag Dispatch Idiom
7. SFINAE

# STL. Контейнеры, алгоритмы, Функциональные объекты, адаптеры. итераторы. аллокаторы
Кроме аллокаторов всё есть в Страуструпе (в конце каждой главы есть список вопросов для самопроверки)
1. Написать unordered map которая работает в обе стороны + обертка над байтовым буффером

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
26. Перечислить 4 вида гарантий

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
12. Проблема избыточного копирования
14. Copy and swap idiom
15. Swap с помощью std::move
16. В чём отличие между rvalue и универасальными ссылками?
17. Collapsing of references
18. Что такое perfect forwarding?
19. Устройство std::forward
20. Copy elision

# Lambda - expression
Нужно разобраться с классом Functor, есть в Александреску и собственно в лекции

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
11. Реализация is_arithmetical_progression
12. Реализовать шаблон TMaybe<T>, который
- хранит в себе переменную типа T
- умеет каститься к bool (выводит 0, если объект не был инициализирован, иначе 1)
- имеет operator*, который возвращает хранящуюся переменную
- умеет в copy constructor, move constructor
- имеет конструктор от variadic template, чтоб можно было сходу конструировать объект под капотом
  (пусть есть Point { x, y, z }, тогда мы сможем написать так: TMaybe<Point> m{1, 2, 3})
    
# Metaprogramming, type traits
1. Как вычислить факториал на этапе компиляции с помощью шаблонов?
2. Что такое constexpr variable и constexpr function? 
3. Как вычислить факториал на этапе компиляции с помощью constexpr?
4. Что такое метапрограммирование?
5. Что такое метафункция?
6. Написать метафункцию, которая вычисляет сумму произвольного числа элементов
7. Helper variables/types
8. Что такое concepts (C++20)?
9. Ключевое слово requires
10. Concepts для сложения двух аргументов
