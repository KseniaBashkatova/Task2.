# Практическая работа №2: Операторы языка C#



> ### Программа 1. 



```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Задача: Вычислите результат выражения int x = 17 / 5; int y = 17 % 5;. Ответ: x = 3, y = 2.
            int x = 17 / 5;
            int y = 17 % 5;
            Console.WriteLine("x = " + x);
            Console.WriteLine("y = " + y);

        }
    }
 }
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.1.1.png">
</picture>


> ### Программа 2. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Задача 2: Каково значение res после выполнения int a = 5; int res = ++a * 2;? Ответ: res = 12 (префиксный инкремент увеличивает a до 6, затем умножение).

            int a = 5;
            int res = ++a * 2;

            Console.WriteLine($"res = {res}");

        }
    }
 }

```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.1.2.png">
</picture>

> ### Программа 3. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            //Задача 3: Каково значение res после выполнения int a = 5; int res = a++ * 2;? Ответ: res = 10(постфиксный инкремент использует исходное значение 5, затем a становится 6).

            int a = 5;
            int res = a++ * 2;

            Console.Write($"res = {res}");
        }
    }
 }

```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.1.3.png">
</picture>

> ### Программа 4. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Задача 4: Чему равен результат 7 / 2 и 7.0 / 2? Ответ: 3 (целочисленное деление) и 3.5 (деление с плавающей точкой).
            int C = 7 / 2;
            decimal P = 7.0m / 2;

            Console.WriteLine($"Решение целочисленного делеия: {C}");
            Console.WriteLine($"Решение целочисленного делеия: {P}");
        }
    }
 }
 
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.1.4.png">
</picture>

> ### Программа 5. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Задача 5: Каков результат выражения -15 % 4 в C#? Ответ: -3 (знак остатка совпадает со знаком делимого).

            int q = -15 % 4;

            Console.WriteLine($"Результат: {q}");

        }
    }
 }
```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.1.5.png">
</picture>

---

> ### Программа 6. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Задача 6: Что выведет выражение int x = 10; x = x++ + ++x;? Ответ: 22(первое слагаемое 10, после него x становится 11, префиксный инкремент делает x = 12, итог 10 + 12 = 22).

            int x = 10;
            x = x++ + ++x;

        }
    }
 }
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.1.6.png">
</picture>

> ### Программа 7.

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program7
{
    internal class Program
    {
        static void Main(string[] args)
        {
         //Запросите три вещественных числа. Вычислите и выведите их среднее арифметическое с округлением до двух знаков после запятой.
         Console.Write("Введите первое число: ");
         double a = double.Parse(Console.ReadLine());
         Console.Write("Введите второе число: ");
         double b = double.Parse(Console.ReadLine());
         Console.Write("Введите третье число: ");
         double c = double.Parse(Console.ReadLine());
         double average = (a + b + c) / 3.0;
         Console.WriteLine($"Среднее арифметическое: {average:F2}");
        }
    }
}

```

> ### Программа 8. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program8
{
    internal class Program
    {
        static void Main(string[] args)
        {
         //Считайте расстояние в метрах и время в секундах. Рассчитайте и выведите скорость движения в км/ч.
         Console.Write("Введите расстояние в метрах: ");
         double meters = double.Parse(Console.ReadLine());

         Console.Write("Введите время в секундах: ");
         double seconds = double.Parse(Console.ReadLine());

         double speedKmH = (meters / 1000) / (seconds / 3600);
         Console.WriteLine($"Скорость: {speedKmH:F2} км/ч");
        }
    }
}

```

> ### Программа 9. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program9
{
    internal class Program
    {
        static void Main(string[] args)
        {
            //Запросите стоимость товара и процент скидки (от 0 до 100). Вычислите сумму скидки и итоговую цену товара с использованием типа decimal.
            Console.Write("Введите стоимость товара: ");
            decimal price = decimal.Parse(Console.ReadLine());
            Console.Write("Введите процент скидки от 0 до 100: ");
            decimal discountPercent = decimal.Parse(Console.ReadLine());
            decimal discountAmount = price * discountPercent / 100m;
            decimal finalPrice = price - discountAmount;
            Console.WriteLine($"Сумма скидки: {discountAmount:F2}");
            Console.WriteLine($"Итоговая цена: {finalPrice:F2}");
        }
    }
}

```

> ### Программа 10. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program10
{
    internal class Program
    {
        static void Main(string[] args)
        {
            //Пользователь вводит баланс мобильного телефона и стоимость одной минуты разговора. Вычислите, сколько полных минут разговора доступно абоненту.
            Console.Write("Введите баланс мобильного телефона: ");
            decimal balance = decimal.Parse(Console.ReadLine());
            Console.Write("Введите стоимость одной минуты разговора: ");
            decimal costPerMinute = decimal.Parse(Console.ReadLine());
            int fullMinutes = (int)Math.Floor(balance / costPerMinute);
            Console.WriteLine($"Доступно полных минут разговора: {fullMinutes}");
        }
    }
}

```
> ### Программа 11. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program11
{
    internal class Program
    {
        static void Main(string[] args)
        {

        }
    }
}

```
> ### Программа 12. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program12
{
    internal class Program
    {
        static void Main(string[] args)
        {

        }
    }
}

```
> ### Программа 13. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program13
{
    internal class Program
    {
        static void Main(string[] args)
        {

        }
    }
}

```
> ### Программа 14. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program14
{
    internal class Program
    {
        static void Main(string[] args)
        {

        }
    }
}

```
> ### Программа 15. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program15
{
    internal class Program
    {
        static void Main(string[] args)
        {

        }
    }
}

```
> ### Программа 16. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program16
{
    internal class Program
    {
        static void Main(string[] args)
        {

        }
    }
}

```
> ### Программа 17. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program17
{
    internal class Program
    {
        static void Main(string[] args)
        {

        }
    }
}

```
> ### Программа 18. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program18
{
    internal class Program
    {
        static void Main(string[] args)
        {

        }
    }
}

```
> ### Программа 19. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program19
{
    internal class Program
    {
        static void Main(string[] args)
        {

        }
    }
}

```
> ### Программа 20. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program20
{
    internal class Program
    {
        static void Main(string[] args)
        {

        }
    }
}

```
🧑‍💻 Ссылка на практическую работу №2 и преподавателя [github](https://github.com/U5er01Task/Fundamentals-of-Algorithmization-and-Programming-2026/tree/main) - [Преподаватель](https://github.com/U5er01Task)

---
