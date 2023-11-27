# Ввод и вывод в консоль

Для работы с сонсолью используется встроенный
класс `Console`.

Для вывода на экран используется две команды:

`Console.WriteLine` - Вывод информации +
переход на следующую строку. 
(Если не хотите чтобы текст слипся)

`Console.Write` - Вывод без перехода на 
новую строку.

##### Пример WriteLine:

```csharp
Console.WriteLine("Hello, World!");
Console.WriteLine("Hello, World!");

//Вывод:
//Hello, World!
//Hello, World!
```

##### Пример Write:

```csharp
Console.Write("Hello, World!");
Console.Write("Hello, World!");

//Вывод:
//Hello, World!Hello, World!
```

Для ввода из консоли используется `Console.ReadLine()`

##### Пример

```csharp
Console.Write("Введите свое имя: ");
string name = Console.ReadLine();
Console.WriteLine($"Привет {name}");
```

#### Важно!

Если программа после выполнение сразу закрывается, 
необходимо добавить `Console.ReadKey()`.

`ReadKey` - ожидает нажатие на любую клавишу.
