
# [док](https://docs.google.com/document/u/0/d/1lFzPt4vnC81c8UabRYkME_Xis2m-acU_esWA-DlN5Mw/mobilebasic)

## 1. Ссылки. Разница между ссылкой и указателем. Зачем в С++ были добавлены ссылки.

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

#### Модификаторы доступа

Уровень доступности позволяет регулировать доступ к данным и методам класса. Одни элементы класса могут быть общедоступны, другие — скрыты. Сокрытие данных и методов в классе называется инкапсуляцией.

1) Private
- элемент недоступен любым экземплярам методов других классов или методов, которые не являются «дружественными» к классу
- элемент недоступен из унаследованных классов
- элемент доступен из методов, которые реализованы в классе
- элемент доступен из дружественных функций
- элемент доступен из методов дружественных классов

2) Public
- элемент доступен всем методам в программе (Исключение составляет случай, когда класс унаследован как private)

3) Protected
- элемент класса недоступен из любого внешнего метода, если этот метод не является дружественным; 
- элемент класса доступен из внутренних методов класса. Здесь следует заметить, что protected-элемент класса также доступен из экземпляра класса, если этот экземпляр объявляется во внутреннем методе класса;
- элемент класса доступен из дружественных функций класса
- элемент класса доступен из методов дружественного класса
- элемент класса доступен из методов унаследованного класса
- элемент класса недоступен из экземпляров унаследованного класса. Это правило не касается «дружественных» методов и методов «дружественных» классов.

#### Наследование 
Наследование представляет один из ключевых аспектов объектно-ориентированного программирования, который позволяет наследовать функциональность одного класса или базового класса (base class) в другом - производном классе (derived class).


Конструкторы при наследовании не наследуются. И если базовый класс содержит только конструкторы с параметрами, то производный класс должен вызывать в своем конструкторе один из конструкторов базового класса

