# Math

Для выполнения различных математических операций
в библиотеке классов .NET предназначен класс Math. 

### Abs -  модуль

```csharp
double result = Math.Abs(-12.4); // 12.4
```

### Max - вернёт максимальное число

```csharp
double result = Math.Max(1,4); // 4
```

### Min - вернёт минимальное число

```csharp
double result = Math.Min(1,4); // 1
```

### Pow - возведение в степень

```csharp
double result = Math.Pow(3,2); // 9
```

### Round - математическое округление

```csharp
double result1 = Math.Round(20.56); // 21
double result2 = Math.Round(20.46); //20

// второй аргумент указыает на 
// точность математического округления

double result1 = Math.Round(20.567, 2); // 20,57
double result2 = Math.Round(20.463, 1); //20,5
```

### Floor - обрубает дробную часть

```csharp
double result = Math.Floor(2.56); // 2
```
  
###  Sqrt - квадратный корень 

```csharp
double result1 = Math.Sqrt(16); // 4
```