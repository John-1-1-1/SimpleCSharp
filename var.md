
# Переменные в C#

**Переменная** - именованная область памяти. 

```csharp
Тип имя_переменной;
```

### Имя переменной 

- **начинается** с буквы;
- может состоять из букв, цифр и символа "_";
- не должно являться ключевым словом.

| Тип     | Размер  | Диапазон                                                   |
|---------|---------|------------------------------------------------------------|
| bool    | 1 байт  | true / false                                               |
| byte    | 1 байт  | от 0 до 255                                                |
| int     | 4 байта | от -2147483648 до 2147483647                               |
| long    | 8 байт  | от –9 223 372 036 854 775 808 до 9 223 372 036 854 775 807 |
| float   | 4 байта | от -3.4*1038 до 3.4*1038                                   |
| double  | 8 байт  | от ±5.0*10-324 до ±1.7*10308                               |
| decimal | 16 байт | от ±1.0*10-28 до ±7.9228*1028 (28 знаков после запятой)    |

**String** - хранит внабор символов, подстраивается под данные

| Операция | Описание           | 
|----------|--------------------|
| +        | сложение           |
| -        | вычитание          |
| /        | деление            |
| *        | умножение          |
| %        | остаток от деления |

##### Пример:

```csharp
int a = 5; 
int b = 2;

int c = a % b; // c будет равен 1 
```

### Переполнение переменных

У каждой переменной есть ограничение, если попробовать превысить лимит, 
программа продолжит работать, однако результат работы будет некорректным.

##### Пример:

Для примера будет использоваться переменная типа byte, которая 
может хранить значения от 0 до 255 (1 байт).

```csharp
byte a = 255;
Console.WriteLine(a); // 255
a = (byte)(a + 1);
Console.WriteLine(a); // 0
```

Представим переменную a в двоичнов виде:

| 7 | 6 | 5 | 4 | 3 | 2 | 1 | 0 | 
|---|---|---|---|---|---|---|---|
| 1 | 1 | 1 | 1 | 1 | 1 | 1 | 1 |

Если прибавить к двоичной записи единицу, 
то программа получит девятиразрядное число.
Однако ячейки для 9 разряда нет, а остальные 
8 рязрядов заполнены нулями!

| 7 | 6 | 5 | 4 | 3 | 2 | 1 | 0 | 
|---|---|---|---|---|---|---|---|
| 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |


