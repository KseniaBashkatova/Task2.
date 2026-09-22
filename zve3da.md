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

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Задача 7: Что произойдет при выполнении int max = int.MaxValue; int res = checked(max + 1);? Ответ: Выбросится исключение System.OverflowException.

            int max = int.MaxValue;
            int res = checked(max + 1);

        }
    }
 }

```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.1.7.png">
</picture>

> ### Программа 8. 

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
            // Задача 8: Что произойдет при int max = int.MaxValue; int res = unchecked(max + 1);? Ответ: res = int.MinValue (произойдет переполнение без ошибки).

            int max = int.MaxValue;
            int res = unchecked(max + 1);

            Console.WriteLine($"Вывод {res}");

        }
    }
 }

```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.1.8.png">
</picture>

> ### Программа 9. 

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
            // Задача 9: Чему равен результат деления 1.0 / 0.0 и 0.0 / 0.0 ? Ответ : double.PositiveInfinity(Infinity) и double.NaN.

            double x = 1.0 / 0.0;
            double y = 0.0 / 0.0;

            Console.WriteLine($"X = {x}");
            Console.WriteLine($"Y = {y}");

        }
    }
 }

```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.1.9.png">
</picture>

> ### Программа 10. 

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
            // Задача 10: Вычислите: int a = 8; int b = 3; int c = a - b * 2 + a / b;. Ответ: 8 - 6 + 2 = 4.

            int a = 8;
            int b = 3;
            int c = a - b * 2 + a / b;

            Console.WriteLine($"C = {c}");

        }
    }
 }

```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.1.10.png">
</picture>

> ### Программа 11. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _3._2
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Задача 1: Каков результат 5 > 3 и 5 >= 5? Ответ: true, true.
            bool x = 5 > 3;
            bool y = 5 >= 5;

            Console.WriteLine($"X = {x}");
            Console.WriteLine($"Y = {y}");
        }
    }
}

```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.2.1.png">
</picture>

> ### Программа 12. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _3._2
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Задача 2: Чему равно "hello" == "hello" в C# и почему? Ответ: true, так как для типа string оператор == перегружен для посимвольного сравнения значений.
            bool x = "hello" == "hello";

            Console.WriteLine($"{x}");
        }
    }
}

```


`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.2.2.png">
</picture>

> ### Программа 13. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _3._2
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Задача 3: Чему равно выражение double.NaN == double.NaN? Ответ: false (по стандарту IEEE 754 NaN не равен ничему, даже самому себе).
            bool x = double.NaN == double.NaN;

            Console.WriteLine($"{x}");

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.2.3.png">
</picture>


> ### Программа 14. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _3._2
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Задача 4:  Каков результат выражения object a = new int[] { 1 }; object b = new int[] { 1 }; bool r = a == b;? Ответ: false (сравниваются ссылки на два разных объекта в куче).
            object a = new int[] { 1 };
            object b = new int[] { 1 };

            bool r = a == b;

            Console.WriteLine($"r = {r}");
        }
    }
}

```


`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.2.4.png">
</picture>

> ### Программа 15. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _3._2
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Задача 5: Чему равно 10 != 10.0? Ответ: false (целое число 10 неявно приводится к 10.0, значения равны).

            bool x = 10 != 10.0;

            Console.WriteLine($"x = {x}");
        }
    }
}

```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.2.5.png">
</picture>

> ### Программа 16. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _3._2
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Задача 6: Что вернет null == null? Ответ: true.
            bool x = null == null;

            Console.WriteLine($"x = {x}");
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.2.6.png">
</picture>



> ### Программа 17. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _3._2
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Задача 7:  Каков результат выражения (3 < 5) == (10 >= 20)? Ответ: false (true == false дает false).
            bool x = (3 < 5) == (10 >= 20);

            Console.WriteLine($"x = {x}");
        }
    }
}
```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.2.7.png">
</picture>


> ### Программа 18. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _3._2
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Задача 8: Вычислите bool res = 4 <= 4 && 5 > 2;. Ответ: true.
            bool res = 4 <= 4 && 5 > 2;

            Console.WriteLine($"res = {res}");
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.2.8.png">
</picture>


> ### Программа 19. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _3._2
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Задача 9: Что вернет выражение char c = 'b'; bool res = c > 'a';? Ответ: true (символы сравниваются по их числовым кодам Unicode: 98 > 97).
            char c = 'b';
            bool res = c > 'a';

            Console.WriteLine($"res = {res}");
        }
    }
}


```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.2.9.png">
</picture>

> ### Программа 20. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _3._2
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Задача 10: Сравните результат bool r = -0.0 == 0.0;. Ответ: true (ноль со знаком равен обычному нулю).
            bool r = -0.0 > 0.0;

            Console.WriteLine($"r = {r}");
        }
    }
}


```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.2.10.png">
</picture>

> ### Программа 21. 

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
            // Задача 1: Вычислите: !true || false && true. Ответ: false (приоритет: ! -> && -> ||: false || false дает false).
            bool x = !true || false && true;

            Console.WriteLine($"x = {x}");
        }
    }
}


```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.3.1.png">
</picture>


> ### Программа 22. 

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
            // Задача 2: Будет ли вызван метод Foo() в false && Foo()? Ответ: Нет, благодаря короткому замыканию оператора &&.
            bool x = false && Foo();

            Console.WriteLine($"x = {x}");
        }
    }
}


```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.3.2.png">
</picture>

> ### Программа 23. 

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
            // Задача 3: Будет ли вызван метод Foo() в false & Foo()? Ответ: Да, побитовое/строгое логическое & вычисляет оба операнда.
            int x = false & Foo();

            Console.WriteLine($"x = {x}");
        }
    }
}


```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.3.3.png">
</picture>

> ### Программа 24. 

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
            // Задача 4: Вычислите результат: true ^ false ^ true. Ответ: false (true ^ false = true, затем true ^ true = false).
            bool x = true ^ false ^ true;

            Console.WriteLine($"x = {x}");
        }
    }
}
```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.3.4.png">
</picture>

> ### Программа 25. 

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
            // Задача 5:  Что вернет выражение !(5 > 2 || 3 < 1)? Ответ: false (5 > 2 истинно, внутри скобок true, отрицание дает false).
            bool x = !(5 > 2 || 3 < 1);

            Console.WriteLine($"x = {x}");
        }
    }
}


```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.3.5.png">
</picture>

> ### Программа 26. 

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
            // Задача 6: Дано: bool a = true, b = false;. Чему равно a && !b || b && !a? Ответ: true (true && true || false && false -> true || false -> true).
            bool a = true, b = false;
            bool c = a && !b || b && !a;

            Console.WriteLine($"c = {c}");
        }
    }
}


```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.3.6.png">
</picture>

> ### Программа 27. 

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
            // Задача 7: Каков результат true || (x / 0 == 1) при любом целом x? Ответ: true (деление на ноль не произойдет из-за короткого замыкания ||).
            int x = 10;

            bool result = true || (x / 0 == 1);

            Console.WriteLine($"res = {result}");
        }
    }
}


```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.3.7.png">
</picture>

> ### Программа 28. 

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
            // Задача 8: Каков результат false & (10 / 0 == 1)? Ответ: Выбросится исключение DivideByZeroException, так как & обязательно вычисляет правый операнд.
            bool x = false & (10 / 0 == 1);

            Console.WriteLine($"x = {x}");
        }
    }
}


```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.3.8.png">
</picture>

> ### Программа 29. 

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
            // Задача 9: Чему эквивалентно выражение !(A && B) по закону де Моргана? Ответ: !A || !B.
            bool A = true, B = false;
            bool Morgan = !(A && B);
            bool MorganEquivalent = !A || !B;

            Console.WriteLine($"{Morgan}, {MorganEquivalent}");
        }
    }
}


```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.3.9.png">
</picture>

> ### Программа 30. 

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
            // Задача 10: Чему эквивалентно выражение !(A || B) по закону де Моргана? Ответ: !A && !B.
            bool A = true, B = false;
            bool Morgan = !(A || B);
            bool MorganEquivalent = !A && !B;

            Console.WriteLine($"{Morgan}, {MorganEquivalent}");
        }
    }
}

```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.3.10.png">
</picture>

> ### Программа 31. 

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
            // Задача 1: Чему равен результат 5 & 3 в двоичном и десятичном виде? Ответ: 0101 & 0011 = 0001 (десятичное 1).
            int x = 5 & 3;

            Console.WriteLine($"{x}");
        }
    }
}


```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.4.1.png">
</picture>

> ### Программа 32. 

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
            // Задача 2: Чему равен результат 5 | 3? Ответ: 0101 | 0011 = 0111 (десятичное 7).
            int x = 5 | 3;

            Console.WriteLine($"{x}");
        }
    }
}