Проблемы множественного наседования:
- Одинаковые поля или методы в родительских классах
 Для решения нужно прямо указывать к какому члену или методу мы обращаемся 
 
 ![image](https://user-images.githubusercontent.com/56086653/173465973-ab73fd70-a3f5-441d-9008-1a6ca50531a5.png)
 
 - Ромбовидное наследование 

![image](https://user-images.githubusercontent.com/56086653/173466097-60b42f47-d87c-4120-8b6a-557dbb345ac6.png)

## 4. ООП. Классы. Инициализация и уничтожение. Виды конструкторов Виртуальные методы. Таблица виртуальных функций. Виртуальные деструкторы.

Конструктор — функция, предназначенная для инициализации объектов класса. Конструктор всегда имеет то же имя, что и сам класс и никогда не имеет возвращаемого значения. Когда класс имеет конструктор, все объекты этого класса будут проинициализированы. Их может быть много разных

Виды конструкторов
- По умолчанию (не имеет параментров)
- С парамерами
- Конструктор копирования


Деструктор обеспечивает соответствующую очистку объектов указанного типа. Многие классы используют динамическую память, которая выделяется конструктором, а освобождается деструктором. Деструктор выполняет освобождение использованных объектом ресурсов и удаление нестатических переменных объекта. Каждый класс может иметь только один деструктор.

Деструктор автоматически вызывается, когда удаляется объект. Удаление объекта происходит в следующих случаях:
- выход из области видимости 
- когда удаляется контейнер (например, массив), который содержит объекты
- динамически созданные объекты удаляются при применении к указателю на объект оператора delete

#### Виртуальные методы

Виртуальные функции — специальный вид функций-членов класса. Виртуальная функция отличается от обычной функции тем, что для обычной функции связывание вызова функции с ее определением осуществляется на этапе компиляции. Для виртуальных функций это происходит во время выполнения программы.

Чистая виртуальная функция — это метод класса, тело которого не определено.

![image](https://user-images.githubusercontent.com/56086653/173471788-1cc0e63d-b934-4fb3-a93b-17bfe123d570.png)

![image](https://user-images.githubusercontent.com/56086653/173584164-ef822d54-34f4-427c-8167-701c96dba469.png)

![image](https://user-images.githubusercontent.com/56086653/173585532-ffa754bb-b5a6-410f-bee7-ada14c9d698b.png)

![image](https://user-images.githubusercontent.com/56086653/173585965-7f40141f-5542-44aa-b128-5856f535f60f.png)

## 5. ООП. Операторы. Перегрузка операторов.

Перегружать можно только операции над пользовательскими типами!

![image](https://user-images.githubusercontent.com/56086653/173588899-df4a2288-c88e-4319-bbbb-ae04b520fb82.png)


![image](https://user-images.githubusercontent.com/56086653/173587172-7801b328-74a7-48f3-8b89-62217acc5e2b.png)

![image](https://user-images.githubusercontent.com/56086653/173587274-d0ea6421-5f17-49f5-b653-ee93ac0f811c.png)

![image](https://user-images.githubusercontent.com/56086653/173588672-0dc34c32-7745-43d3-aaf3-9126759b4dfd.png)

![image](https://user-images.githubusercontent.com/56086653/173589111-0311a0c8-ea75-4edf-a589-4335076ba361.png)

![image](https://user-images.githubusercontent.com/56086653/173589142-8b2bdc8a-93e3-413e-9c44-784b9ea137bc.png)

![image](https://user-images.githubusercontent.com/56086653/173666141-9cc69d35-fbb6-42f9-96c9-a351fa4cb34e.png)



## 6. Исключения. Обработка ошибок в Си. Assert. Исключения.Преимущества и недостатки исключений.

![image](https://user-images.githubusercontent.com/56086653/173592714-47b7e67b-1b10-430a-842a-154b5048df2f.png)

---

![image](https://user-images.githubusercontent.com/56086653/173592775-d34a46f2-b067-4f30-bd7a-f4efe9758cb6.png)

---

![image](https://user-images.githubusercontent.com/56086653/173603053-c92d0379-512b-46a0-b280-8c3fd843e7c0.png)

---

![image](https://user-images.githubusercontent.com/56086653/173603653-95a3c45f-174a-4c50-a456-18ae0639c4d0.png)

---

![image](https://user-images.githubusercontent.com/56086653/173603767-1613ecdf-27e3-4968-8f7e-dedcafea31e6.png)

![image](https://user-images.githubusercontent.com/56086653/173603816-5025b91d-973c-4d67-8f0a-8479da455e29.png)

![image](https://user-images.githubusercontent.com/56086653/173630596-1666f10b-801f-4400-a71c-4afd10f023e7.png)

![image](https://user-images.githubusercontent.com/56086653/173630640-28d4c062-658b-43b9-8db5-2248ed2de1f3.png)

ВАЖНО !

![image](https://user-images.githubusercontent.com/56086653/173631138-f1b1f877-c870-4834-830b-4ffd69ad8808.png)


Перехватываем оверфлоу 

![image](https://user-images.githubusercontent.com/56086653/173630539-cbc77b36-b8ec-46be-a29f-76d26ab82f02.png)


## 7. Шаблоны. Шаблоны функций, классов.

![image](https://user-images.githubusercontent.com/56086653/173663542-1bfddffa-cdd8-4cc7-a721-b2f28901ddfd.png)


![image](https://user-images.githubusercontent.com/56086653/173670828-b587a901-e17a-48b9-a80b-c27f807d9e7f.png)

![image](https://user-images.githubusercontent.com/56086653/173670857-82d96596-c0d4-4c3b-a132-13fe7189e38a.png)

![image](https://user-images.githubusercontent.com/56086653/173670868-419ee83d-157a-45ad-9f40-dea832633eff.png)

![image](https://user-images.githubusercontent.com/56086653/173670890-6d8e65f0-56e9-4112-aa53-87384cb32d57.png)



## 8. Шаблоны. Частичная специализация и полная специализация

```
https://habr.com/ru/post/54762/
```

![image](https://user-images.githubusercontent.com/56086653/173670769-a5cc508b-f787-4dab-89c4-845b3a6bd244.png)

![image](https://user-images.githubusercontent.com/56086653/173671121-ab289703-4c70-43d6-ae85-60f38e2e93fb.png)

![image](https://user-images.githubusercontent.com/56086653/173673459-2e30bef3-30fe-4f48-877f-f3f0682a7d6f.png)




## 9. Variadic template

```
https://teccxx.neocities.org/mx1/variadic_templates.html

```
Variadic template - это шаблон с переменным количеством аргументов


![image](https://user-images.githubusercontent.com/56086653/173674064-c4504bac-1cbe-4ce4-a8e0-a923209a09de.png)


## 10.Преобразования типов. Явные и неявные. С-cast, static_cast, dynamic_cast, const_cast, reinterpret_cast. CRTP

![image](https://user-images.githubusercontent.com/56086653/173632967-e94786e8-3225-436d-bec7-69925be5815d.png)

![image](https://user-images.githubusercontent.com/56086653/173635023-e5529a41-4e90-43fa-9325-92e50e0c56f0.png)

![image](https://user-images.githubusercontent.com/56086653/173635080-5d6e417f-2c2c-4a82-9981-696f03f5b07e.png)

#### ИМБА! - [СТАТЬЯ ПРО КАСТЫ](https://habr.com/ru/post/266747/)
---

CRTP - позже



## 11. Стандартная библиотека. Итераторы. Алгоритмы. Основные классы алгоритмов.

## 12.Стандартная библиотека. Контейнеры. Последовательные контейнеры.

## 13.Стандартная библиотека. Контейнеры. Ассоциативные контейнеры.

## 14.Стандартная библиотека. Адаптеры.

## 15.Умные указатели. auto_ptr, unique_ptr, shared_ptr, weak_ptr. Устройство, преимущества и недостатки.
