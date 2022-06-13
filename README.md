
# [док](https://docs.google.com/document/u/0/d/1lFzPt4vnC81c8UabRYkME_Xis2m-acU_esWA-DlN5Mw/mobilebasic)

## 1. Ссылки. Разница между ссылкой и указателем. Зачем в С++ были добавлены ссылки.
```

```

![image](https://user-images.githubusercontent.com/56086653/172843208-904f8af5-de42-44ff-8508-9352fa44e7b9.png)

![image](https://user-images.githubusercontent.com/56086653/172843341-db44d28d-21a5-4c67-99c4-3d41d18656d9.png)

![image](https://user-images.githubusercontent.com/56086653/172843395-cfbcebe7-8eea-44b8-82d7-e7855a06810b.png)

![image](https://user-images.githubusercontent.com/56086653/172843528-1a9b6e0b-f24b-4cb7-b196-0922de2b2937.png)

![image](https://user-images.githubusercontent.com/56086653/173192302-c2d5e7b9-6f1f-4f1d-90a2-39445656c0e7.png)

![image](https://user-images.githubusercontent.com/56086653/173193041-f5d7f5ac-6356-43d3-aa2b-9970039bb085.png)

![image](https://user-images.githubusercontent.com/56086653/173193126-290d6e72-af03-4dc8-abf1-c338ca4081c7.png)

Указатели и ссылки — это два синтаксически разных способа в C++ выразить понятие адреса

```
https://habr.com/ru/post/251091/


```

--- 


## 2. ООП. Базовые принципы. Абстракция, инкапсуляция, наследование полиморфизм. SOLID.

Определение гласит, что «Объектно-ориентированное программирование – это парадигма программирования,
в которой основной концепцией является понятие объекта, который отождествляется с предметной областью.»

Таким образом, система представляется в виде набора объектов предметной области, которые взаимодействуют между собой некоторым образом. 
Каждый объект обладает тремя cоставляющими: идентичность (identity), состояние (state) и поведение (behaviour).


Состояние объекта — это набор всех его полей и их значений.


Поведение объекта — это набор всех методов класса объекта.

Идентичность объекта — это то, что отличает один объект класса от другого объекта класса

![image](https://user-images.githubusercontent.com/56086653/172845737-43ef1873-653f-48e0-a29a-cfc6e764c466.png)

![image](https://user-images.githubusercontent.com/56086653/172845809-bd03d37d-811c-4de1-8955-f0b1abfb40ca.png)

![image](https://user-images.githubusercontent.com/56086653/172847679-07b76cb0-71ef-401b-a3e7-f895a59d3005.png)

### Solid

### [принцип единственной ответственности](https://web-creator.ru/articles/solid_the_single_responsibility_principle)

### [принцип открытости-закрытости](https://web-creator.ru/articles/solid_the_open_closed_principle)

### [принцип подстановки Барбары Лисков](https://web-creator.ru/articles/solid_the_liskov_substitution_principle)

### [принцип разделения интерфейса](https://web-creator.ru/articles/solid_the_interface_segregation_principle)

### [принцип инверсии зависимостей](https://web-creator.ru/articles/solid_the_dependency_inversion_principle)


---


## 3. ООП. Классы. Устройство в памяти. Инкапсуляция. Модификаторы доступа. Наследование. Множественное наследование. Проблемы множественного наследование.

### Как выделяется память?

![image](https://user-images.githubusercontent.com/56086653/173194352-b4f4134e-ca97-4639-aaa0-e555aef4517f.png)

![image](https://user-images.githubusercontent.com/56086653/173194463-80fd05e2-ee2d-4dca-be48-fbe5dca0d69d.png)

выравнивать стоит по размеру наибольшего типа в классе!

![image](https://user-images.githubusercontent.com/56086653/173461319-7f824eba-cdb6-40c3-bbc7-82ea6e285a52.png)

![image](https://user-images.githubusercontent.com/56086653/173462458-101559ba-541e-4c75-83c8-389de6a51d20.png)

![image](https://user-images.githubusercontent.com/56086653/173463478-6a374bdf-481b-4633-8fd2-37bc81ca009c.png)

![image](https://user-images.githubusercontent.com/56086653/173463599-96b6e769-f256-456d-adde-7f2e1a0b504e.png)

![image](https://user-images.githubusercontent.com/56086653/173464014-29cd1ec6-c03e-4784-b500-9fd04a907e76.png)

![image](https://user-images.githubusercontent.com/56086653/173464075-a9fa76da-394e-490e-b301-e219b327736b.png)

![image](https://user-images.githubusercontent.com/56086653/173464443-fe92e377-2808-4c7c-bb1e-b8d7a9268461.png)

```
http://scrutator.me/post/2014/06/02/objects_memory_layout_p2.aspx
```

Класс – это способ описания сущности, определяющий состояние и поведение, зависящее от этого состояния, а также правила для взаимодействия с данной сущностью (контракт).
С точки зрения программирования класс можно рассматривать как набор данных (полей, атрибутов, членов класса) и функций для работы с ними (методов).



## 4. ООП. Классы. Инициализация и уничтожение. Виды конструкторов Виртуальные методы. Таблица виртуальных функций. Виртуальные деструкторы.

## 5. ООП. Операторы. Перегрузка операторов.

## 6. Исключения. Обработка ошибок в Си. Assert. Исключения.Преимущества и недостатки исключений.

## 7. Шаблоны. Шаблоны функций, классов.

## 8. Шаблоны. Частичная специализация и полная специализация

## 9. Variadic template

## 10.Преобразования типов. Явные и неявные. С-cast, static_cast, dynamic_cast, const_cast, reinterpret_cast. CRTP

## 11. Стандартная библиотека. Итераторы. Алгоритмы. Основные классы алгоритмов.

## 12.Стандартная библиотека. Контейнеры. Последовательные контейнеры.

## 13.Стандартная библиотека. Контейнеры. Ассоциативные контейнеры.

## 14.Стандартная библиотека. Адаптеры.

## 15.Умные указатели. auto_ptr, unique_ptr, shared_ptr, weak_ptr. Устройство, преимущества и недостатки.