```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.4.2.png">
</picture>


> ### Программа 33. 

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
            // Задача 3: Чему равен результат 5 ^ 3? Ответ: 0101 ^ 0011 = 0110 (десятичное 6).
            int x = 5 ^ 3;
            Console.WriteLine($"{x}");
        }
    }
}


```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.4.3.png">
</picture>


> ### Программа 34. 

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
            // Задача 4: Вычислите ~0 для типа int. Ответ: -1 (все биты устанавливаются в 1, что в дополнительном коде равно -1).
            int x = ~0;
            Console.WriteLine($"{x}");
        }
    }
}


```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.4.4.png">
</picture>


> ### Программа 35. 

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
            // Задача 5: Чему равно 1 << 4? Ответ: 16 ( 1 × 2^4 ).
            int x = 1 << 4;
            Console.WriteLine($"{x}");
        }
    }
}


```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.4.5.png">
</picture>


> ### Программа 36. 

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
            // Задача 6: Чему равно 40 >> 2? Ответ: 10 ( 40 /  2^2 ).
            int x = 40 >> 2;
            Console.WriteLine($"{x}");
        }
    }
}


```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.4.6.png">
</picture>


> ### Программа 37. 

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
            // Задача 7: Как с помощью побитовой операции проверить, установлен ли третий бит числа n (маска 2^3 = 8 )? Ответ: (n & 8) != 0 или(n & (1 << 3)) != 0.
            int n = 13;
            bool x = (n & 8) != 0;
            bool y = (n & (1 << 3)) != 0;
            if (x)
            {
                Console.WriteLine("3-й бит установлен");
            }
            else
            {
                Console.WriteLine("3-й бит не установлен");
            }
        }
    }
}

```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.4.7.png">
</picture>


> ### Программа 38.

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
            // Задача 8: Как с помощью побитовой операции установить 2 - й бит числа n в 1 ? Ответ : n = n | (1 << 2); (или n |= (1 << 2);).
            int n = 8;
            n |= (1 << 2);
            Console.WriteLine(n);
        }
    }
}

```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.4.8.png">
</picture>


> ### Программа 39.

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
            // Задача 9: Как сбросить (установить в 0) 4-й бит числа n? Ответ: n = n & ~(1 << 4); (или n &= ~(1 << 4);).
            int n = 20;
            n &= ~(1 << n);
            Console.WriteLine($"{n}");
        }
    }
}


```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.4.9.png">
</picture>


> ### Программа 40. 

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
            // Задача 10: Каков результат выражения (-16) >> 2 для int? Ответ: -4 (арифметический сдвиг вправо сохраняет знаковый бит 1).
            int x = (-16) >> 2;
            Console.WriteLine($"{x}");
        }
    }
}


```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.4.10.png">
</picture>


> ### Программа 41. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace program
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Задача 1: Что делает оператор x += 5? Ответ: Эквивалентен x = x + 5 (с приведением типа при необходимости).
            int x = 10;
            x += 5;
            Console.WriteLine($"{x}");
        }
    }
}

```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.5.1.png">
</picture>

> ### Программа 42. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace z
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Задача 2: Каково значение a после выполнения: int a = 10; a *= 2 + 3;? Ответ: 50 (правая часть вычисляется полностью перед умножением: a = a * (2 + 3)).
            int a = 10;
            a *= 2 + 3;
            Console.WriteLine($"{a}");
        }
    }
}

```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.5.2.png">
</picture>


> ### Программа 43. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace z
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Задача 3: Чему равен x после int x = 12; x >>= 2;? Ответ: 3
            int x = 12;
            x >>= 2;
            Console.WriteLine($"{x}");
        }
    }
}

```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.5.3.png">
</picture>

> ### Программа 44. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace z
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Задача 4: Что делает оператор x ??= y? Ответ: Присваивает переменной x значение y только в том случае, если x == null.
            int? x = null;
            int y = 5;
            x = x ?? y;
            Console.WriteLine($"{x}");
        }
    }
}

```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.5.4.png">
</picture>

> ### Программа 45. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace z
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Задача 5: Чему будет равна строка str после: string str = null; str ??= "default"; str ??= "custom";
            string str = null;
            str = str ?? "default";
            str = str ?? "custom";
            Console.WriteLine($"{str}");
        }
    }
}

```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.5.5.png">
</picture>

> ### Программа 46. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace z
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Задача 6: Допустимо ли выражение byte b = 1; b += 2; без явного приведения? Ответ: Да, составные операторы присваивания содержат неявное сужающее приведение типа: b = (byte)(b + 2).
            byte b = 1;
            b += 2;
            Console.WriteLine($"{b}");
        }
    }
}

```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.5.6.png">
</picture>

> ### Программа 47. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace z
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Задача 7: Чему равно значение c после int a = 5, b = 10, c = 0; c = a = b;? Ответ: 10 (присваивание ассоциативно справа налево).
            int a = 5, b = 10, c = 0;
            c = a = b;
            Console.WriteLine($"{c}, {a}");
        }
    }
}

```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.5.7.png">
</picture>

> ### Программа 48. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace z
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Задача 8: Каково значение mask после: int mask = 1; mask <<= 3; mask |= 2;? Ответ: 10 (1 << 3 = 8, затем 8 | 2 = 10).
            int mask = 1;
            mask <<= 3;
            mask |= 2;
            Console.WriteLine($"{mask}");
        }
    }
}

```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.5.8.png">
</picture>

> ### Программа 49. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace z
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Задача 9: Чему равно x после int x = 15; x %= 4;? Ответ: 3.
            int x = 15;
            x %= 4;
            Console.WriteLine($"{x}");
        }
    }
}

```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.5.9.png">
</picture>

> ### Программа 50. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace z
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Задача 10: Чему равно int? count = null; int res = count?.GetHashCode() ?? -1;? Ответ: -1.
            int? count = null;
            int res = count?.GetHashCode() ?? -1;
            Console.WriteLine($"{res}");
        }
    }
}

```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.5.10.png">
</picture>

> ### Программа 51. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace l
{
    internal class Program
    {
        static void Main(string[] args)
        {
        // Задача 1: Вычислите int score = 75; string res = score >= 60 ? "Pass" : "Fail";. Ответ: "Pass".
        int score = 75;
        string res = score >= 60 ? "Pass" : "Fail";
        Console.WriteLine($"{res}");
        }
    }
}

```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.6.1.png">
</picture>

> ### Программа 52. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace l
{
    internal class Program
    {
        static void Main(string[] args)
        {
        // Задача 2 : Чему равно int x = 5; int y = (x > 10) ? 100 : (x > 2) ? 50 : 0;? Ответ: 50.
        int x = 5;
        int y = (x > 10) ? 100 : (x > 2) ? 50 : 0;
        Console.WriteLine($"{y}");
        }
    }
}

```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.6.2.png">
</picture>

> ### Программа 53. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace l
{
    internal class Program
    {
        static void Main(string[] args)
        {
        // Задача 3: Какой тип имеет результат выражения true ? 10 : 15.5 ? Ответ : double.
        double result = true ? 10 : 15.5;
        Console.WriteLine($"{result}");
        }
    }
}

```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.6.3.png">
</picture>

> ### Программа 54. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace l
{
    internal class Program
    {
        static void Main(string[] args)
        {
        // Задача 4 : Что выведет выражение string s = null; Console.WriteLine(s?.Length);? Ответ: Ничего / null (оператор ?. предотвращает NullReferenceException).
        string s = null;
        Console.WriteLine(s?.Length);
        }
    }
}
```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.6.4.png">
</picture>

> ### Программа 55. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace l
{
    internal class Program
    {
        static void Main(string[] args)
        {
        // Задача 5: Какой тип имеет результат выражения s?.Length для string s? Ответ: int? (Nullable<int>).
        string s = "Сигмаплеер";
        int? lenght = s?.Length;
        Console.WriteLine($"{lenght}");
        }
    }
}

```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.6.5.png">
</picture>

> ### Программа 56. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace l
{
    internal class Program
    {
        static void Main(string[] args)
        {
        // Задача 6: Вычислите: string name = null; string res = name ?? "Anonymous";. Ответ: "Anonymous".
        string name = null;
        string res = name ?? "Anonymous";
        Console.WriteLine($"{res}");
        }
    }
}

```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.6.6.png">
</picture>

> ### Программа 57. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace l
{
    internal class Program
    {
        static void Main(string[] args)
        {
        // Задача 7: Вычислите: string a = null, b = "User", c = "Admin"; string res = a ?? b ?? c;. Ответ: "User".
        string a = null, b = "User", c = "Admin";
        string res = a ?? b ?? c;
        Console.WriteLine($"{res}");
        }
    }
}

```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.6.7.png">
</picture>

> ### Программа 58. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace l
{
    internal class Program
    {
        static void Main(string[] args)
        {
        // Задача 8: Что вернет выражение false ? (10 / 0) : 42 ? Ответ : 42(второй операнд не вычисляется из - за ложного условия).
        int zero = 0;
        int result = false ? (10 / zero) : 42;
        Console.WriteLine($"{result}");
        }
    }
}

```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.6.8.png">
</picture>

> ### Программа 59. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace l
{
    internal class Program
    {
        static void Main(string[] args)
        {
        // Задача 9: Скомпилируется ли код var x = condition ? 10 : "text";? Ответ: Нет (в классическом C#), так как у типов int и string нет неявного взаимного приведения.
        bool condition = true;
        var x = condition ? 10 : "text"; // код не скомпилируется, как дано по условию
        }
    }
}
```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.6.9.png">
</picture>

> ### Программа 60. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace l
{
    internal class Program
    {
        static void Main(string[] args)
        {
        // Задача 10: Чему равно int? count = null; int res = count?.GetHashCode() ?? -1;? Ответ: -1.
        int? count = null;
        int res = count?.GetHashCode() ?? -1;
        Console.WriteLine($"{res}");
        }
    }
}

```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.6.10.png">
</picture>

> ### Программа 61. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Cons
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Задача 1: Что вернет выражение object obj = "Hello"; bool check = obj is string;? Ответ: true.
            object obj = "Hello";
            bool check = obj is string;
            Console.WriteLine($"{check}");
        }
    }
}

```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.7.1.png">
</picture>



> ### Программа 62. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Cons
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Задача 2 : Что вернет object obj = 123; string s = obj as string;? Ответ: null (оператор as возвращает null при невозможности безопасного приведения ссылочного типа).
            object obj = 123;
            string s = obj as string;
            Console.WriteLine(s ?? "null");
        }
    }
}


```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.7.2.png">
</picture>

> ### Программа 63. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Cons
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Задача 3: Что произойдет при явном приведении object obj = 123; string s = (string)obj;? Ответ: Выбросится исключение System.InvalidCastException.
            object obj = 123;
            string s = (string)obj;
            Console.WriteLine($"{s}");
        }
    }
}

```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.7.3.png">
</picture>

> ### Программа 64. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Cons
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Задача 4: Что вернет typeof(int) == typeof(Int32)? Ответ: true (псевдоним языка ссылается на один и тот же тип CLR).
            bool res = typeof(int) == typeof(Int32);
            Console.WriteLine($"{res}");
        }
    }
}


```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.7.4.png">
</picture>

> ### Программа 65. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Cons
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Задача 5: Чему равен результат sizeof(long) в байтах? Ответ: 8.
            int res = sizeof(long);
            Console.WriteLine($"{res}");
        }
    }
}

```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.7.5.png">
</picture>

> ### Программа 66. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Cons
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Задача 6 : Что вернет null is string? Ответ: false (шаблон is для null всегда возвращает false, кроме шаблона is null).
            object obj = null;
            bool res = obj is string;
            Console.WriteLine($"{res}");
        }
    }
}

```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.7.6.png">
</picture>

> ### Программа 67. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Cons
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Задача 7: Что вернет выражение object x = null; bool b = x is null;? Ответ: true.
            object x = null;
            bool b = x is null;
            Console.WriteLine($"{b}");
        }
    }
}


```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.7.7.png">
</picture>

> ### Программа 68. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Cons
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Задача 8: Каков результат (int)3.99? Ответ: 3 (дробная часть отсекается без округления).
            int res = (int)3.99;
            Console.WriteLine($"{res}");
        }
    }
}


```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.7.8.png">
</picture>

> ### Программа 69. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Cons
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Задача 9: Каков результат pattern matching: object o = 42; if (o is int val && val > 40) { ... } Будет ли выполнено тело блока? Ответ: Да, val получит значение 42, условие val > 40 истинно.
            object o = 42;
            if (o is int val && val > 40)
            {
                Console.WriteLine($"val = {val}");
            }
        }
    }
}


```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.7.9.png">
</picture>

> ### Программа 70. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Cons
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Задача 10: Что вернет выражение default(int) и default(string)? Ответ: 0 и null.
            Console.WriteLine($"{default(int)}, {default(string) ?? "null"}");
        }
    }
}

```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task2./blob/main/asssets/3.7.10.png">
</picture>

---

🧑‍💻 Ссылка на практическую работу №2 и преподавателя [github](https://github.com/U5er01Task/Fundamentals-of-Algorithmization-and-Programming-2026/tree/main) - [Преподаватель](https://github.com/U5er01Task)

---
