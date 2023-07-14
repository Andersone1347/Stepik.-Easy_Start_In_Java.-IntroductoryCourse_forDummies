# Stepik.-Easy_Start_In_Java.-IntroductoryCourse_forDummies

## Задачки

### 2 Базовые понятия.

#### 2.1 

##### Вывод в консоль hello world.
```
class Main {
    public static void main(String[] args) {
        System.out.println("Hello, World!"); // сокращённо sout 
    }}

```
---

#### 2.2 Комментарии

```
class Main {
    public static void main(String[] args) {
        //System.out.println("Однострочный"); 
        /*много
          строчный 
          коментарий*/ 
        System.out.println("Hello, World!");
    }
}
```

#### 2.3 Переменные

##### Задача

Доработайте программу так, чтобы она выводила на печать имя, возраст и рост. 

Sample Input:


Sample Output:

Ivan
25
1.85

```
class Man {
    public static void main(String[] args) {
        ______ name = "Ivan";
        ___ age = 25;
        ______ height = 1.85;
        System.out.println(name);
        System.out.println(age);
        System.out.println(height);
    }
}
```

##### Решение 

Имя стринг, возраст инт и рост в дабл.

```
class Man {
    public static void main(String[] args) {
        String name = "Ivan";
        int age = 25;
        double height = 1.85;
        System.out.println(name);
        System.out.println(age);
        System.out.println(height);
    }
}
```

##### Задача

Доработайте программу так, чтобы она выводила на печать имя "Ivan" (без кавычек).

Sample Input:


Sample Output:

Ivan

```
class  {
    public static void main() {
        //put your code here
        System.out.println();
    }
}
```

##### Решение 

Отсувствует название класса и в методе main не прописанно (String[] args). Создаём стринг name и выводим через sout.

```
class Main {
    public static void main(String[] args) {
        String name = "Ivan";
        System.out.println(name);
    }
}
```

##### Задача

Присвойте переменной myVar значение 3.1415 и выведите на печать.

Sample Input:


Sample Output:

3.1415

```
class Main {
    public static void main(String[] args) {
        //put your code here
        System.out.print(myVar);
  }
}
```
##### Решение 

Создать переменную double, назвать её myVar и вывести через sout.
```
class Main {
    public static void main(String[] args) {
        double myVar = 3.1415;
        System.out.print(myVar);
    }
}
```

##### Задача

Напишите программу, выводящую на печать фразу "Я программирую на Java" (без кавычек).

Sample Input:


Sample Output:

Я программирую на Java

```
class Main {
    public static void main(String[] args) {
        //put your code here        
    }
}
```
##### Решение 
Sout и нужная фраза.
```
class Main {
    public static void main(String[] args) {
        System.out.println("Я программирую на Java");
    }
}
```

##### Задача

Напишите программу, которая присваивает трем переменным значения 100, 200 и 300.

Выведите на печать значения переменных в столбик, а затем в строку через пробел.

Примечание 1. Вспомните о различии методов println() и print().

Примечание 2. Пробел - это не пустота, а тоже символ.

Sample Input:


Sample Output:

100
200
300
100 200 300

##### Решение 
Создал 3 инта, вывел 3 с новой строки, и тоже самое вывел с одной строки через пробел.
```
class Main {
    public static void main(String[] args) {
        int a = 100;
        int b = 200;
        int c = 300;
        System.out.println(a);
        System.out.println(b);
        System.out.println(c);
        System.out.print(a +" "+ b +" "+ c);
    }
}
```
Альтернативное решение для понипания различия println() и print()

```
class Main {
    public static void main(String[] args) {
        int a = 100;
        int b = 200;
        int c = 300;
        System.out.println(a);
        System.out.println(b);
        System.out.println(c);
        System.out.print(a+" ");
        System.out.print(b+" ");
        System.out.print(c);
    }
}
```

##### Задача

Создайте четыре переменных разного типа и выведите их на печать, каждое на новой строке. Присвойте переменным значения:

1)  2021

2)  3.1415

3)  Java

4) 5  < 10

Выведите значения переменных столбиком в этом же порядке. 

Sample Input:


Sample Output:

2021
3.1415
Java
true

##### Решение 
Создаём переменные под тип данных и выводим через sout.
```
class Main {
    public static void main(String[] args) {
        int a = 2021;
        double b = 3.1415;
        String c = "Java";
        boolean d = 5  < 10;
        System.out.println(a);
        System.out.println(b);
        System.out.println(c);
        System.out.println(d);
    }
}
```
---
#### 2.4 Ввод данных

##### Задача 

Доработайте программу так, чтобы она считывала строку, а затем выводила эту же строку на печать.

Примечание. В этой задаче, как и в большинстве других, есть скрытые тесты с другими значениями ввода. Код не должен быть привязан к конкретным данным.

Sample Input:

10
Sample Output:

10
```
import java.util.Scanner;

class Test {
    public static void main(String[] args) {
        _______ sc = new Scanner(System.in);
        String st = sc.________();

   }
}
```
##### Решение 

Scanner, nextline(), и через соут выводим стринг , который считывает сканер.

```
import java.util.Scanner;

class Test {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String st = sc.nextLine();
        System.out.println(st);
    }
}
```
Альтернативное решение :           
Без записывания в стринг, а сразу в соут и в конце закрытие сканера close.
```
import java.util.Scanner;

class test {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print (sc.nextLine());
        sc.close();
    }
}
```
##### Задача 

Напишите программу, которая считывает имя пользователя и затем приветствует его.

Sample Input:

Нео
Sample Output:

Привет, Нео

```
class MySolution {
    public static void main(String[] args) {
        //put your code here        
    }
}
```
##### Решение 
Создаём сканер, в сауте пишем нужный текст + полученные данные со сканера.
```
import java.util.Scanner;

class MySolution {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.println("Привет, "+sc.nextLine());
        sc.close();
    }
}
```

Альтернативное решение: 
В одну строку.
```
import java.util.Scanner;
class Main {
public static void main(String[] args) {
        System.out.println("Привет, "+(new Scanner(System.in)).nextLine());     
  }
}
```

##### Задача 
Напишите программу, которая считывает строку, а затем выводит эту же строку на печать 3 раза в столбик.

Sample Input:

Java сложный, прямо капец
Sample Output:

Java сложный, прямо капец
Java сложный, прямо капец
Java сложный, прямо капец

##### Решение 
Всё как и в прошлых примерах, только три саута.
```
import java.util.Scanner;

class MySolution {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String a = sc.nextLine();
        System.out.println(a);
        System.out.println(a);
        System.out.println(a);
        sc.close();
    }
}
```
Альтернативное решение: 
Через цикл for.
```
import java.util.Scanner;
class Main {
public static void main(String[] args) {
        Scanner st = new Scanner(System.in);
    String string = st.nextLine();
    for (int i = 0; i < 3; i++)
        System.out.println(string);
  }
}
```

##### Задача 

Напишите программу, которая считывает строку, а затем выводит эту же строку на печать 2 раза в первой строке через пробел, а затем ещё два раза в столбик.

Sample Input:

Java forever!
Sample Output:

Java forever! Java forever!
Java forever!
Java forever!

##### Решение 
Через цикл for, c одним принтом до цикла.
```
import java.util.Scanner;

class MySolution {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String a = sc.nextLine();
        System.out.print(a+" ");
        for (int i=0; i<3;i++){
            System.out.println(a);
        }
        sc.close();
    }
}
```

Альтернативное решение через 4 саута:
```
import java.util.Scanner;

class MySolution {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String a = sc.nextLine();
        System.out.print(a+" ");
        System.out.println(a);
        System.out.println(a);
        System.out.println(a);
        sc.close();
    }
}
```
Альтернативное решение c if: 
Если в цикле i==0 то (принт стринг + " ") в противном случае вывод на новой строке.

```
import java.util.Scanner;

class MySolution {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String userString = sc.nextLine(); // счётчик считывает слово
        for (int i=0; i<4; i++) {
            if (i==0) {
                System.out.print(userString + " ");
            } else System.out.println(userString);
        }
    }
}
```
##### Задача 
Напишите программу, которая считывает целое число t - температуру воздуха, и выводит фразу:

Температура воздуха сегодня: t градусов.

Sample Input:

18
Sample Output:

Температура воздуха сегодня: 18 градусов.
##### Решение
Сканер, саут и в строке плюсуем sc.nextInt().
```
import java.util.Scanner;

class fun {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.println("Температура воздуха сегодня: "+sc.nextInt()+" градусов.");
    }
}
```

Альтеративное решение: 
%d в строке выводит int tem.
```
import java.util.Scanner;
class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int tem = sc.nextInt();
        System.out.println(String.format("Температура воздуха сегодня: %d градусов.", tem));
    }
}
```

##### Задача 

Напишите программу, которая принимает три числа - год, месяц и день и выводит на печать фразу:

DD:MM:YYYY.

Проверять валидность даты не требуется.

Sample Input:

2021
01
30
Sample Output:

30:01:2021

##### Решение
Пишем 3 счётчика которые считываю инт и 2 string в соуте склеиваем их черех :.
```
import java.util.Scanner;
class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int a = sc.nextInt();
        String b = sc.next();
        String c = sc.next();
        System.out.println(c+":"+b+":"+a);
    }
}
```
Альтернативное решение
Значения форматного вывода, где %2d это 2 символа инта, %02d ноль если нет второго числа. %4d 4 символа инта.
```
import java.util.Scanner;
class MyClassStudyJava {
public static void main(String[] args) {
    Scanner sc = new Scanner(System.in);
    int y = sc.nextInt();
    int m = sc.nextInt();
    int d = sc.nextInt();
    String str = String.format("%2d:%02d:%4d",d,m,y);
    System.out.print(str);
  }
}
```

##### Задача 

Давайте напишем программу-помощника, которая сообщает, сколько у Вас новых сообщений на почте.

Формат ввода. На первой строке вводится имя пользователя, на второй имя помощника, на третьей - количество сообщений.

Формат вывода - в соответствии с образцом.

Sample Input:

Илон Маск
Рогозин
19
Sample Output:

Привет, Илон Маск, это твой помощник Рогозин.
У тебя 19 новых писем.

##### Решение
Сканер с 2 стрингами и интом,помещаем в шаблон текста и выводим сокращённо.
```
import java.util.Scanner;
class MyClassStudyJava {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String name = sc.nextLine();
        String name2 = sc.nextLine();
        int age = sc.nextInt();

        System.out.println(String.format("Привет, %s, это твой помощник %s.",name,name2));
        System.out.print(String.format("У тебя %d новых писем.",age));
    }
}
```
Альтернaтивное решение: 
более сокращённое
```
import java.util.Scanner;

class MySolution {
    public static void main(String[] args) {
        Scanner rd = new Scanner(System.in);
        System.out.print("Привет, " + rd.nextLine() + ", это твой помощник "+ rd.nextLine() +".\n" + "У тебя " + rd.nextLine() + " новых писем." + "\n");       
    }
}
```
---

#### 2.5 Операторы

##### Задача 

Закончите программу таким образом, чтобы она выводила на печать целое число 5. Переменную можно назвать myVar.

Sample Input:


Sample Output:

5
```
class MyNumber {
    public static void main(String[] args) {
        // put your code here
        System.out.print(myVar);
   }
}
```

##### Решение
Просто создаём переменную int myVar = 5.
```
class MyNumber {
    public static void main(String[] args) {
        int myVar = 5;
        System.out.print(myVar);
    }
}
```

##### Задача 

Завершите программу, которая выводит на печать сумму чисел 2 и 4. Переменную вывода можно назвать myVar.

Sample Input:


Sample Output:

6

```
class MyNumber {
    public static void main(String[] args) {
        int x = 2; int y = 4;
        // put your code here
        System.out.print(myVar);
   }
}
```

##### Решение
аналогично int myVar = x + y;   
```
class MyNumber {
    public static void main(String[] args) {
        int x = 2; int y = 4;
        int myVar = x + y;
        System.out.print(myVar);
    }
}
```

##### Задача 

Напишите программу, которая получает два целых числа и выводит их сумму.

Sample Input:

8 11
Sample Output:

19

##### Решение
Создаём сканер и создаём 2 инта которые считывает сканер , в сауте плюсуем переменные.
```
import java.util.Scanner;

class MyNumber {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int a = sc.nextInt() , b = sc.nextInt();
        sc.close();
        System.out.print(a+b);
    }
}
```
Альтернативное решение:
без переменных.
```
import java.util.Scanner;
class MyNumber {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print(sc.nextInt() + sc.nextInt());
    }
}
```

##### Задача

На вход подаются два положительных действительных числа - стороны прямоугольника. Посчитайте его площадь и периметр и выведите на отдельных строках.

Sample Input:

5 10
Sample Output:

50.0
30.0

##### Решение

Что бы посчитать **площадь S = a * b**, **периметр P = (a + b) * 2**.
Как мы видим **Sample Output:**(выходные данные) записаны в double. Создаём сканер считываем doble и NextDouble соответствено, создаём переменные с формулами и выводим.
```
import java.util.Scanner;

class MyNumber {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        double a = sc.nextDouble() , b = sc.nextDouble();
        sc.close();
        double s = a * b, p = (a+b)*2;
        System.out.println(s);
        System.out.println(p);
    }
}
```
Альтернативное решение:   
c \n.
```
import java.util.Scanner;

class MyNumber {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        double a = sc.nextDouble(), b = sc.nextDouble();
        System.out.print(a * b + "\n" + 2 * (a + b));
    }
}
```

##### Задача

На вход подаётся число x0. Посчитайте значение функции y=5x(вкв)+2x+11 в точке x0 и выведите на печать.

Sample Input:

1
Sample Output:

18.0

##### Решение
Для того что бы возвести в степень нужно записать **Math.pow(a,b)** где **a** - это число, а **b** - это степень.
Создали сканер считываем значение в double x, преобразовываем формулу y = 5*Math.pow(x,2)+2*x + 11. Выводим y.

```
import java.util.Scanner;

class MyNumber {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        double x = sc.nextDouble();
        sc.close();
        double y = 5*Math.pow(x,2)+2*x + 11;
        System.out.print(y);
    }
}
```

##### Задача
На вход подаётся целое числo **n**. Выведите в одной строке через пробел само число, его квадрат и куб.

Sample Input:

2
Sample Output:

2 4 8

##### Решение
Сканер, int n, соут (int)Math.pow(a,b).
```
import java.util.Scanner;
class MyProgram {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        System.out.println(n+" "+(int)Math.pow(n,2)+" "+(int)Math.pow(n,3));
        sc.close();
    }
}
```
##### Задача

На вход подаётся три числа. Выведите на одной строке их среднее арифметическое.    

Примечание. Среднее арифметическое вычисляется по формуле:    
 a + b + c / 3(количество цифр до знака деления)

Sample Input:

1 3 5
Sample Output:

3.0

##### Решение
Сканер, принимаем 3 переменных double, и по формуле выводим в саут.
```
import java.util.Scanner;
class MyProgram {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        double a = sc.nextDouble(), b = sc.nextDouble(), c = sc.nextDouble();
        System.out.println((a+b+c)/3);
        sc.close();
    }
}
```

##### Задача

Завершите программу таким образом, чтобы она выводила на печать остаток от деления 41 на 7. Переменную вывода можно назвать myVar.

Sample Input:


Sample Output:

6

```
class MyNumber {
    public static void main(String[] args) {
        int x = 41; int y = 7;
        // put your code here
        System.out.print(myVar);
   }
}
```
##### Решение
Создаём инт myVar = x%y.
```
class MyNumber {
    public static void main(String[] args) {
        int x = 41; int y = 7;
        int myVar = x%y;
        System.out.print(myVar);
    }
}
```

##### Задача

На вход подаётся целое число. Найдите его последнюю цифру.

Примечание. Для вычислений может понадобиться метод Math.abs(x), возвращающий абсолютное значение (модуль) числа. Это один из множества методов, предоставляемых классом Math. Более подробно этот класс будет рассмотрен в следующих модулях.

Sample Input:

365
Sample Output:

5
##### Решение
Что бы найти последнее число, надо число, знак остаток от деления на 10, + Math.abc().
```
import java.util.Scanner;
class MyNumber {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print(Math.abs(sc.nextInt()%10));
    }
}
```
Альтернативное решение:
sout в одну строку.
```
import java.util.Scanner;
class MyNumber {
    public static void main(String[] args) {
        System.out.print(Math.abs(new Scanner(System.in).nextInt() % 10));
   }
}
```
##### Задача
ООО "Круче Гугла" нанимает Java-разработчиков. Месячный бюджет на зарплату разработчиков - X, зарплата одного разработчика - Y. Выведите на печать в одной строке через пробел, какое максимальное количество разработчиков компания сможет нанять, и какое количество денег из ежемесячного бюджета останется неиспользованным.

Sample Input:

16 5
Sample Output:

3 1
##### Решение
Что бы получить первое число используем деление, а второе остаток от деления.
```
import java.util.Scanner;
class MyNumber {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int a = sc.nextInt(),b = sc.nextInt();
        System.out.print(a/b+" ");
        System.out.print(a%b);
    }
}
```
##### Задача
Задача повышенной сложности

Реализуйте простые домашние часы.

На вход подаётся число секунд, которое прошло с момента начала суток (00:00:00). Выведите текущее время в формате ЧЧ:ММ:СС.

Примечание 1. Используйте 24-часовой формат.

Примечание 2. Для преобразования типа int в тип String (если это понадобится) можно использовать встроенный служебный метод String.valueOf(num), который преобразует число num в строку "num".

Sample Input 1:

41000
Sample Output 1:

11:23:20
Sample Input 2:

3600
Sample Output 2:

01:00:00

##### Решение
Код с пояснениями формул решения.
```
import java.util.Scanner;

class MyNumber {
   public static void main(String[] args) {
       Scanner t = new Scanner(System.in);
       int sec = t.nextInt();
       sec %=24*60*60; // проверка, что в данных секундах не было больше суток
       int hour = sec/3600; // находим часы, просто сколько содержится 3600 секунд(час) в данных секундах
       int min = sec%3600/60; // находим остаток секунд которые не входит в целый час, а потом делим на 60 сек(час)
       int s=sec%60; // находим остаток от деления всех минут

       System.out.print(String.format("%02d:%02d:%02d",hour,min,s));
   }
}
```
---
#### 2.6 Инкремент
##### Задача
Измените программу таким образом, чтобы она выводила на печать число 11.

Sample Input:


Sample Output:

11
```
class myNumber {
    public static void main(String[] args) {
        int x = 10;
        // put your code here        
   }
}
```
##### Решение
С помощью инкремента x++;.
```
class myNumber {
    public static void main(String[] args) {
        int x = 10;
        x++;
        System.out.println(x);
    }
}
```
##### Задача
Измените программу таким образом, чтобы она выводила на печать числа 11, 12, 13. Используйте инкремент.

Sample Input:


Sample Output:

11
12
13
```
class MyNumber {
    public static void main(String[] args) {
        int x = 10;
        // put your code here
    }
}
```
##### Решение
через инкремент в цикле for.
```
class MyNumber {
    public static void main(String[] args) {
        int x = 11;
        for (int i = x; i<=13; i++){
            System.out.println(i);
        }
    }
}
```
Альтернатива:
инкременте в саут
```
class MyNumber {
   public static void main(String[] args) {
       int x = 10;
       System.out.println(++x);
       System.out.println(++x);
       System.out.println(++x);
   }
}

```
##### Задача
Завершите программу таким образом, чтобы она выводила на печать число 13.

Sample Input:


Sample Output:

13
```
class MyNumber {
    public static void main(String[] args) {
        int x = 25; int y;
        // put your code here
        System.out.print();
   }
}
```
##### Решение
обьявляем у 12 и x-y в саут.
```
class MyNumber {
    public static void main(String[] args) {
        int x = 25, y=12;
        System.out.print(x-y);
    }
}
```
Альтернатива без у.
```
class MyNumber {
    public static void main(String[] args) {
        int x = 25; int y;
        x -= 12;
        System.out.print(x);
   }
}
```
##### Задача
На вход подаётся натуральное число n. Выведите на печать числа n - 1, n, n + 1 в одну строку, через пробел (см. образец).

Sample Input:

10
Sample Output:

9 10 11
##### Решение
через сканер выводим декремент, инкремент и инкремент.
```
import java.util.Scanner;
class MyNumber {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int a = sc.nextInt();
        System.out.println(--a+" "+ ++a +" "+ ++a);
    }
}
```
##### Задача
На вход подаются два числа: x и y.
Выведите на печать значение выражения
z= (x+1)/(y-1) + (y+1)/(x-1)   
Гарантируется, что x != 1 && у != 1
##### Решение
Сканер 2 инта, и по формуле в соут.
```
import java.util.Scanner;

class MyNumber {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int a = sc.nextInt(), b = sc.nextInt();
        System.out.println((a+1)/(b-1) + (b+1)/(a-1));
    }
}
```
Альтернативное решение:
Через инкремент и декремент.
```
import java.util.Scanner;
class MyNumber {
   public static void main(String[] args) {
       Scanner sc = new Scanner(System.in);
       int x = sc.nextInt();
       int y = sc.nextInt();
       ++x;
       --y;
       System.out.print((x--/y++) + (++y/--x));
   }
}
```

#### 2.7 Строки

##### Задача
Завершите программу таким образом, чтобы она выводила на печать приветствие Hello, World!

Sample Input:


Sample Output:

Hello, World!
```
class MyString {
   public static void main(String[] args) {
       ______ myVar;
       myVar = 
       System.out.print();
   }
}
```
##### Решение 
```
class MyString {
   public static void main(String[] args) {
       String myVar;
       myVar = "Hello, World!";
       System.out.print(myVar);
   }
}
```
##### Задача
На вход подаётся строка. Выведите её длину.

Sample Input:

abracadabra
Sample Output:

11
##### Решение
Используем length(), для того что бы найти длину строки, которую передаём через сканер.
```
import java.util.Scanner;
class MyNumber {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String a = sc.nextLine();
        System.out.println(a.length());
    }
}
```
##### Задача
На вход подаётся строка текста. Выведите её первый и последний элемент в одну строку через пробел. 

Sample Input:

abracadabra
Sample Output:

a a
##### Решение
Для того что бы взять первый и последний символ, используем CharAt().
Сканер передаёт информацию в стринг а,создаём инт b и пихаем в него a.length(). Далее выводим через соут a.CharAt(0) это первая буква, и a.CharAt(b-1) это последняя.
```
import java.util.Scanner;
class MyNumber {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String a = sc.nextLine();
        int b = a.length();
        System.out.println(a.charAt(0)+" "+a.charAt(b-1));
    }
}
```
Альтернативное:
более короткое
```
import java.util.Scanner;

class MyProgram {
    public static void main(String[] args) {
        String str = new Scanner(System.in).nextLine();
        System.out.print(str.charAt(0) + " " + str.charAt(str.length() - 1));
    }
}
```
##### Задача
На вход подаётся строка текста, затем слово. Выведите на печать true, если слово содержится в строке, и false - если не содержится.

Sample Input 1:

My name is John
name
Sample Output 1:

true
Sample Input 2:

My name is John
john
Sample Output 2:

false
##### Решение
Пишем сканер на 2 стринга, и с помощью метода контеинс проверяем есть ли в первом стринге второй.
```
import java.util.Scanner;

class myNumber {
    public static void main(String[] args) {
        int x = 10;
        Scanner sc = new Scanner(System.in);
        String a = sc.nextLine(), b =sc.nextLine();
        System.out.println(a.contains(b));
    }
}
```
##### Задача
На вход подаётся строка. Выведите её на печать сначала строчными, а затем прописными буквами.

Sample Input:

This is new string
Sample Output:

this is new string
THIS IS NEW STRING
##### Решение
Сканер,стринг, в соуте ловер энд апер.
```
import java.util.Scanner;
class myNumber {
    public static void main(String[] args) {
        int x = 10;
        Scanner sc = new Scanner(System.in);
        String a = sc.nextLine();
        System.out.println(a.toLowerCase()+"\n"+a.toUpperCase());
    }
}
```
##### Задача
На вход подаётся строка, а затем целое число n > 0. Выведите n- й символ с начала строки. 

Sample Input:

This is a string
1
Sample Output:

T
##### Решение
Сканер, стринг и инт, соут стринг charAt() и засовываем в него инт - 1.
```
import java.util.Scanner;
class myNumber {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String a = sc.nextLine();
        int b = sc.nextInt();
        System.out.println(a.charAt(b-1));
    }
}
```
##### Задача
На вход подаются две строки текста. Выведите на печать true, если строки совпадают, и false - если нет.

Sample Input 1:

abracadabra
abracadabra
Sample Output 1:

true
Sample Input 2:

My name is John
My name is Boris
Sample Output 2:

false
##### Решение
Сканер 2 стринга, создаём ещё один стринг который с пробелом склеивает те два, соут третий стринг \n третий стринг length()
```
import java.util.Scanner;
class myNumber {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String a = sc.nextLine(), b = sc.nextLine(), c = a+" "+b;
        System.out.println(c+"\n"+c.length());
    }
}
```
Альтернативное короткое решение:
```
import java.util.Scanner;
class is_John {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String str = (sc.nextLine() + " " + sc.nextLine());
        System.out.format("%s\n%d", str, str.length());
    }
}
```
##### Задача
На вход подаются два числа. Выведите сначала их сумму, а на следующей строке переведите числа в строковый формат и сложите в строковом формате.

Sample Input:

8 11
Sample Output:

19
811
##### Решение
Сканер двух интов, инт с сложение их, перевод интов в стринг Integer.toString(a,b); далее вывод.
```
import java.util.Scanner;
class myNumber {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int a = sc.nextInt(), b = sc.nextInt(), c = a+b;
        Integer.toString(a,b);
        System.out.format(c+"\n"+a+b);
    }
}
```
##### Задача
Сравнение строк

Строки, подобно числам, можно сравнивать. Это весьма полезно, если, к примеру, нужно отсортировать список каких-нибудь слов по алфавиту. Однако, если мы просто напишем:

System.out.println("Python" > "Java");
то компилятор выдаст ошибку.

Чтобы сравнить слова, мы должны сделать это посимвольно. Символьный тип в Java - это char. Сравним первые буквы:

System.out.println("Python".charAt(0) > "Java".charAt(0)); // true
Такое сравнение возможно, так как char является числовым типом, а не строковым. Когда мы присваиваем переменной типа char какое-нибудь значение, на самом деле мы сохраняем в переменной число, соответствующее номеру данного символа в  символьной таблице Unicode.  Символ P (латиницей) имеет значение 80, а символ J - 74, поэтому 'P' > 'J'.

Кстати, переменной char можно присвоить и численное значение. Обратите внимание, что переменные типа char заключаются в одинарные кавычки, в отличие от строк.

char a, b;
a = 80;
b = 'J';
System.out.println(a); // P
System.out.println(b); // J
В таблице Unicode представлены все возможные буквы всех языков мира, спецсимволы и масса других символов.

 

На вход подаются два слова на одной строке, разделённые пробелом. Выведите true, если они идут по алфавиту, и false, если нет. Гарантируется, что слова начинаются с разных букв.

Примечание. Использовать условные конструкции для решения этой задачи не нужно.

Sample Input 1:

task angel
Sample Output 1:

false
Sample Input 2:

moment twix
Sample Output 2:

true

##### Решение
Сканер 2 стринга, sc.next считывает до пробела, с помощью charAt(0) сравниваем по первой букве(то есть по индексу).

[Таблица Символов по номеру](https://istarik.ru/blog/programmirovanie/53.html)
```
import java.util.Scanner;

class MyProgram {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String a = sc.next();
        String b = sc.next();
        System.out.println(a.charAt(0)<b.charAt(0));
    }
}
```
---
###### 2.8 Тест

##### Задача
Завершите код, выводящий на печать сумму двух чисел. Не меняйте значение переменных.

Sample Input:


Sample Output:

11
```
class MyNumber {
   public static void main(String[] args) {
       int x = 4; 
           y = 7;
       int sumNum = x   y
       System.out.print();
   }
}
```
##### Решение
Дописал недостающие элементы.
```
class MyNumber {
   public static void main(String[] args) {
       int x = 4; 
          int y = 7;
       int sumNum = x + y;
       System.out.print(sumNum);
   }
}
```
##### Задача
Завершите программу таким образом, чтобы она вывела на печать значение переменной name. Не меняйте значение переменной.

Sample Input:


Sample Output:

Максим
```
class MyString {
   public static void main(String[] args) {
           name;
       name = "Максим"
       out.print();
   }
}
```
##### Решение
Дописал недостающие элементы.
```
class MyString {
    public static void main(String[] args) {

        String name = "Максим";
        System.out.print(name);
    }
}
```
##### Задача
Рептилоиды с планеты Нибиру измеряют время исключительно в секундах. Помогите рептилоидам разобраться, какой промежуток времени в секундах проходит за n земных дней.

 

На вход программа получает n - количество дней.

На выходе программа должна вывести количество секунд в этом количестве дней.

Sample Input:

12
Sample Output:

1036800

##### Решение
Сканер принимает дни в инт, в сауте переводит в секунды.
Расчет количества секунд в сутках 60 секунд * 60 минут * 24 часа= **86 400** секунд.
```
import java.util.Scanner;

class MyString {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print(sc.nextInt()*86400);
    }
}
```
##### Задача
Напишите программу, находящую корни квадратного уравнения  ax(вкв)+bx+c=0

На вход подаются целые числа a, b и c. Выведите сумму и произведение корней в одной строке, через пробел.

Примечание 1. Гарантируется, что существует два различных корня.

Примечание 2. Можно воспользоваться, к примеру, [теоремой Виета](https://ru.wikipedia.org/wiki/Формулы_Виета).

Sample Input:

1 2 -4
Sample Output:

-2.0 -4.0

##### Решение
Сканер 3 инта, облегченная формула суммы (-1*b)/a, и произведения c/a.
```
import java.util.Scanner;

class MyString {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        double a = sc.nextDouble(), b = sc.nextDouble(), c = sc.nextDouble();
        double sum = (-1*b)/a;
        double pro = c/a;
        System.out.println(sum +" "+ pro);
    }
}
```
##### Задача
На вход подаётся число N - номер года по григорианскому календарю. Посчитайте, сколько високосных лет прошло, начиная с 1 года н. э. Будем считать, что григорианский календарь действовал всё это время).

Примечание 1. Правила определения високосного года:

год, номер которого кратен 400, — високосный;
остальные годы, номер которых кратен 100, — невисокосные (например, годы 1700, 1800, 1900, 2100, 2200, 2300);
остальные годы, номер которых кратен 4, — високосные.
Примечание 2. Для решения этой задачи условные конструкции не требуются.

Sample Input 1:

1
Sample Output 1:

0
Sample Input 2:

10
Sample Output 2:

2
##### Решение
Сканер инт, формула подчёта ((a/4 ) - (a/100) + (a/400)).
```
import java.util.Scanner;
class MyProgram {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int a = sc.nextInt();
        int b= ((a/4 ) - (a/100) + (a/400));
        System.out.println(b);
    }
}
```
Альтернатива:     
более подробное
```
import java.util.Scanner;
class MyProgram {
    public static void main(String[] args) {
        
        int n;
        Scanner sc = new Scanner(System.in);
        
        n = sc.nextInt();
        sc.close();         // зкрываем входной поток дабы избежать утечки памяти!
        
        // n/100 - год(а) которые не входять в календарь
        // n/400 - год(а) которые входять в календарь
        // n/4 - год(а) которые входять в календарь
        
        System.out.println(n/400 + n/4 - n/100);
        
    }
}
```
##### Задача
На вход подаются целые числа x и y. Выведите их сумму и разность в формате, соответствующем примеру.

Sample Input:

10 5
Sample Output:

Сложение: 10 + 5 = 15
Вычитание: 10 - 5 = 5

##### Решение
Сканер на 2 инта, вывод по шаблону.
```
import java.util.Scanner;

class MyString {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int a = sc.nextInt(), b = sc.nextInt();
        System.out.println("Сложение: "+a+" + "+b+" = "+(a+b));
        System.out.println("Вычитание: "+a+" - "+b+" = "+(a-b));
    }}
```



---
### 3  Условные конструкции

#### 3.1 Условные конструкции

##### Задача 

Исправьте ошибки в коде таким образом, чтобы код выводил на печать слово "YES" (без кавычек), если значение переменной х равно 5.

Sample Input:


Sample Output:

YES
```
class Example {
	public static void main(String[] args) {
		int x = 5;
        if x = 5 {
            System.println("YEP")

        }	
}
```
##### Решение
В ифе отсувствуют круглые скобки и одна фигурная, в выводе out, и сам вывод одна буква.
```
class Example {
    public static void main(String[] args) {
        int x = 5;
        if ( x == 5) {
            System.out.println("YES");
        }
        }
    }
```
##### Задача
Два индийских программиста, Махатма и Джавахарлал, решили выяснить, кто из них быстрее пишет код. Напишите программу, которая поможет им выяснить это.

На вход подаются два целых числа в одной строке через пробел. Если первое число больше второго, необходимо вывести на печать "Махатма", если второе - "Джавахарлал". Гарантируется, что числа больше нуля и различны.

Sample Input:

8 11
Sample Output:

Джавахарлал

##### Решение
Сканер, 2 инта, через иф.
```
import java.util.Scanner;

class MyString {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int a = sc.nextInt(), b = sc.nextInt();
        if( a>b ){
            System.out.println("Махатма");
        } else {
            System.out.println("Джавахарлал");
        }
    }}
```
##### Задача
Два индийских программиста, Махатма и Джавахарлал, решили выяснить, чей код длиннее. Напишите программу, которая поможет им выяснить это. 

На вход подаются две строки текста. Если первая строка длиннее второй, необходимо вывести на печать "Махатма", если наоборот - "Джавахарлал". Гарантируется, что строки имеют разную длину.

Sample Input:

abracadabra
The world is mine
Sample Output:

Джавахарлал
##### Решение
Всё как в прошлом задание, только инты поменяли на стринги и сравниваем ленг.
```
import java.util.Scanner;

class MyString {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String a = sc.nextLine(), b = sc.nextLine();
        if( a.length()>b.length() ){
            System.out.println("Махатма");
        } else {
            System.out.println("Джавахарлал");
        }
    }}
```
##### Задача
На первой строке подаётся пароль, хранящийся в базе данных, на второй - пароль, введённый пользователем.

Выведите на печать фразу "Access is granted", если пользователь ввёл верный пароль, и "Access is denied" - если нет. 

Sample Input:

111111
111111
Sample Output:

Access is granted
##### Решение
В ифе через экалс.
```
import java.util.Scanner;
class MyString {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String a = sc.nextLine(), b = sc.nextLine();
        if( a.equals(b) ){
            System.out.println("Access is granted");
        } else {
            System.out.println("Access is denied");
        }
    }}
```
##### Задача
Выведите на печать наибольшее из трёх целых чисел.

Sample Input:

5 6 12
Sample Output:

12
##### Решение
С помощью if else сравниваем каждую переменную.
```
import java.util.Scanner;
class MyString {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int a = sc.nextInt(), b = sc.nextInt(), c = sc.nextInt();
        if( a>=b && a>=c ) {
            System.out.println(a);
        } else if (b>=a && b>=c) {
            System.out.println(b);
        } else if (c>=a && c>=b) {
            System.out.println(c);
        }
    }}
```
Альтернативное решение:
Math.max
```
import java.util.Scanner;
class MyProg {
    public static void main(String[] args) {
        Scanner in = new Scanner(System.in);
        System.out.print(Math.max(in.nextInt(), Math.max(in.nextInt(), in.nextInt())));
    }
}
```
Альтернативное решение:
Переназначением
```
import java.util.Scanner;
class MyProg {
	public static void main(String[] args) {
		Scanner consol = new Scanner(System.in);
        int a = consol.nextInt(), b = consol.nextInt(), c = consol.nextInt();
        if (a < b) a = b;
        if (a < c) a = c;
        System.out.println(a);
	}
}
```
##### Задача
В 1997 году во время боксёрского боя за звание чемпиона мира Майк Тайсон откусил ухо Эвандеру Холифилду (не целиком). Рефери нужно определить, как поступить. Если откушенный кусок уха меньше норматива, бой продолжится. Если нет - Майк Тайсон должен быть дисквалифицирован, и чемпионом становится Холифилд.

На вход подаются два числа -  масса откушенного куска уха и норматив. Выведите "Бой продолжается!" или "Холифилд - чемпион!" в зависимости от выполнения условия.

Sample Input:

5 10
Sample Output:

Бой продолжается!

##### Решение
На вход подаются два числа с плавающей точкой, если первое больше или равно второму то Холифилд - чемпион!.
```
import java.util.Scanner;
class MyProg {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        double a = sc.nextDouble(), b = sc.nextDouble();
        System.out.println((a>=b)? "Холифилд - чемпион!" : "Бой продолжается!");
    }
}
```
##### Задача
На вход подаётся целое число n. Выведите "YES", если можно построить правильный многогранник из правильных плоских n-угольников, в противном случае - "NO".

Sample Input:

3
Sample Output:

YES
##### Решение
Сканер, int == 3 || 4 || 5 Yes, else No.
```
import java.util.Scanner;

class MyProgram {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int a = sc.nextInt();
       System.out.println((a==3 || a==4 || a==5) ? "YES" : "NO");
    }
}
```
##### Задача
На вход подаётся целое число. Выведите "YES", если оно нацело делится на 7, и "NO" - если нет.

Sample Input 1:

7
Sample Output 1:

YES
Sample Input 2:

10
Sample Output 2:

NO
##### Решение
На вход подаётся целое число. Используем деление по остатку на 7, равное 0.
```
import java.util.Scanner;
class MyProg {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int a = sc.nextInt();
        System.out.println((a%7 == 0)? "YES" : "NO");
    }
}
```
##### Задача
На вход подаётся целое число. Выведите "YES", если оно нацело делится на 7, но не делится на 5, иначе -  "NO".

Sample Input:

7
Sample Output:

YES
##### Решение
Всё тоже самое, только добавляем и не делиться на 5. Для проверки правильности проверьте число 35, должно быть нет.
```
import java.util.Scanner;
class MyProg {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int a = sc.nextInt();
        System.out.println((a%7 == 0 && a%5 !=0) ? "YES" : "NO");
    }
}
```

---

#### 3.2 Логические конструкции

##### Задача
Исправьте программу таким образом, чтобы она выводила на печать приветствие "Добро пожаловать!".

Sample Input:


Sample Output:

Добро пожаловать!
```
class Main {
	public static void main(String[] args) {
		int age = 23;
        tasks = 4000;
        if age > 21 & tasks > 500 {
            System.out.print("Добро пожаловать!");
        }
	}
}
```
##### Решение
Переменную tasks переводим в int, условие if засовываем в скобки.
```
class Main {
    public static void main(String[] args) {
        int age = 23 , tasks = 4000;
        if (age > 21 & tasks > 500) {
            System.out.print("Добро пожаловать!");
        }
    }
}
```
##### Задача
Давайте убедимся, что мы верно разобрали логическое выражение из предыдущего шага. Просто запустите программу.

Sample Input:

Sample Output:

true
```
class Test {
    public static void main(String[] args) {
        boolean a = true;
        boolean b = false;
        int c = 30;
        int q = 5;
        boolean r = (a || b && c >= 25) || (c < 20 * q) && !(q == 5);
        System.out.println(r);
    }
}
```
##### Решение
Выражение оставляем без изменений оно верно.        
Аргументация :  
        1) Решаем сначала все, что в скобках.Начнем с выражения слева: (a || b && c >= 25)
        2) т.к арифметические операции и операции сравнения выполняется до логических то рассмотрим для начала 
        c >= 25 (true), т.к 30 >= 25
        3) следующий этапом - посчитаем b && c (false), потому что "логическое и" подразумевает что b = false и с = true
        4) и последний этап в левом выражении a || false - результат вычисления будет TRUE
        5) результат выполнения выражения слева: (a || b && c >= 25) = true;
        6) перейдем к вычислениям в правом выражении: (с < 20 * q) && !(q == 5);
        7) 20 * q = 20 * 5 = 100, отсюда с < 100 или 30 < 100 (это истинное выражение, значит true)
        8)!(q == 5), отсюда !(5 == 5) (это ложное выражение, значит false)
        9) мы получаем (true) && (false) (результатом вычисления будет FALSE)
        10) теперь вычислим результат последней операции: TRUE || FALSE (результат вычисления будет true, что и видим в выводе)

##### Задача
На вход подаётся строка, а затем - одна буква. Если строка содержит эту букву или строка длиннее 20 символов, выведите "YES", в противном случае - "NO".

Sample Input:

This is a string
a
Sample Output:

YES
##### Решение
Сканер, 2 стринга, контаинс или ленг.
```
import java.util.Scanner;
class MyProg {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String a = sc.nextLine(), b = sc.nextLine();
        System.out.println((a.contains(b) || a.length() >= 20) ? "YES" : "NO");
    }
}
```
##### Задача
На вход подаются два целых числа.  Выведите на печать true, если их сумма чётна, а произведение - нечётно, и false - в противном случае.

Sample Input:

5 3
Sample Output:

true
##### Решение
Сканер, два инта, сумма интов и проверка на чётность(%2 == 0) && произведение(умножение) интов и нечётность (% 2 !=0)
```
import java.util.Scanner;
class MyProg {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int a = sc.nextInt(), b = sc.nextInt();
        System.out.println(((a+b) % 2 ==0 && (a*b) % 2 !=0));
    }
}
```
##### Задача
На вход подаются три целых числа. Выведите true, если среди них есть ровно два чётных, и false - если нет.

Sample Input:

4 6 7
Sample Output:

true
##### Решение
Сравнил все возможные варианты, и написал условие при 3 чётных интах false.
```
import java.util.Scanner;
class MyProg {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int a = sc.nextInt(), b = sc.nextInt(), c = sc.nextInt();

        boolean d = ((a % 2 == 0) && (b % 2 == 0) || (a % 2 == 0) && (c % 2 == 0) || (b % 2 == 0) && (a % 2 == 0) || (b % 2 == 0) && (c % 2 == 0) || (c % 2 == 0) && (a % 2 == 0) || (c % 2 == 0) && (b % 2 == 0));

        if (a % 2 == 0 && b % 2 == 0 && c % 2 == 0){
            System.out.println("false");
        } else {
            System.out.println(d);
        }
    }
}
```
Альтернативное решение:    
гениальный подход.
```
import java.util.Scanner;
class MyProgram {
	public static void main(String[] args) {
	  Scanner sc = new Scanner(System.in);
        int a = sc.nextInt();
        int b = sc.nextInt();
        int c = sc.nextInt();
        boolean a1 = (a%2+b%2+c%2)==1;
            System.out.println(a1);   
	}
}
```
##### Задача
На вход подаются целых три числа - день, месяц и год (по григорианскому календарю). Выведите true, если эти числа составляют валидную дату, и false - в противном случае.

Примечание.

Не все года одинаковые.

 

Лирическое отступление. 

В комментариях к этой задаче (и ко многим другим) студенты высказываются, что условия сформулированы недостаточно чётко.  Дескать, напишите прямо, какие случаи нужно проверить - и проверим. 

К сожалению, в реальной практике абсолютно чёткие ТЗ (технические задания) Вы будете получать с периодичностью примерно никогда. И это касается не только программирования, но и других сфер. Вам придётся самостоятельно устанавливать границы - где работает код, где нет, каковы его границы и как он работает с заданными критериями. Более того, недалёк тот день, когда для написания кода по абсолютно точному ТЗ люди будут не нужны - это будет делать искусственный интеллект.

Поэтому, крайне важно не бросаться сразу писать код. Наоборот, сядьте и спланируйте - что, где, почему, как. Это позволит избежать стадии вырывания волос на голове с криками "НУ ПОЧЕМУ НЕ РАБОТАЕТ?!!!".

 Именно так работают успешные программисты: сначала проектирование кода, затем его реализация. Привыкайте к этому сразу же. 
 ##### Решение
 ```
import java.util.Scanner;
class Circle {
    public static void main(String[] args) {
        Scanner a = new Scanner(System.in);
        int day = a.nextInt();
        int mon = a.nextInt();
        int year = a.nextInt();

        if ((day >= 1 && day <= 31) && (mon >= 1 && mon <= 12) && year >= 0) {
            if (day <= 29 && mon == 2 && (year % 400 == 0 || year % 4 == 0 && year % 100 != 0)) {
                System.out.println("true");
            } else if (mon == 1 || mon == 3 || mon == 5 || mon == 7 || mon == 8 || mon == 10 || mon == 12 && (day >= 1 && day <= 31)) {
                System.out.println("true");
            } else if ((mon == 4 || mon == 6 || mon == 9 || mon == 11) && (day >= 1 && day <= 30)) {
                System.out.println("true");
            }  else if (day <= 28 && mon == 2 && (year % 4 != 0 || (year % 100 == 0 && year % 400 !=0))) {
                System.out.println("true");
            } else System.out.println("false");
        } else {
            System.out.println("false");
        }
    }
}
 ```
 Альтернативное решение:     
 с пояснениями
 ```
import java.util.Scanner;
class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int day = sc.nextInt();
        int mounth = sc.nextInt();
        int year = sc.nextInt();
        boolean visyear = (year % 4 == 0 && year % 100 != 0) || (year % 400 == 0);    // вычисляем високосные года
        boolean rightmounth = mounth > 0 && mounth <= 12;                     // вычисление правильный месяц
        boolean rightday = day > 0 && day <= 31;                              // вычисление правильный день
        boolean rightyear = year > 0;                                         // вычисление правильный гож
        boolean smallmounth = (mounth == 4 || mounth == 6 || mounth == 9 || mounth == 11); // вычисление маленьких месяцев в которых должно быть меньше 30 дней
        if (rightyear && rightday && rightmounth) {                         // если (год, день и месяц имеют значение true) то
            if (visyear) {                                                  // если (год високосный) то
                if(mounth == 2) {                                           // если (месяц равен 2) то
                    System.out.println(day <= 29);                          // выводим на экран false или true в зависимости от правильности утверждения
                }
            } else {                                                        // в других случаях (то есть когда год високосный)     
                if (mounth == 2) {                    
                    System.out.println(day <= 28);                          // выводим на экран false или true в зависимости от правильности утверждения
                }
            }
            if (smallmounth) {                                              // если (указан маленький месяц) то     
                System.out.println(day <= 30);                              // выводим на экран false или true в зависимости от правильности утверждения
            } else if (!smallmounth && mounth !=2) {System.out.println("true");} // также если (указан не маленький месяц и значение месяца не равно 2) то выводим "true"



        } else {System.out.println("false");}                                 // во всех остальных случаях false
    }
}
 ```
##### Задача
 На вход подаются три слова на одной строке, разделённые пробелом. Выведите их в алфавитном порядке. Гарантируется, что слова начинаются с разных букв.

Sample Input:

Python Java C++
Sample Output:

C++
Java
Python
##### Решение
Сканер 3 стринга, узнаём первые символы стрингов и переводим в чары, сравниваем все возможные варианты и пишем результат.
```
import java.util.Scanner;
class MyProg {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String str1 = sc.next(), str2 = sc.next(), str3 = sc.next();
        char a = str1.charAt(0), b = str2.charAt(0), c = str3.charAt(0);
        if ((a < b) && (a < c) && (b < c)) {System.out.println(str1 +"\n" + str2 + "\n" + str3);}
        if ((b < a) && (a < c) && (b < c)) {System.out.println(str2 + "\n" + str1 + "\n" + str3);}
        if ((c < a) && (a < b) && (c < b)) {System.out.println(str3 + "\n" + str1 + "\n" + str2);}
        if ((a < b) && (a < c) && (c < b)) {System.out.println(str1 + "\n" + str3 + "\n" + str2);}
        if ((b < c) && (b < a) && (c < a)) {System.out.println(str2 + "\n" + str3 + "\n" + str1);}
        if ((c < b) && (c < a) && (b < a)) {System.out.println(str3 + "\n" + str2 + "\n" + str1);}
    }
}
```
Альтернативное решение:            
Пузырьком с пояснением 
```
import java.util.Scanner;
class Program {
    public static void main(String[] args) {
        Scanner scn = new Scanner(System.in);
        String a = scn.next(), b = scn.next(), c = scn.next();
        String n; // n - вспомогательная строка
        if (a.charAt(0)>b.charAt(0)) {n = a; a = b; b = n;} // сравниваем a и b
        if (a.charAt(0)>c.charAt(0)) {n = a; a = c; c = n;} // сравниваем a и c
        if (b.charAt(0)>c.charAt(0)) {n = b; b = c; c = n;} // сравниваем b и c
        System.out.println(a+"\n"+b+"\n"+c);
        scn.close();
    }
}
```
---
#### 3.3 Вложенные условные конструкции

##### Задача
Исправьте программу таким образом, чтобы она вывела на печать "Ура, заработало!!!" (без кавычек).

Sample Input:


Sample Output:

Ура, заработало!!!
```
class Example {
	public static void main(String[] args) {
		int x = 3;
        if x > 15 {
            if (x <= 25) {
                System.out["Ура, заработало!!!"]
            }
        }
    }
}
```

##### Решение
В иф скобки и > на < меняем, в вывод аут и скобки.
```
class Example {
    public static void main(String[] args) {
        int x = 3;
        if (x < 15) {
            if (x <= 25) {
                System.out.println("Ура, заработало!!!");
            }
        }
    }
}
```
##### Задача
На вход подаётся три целых числа. Выведите среднее из них (т.е. не минимальное и не максимальное).

Sample Input:

5 10 11
Sample Output:

10

##### Решение
Сканер 3 инта, и перебираем все возможные комбинации.
```
import java.util.Scanner;

class Example {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int a = sc.nextInt(), b = sc.nextInt(), c = sc.nextInt();
        if ((a >= b && a <= c) || (a <= b && a >= c)){
            System.out.println(a);
        }else if((b >= a && b <= c) || (b <= a && b >= c)){
            System.out.println(b);
        }else  if ((c >= a && c <= b) || (c <= a && c >= b)){
            System.out.println(c);
        }
    }
}
```
Альтернативное решение: 
Заносим в массив и через метод sort.
```
import java.util.Scanner;
import java.util.Arrays;
class Main {
    public static void main(String[] args) {
        Scanner s = new Scanner(System.in);
        int[] numb = {s.nextInt(), s.nextInt(), s.nextInt()};
        Arrays.sort(numb);
        System.out.println(numb[1]);
    }
}
```

##### Задача
ООО "Круче Гугла" наняло трёх разработчиков. Внезапно разработчики узнали, что их зарплаты различаются. Разработчики решили объявить забастовку, если разница максимальной и минимальной зарплаты превысит определённый уровень. Определите, грозит ли ООО "Круче Гугла" забастовка.

Формат ввода:

В первой строке - зарплаты разработчиков через пробел, три целых числа.

Во второй строке - разница, при превышении которой будет объявлена забастовка.

Формат вывода:

"Ура, бастуем!" - если критический уровень превышен;

"За работу, Солнце ещё высоко" - если критический уровень не превышен.

Sample Input:

300 400 500
100
Sample Output:

Ура, бастуем!

##### Решение
Сканер 3 инта , матх макс и мин , if.
```
import java.util.Scanner;

class Example {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int a = sc.nextInt();
        int b = sc.nextInt();
        int c = sc.nextInt();

        int d = sc.nextInt();

        int e = (Math.max(Math.max(a, b),c)) - (Math.min(Math.min(a, b),c));

        if (e>d) {
            System.out.println("Ура, бастуем!");
        }else {
            System.out.println("За работу, Солнце ещё высоко");
        }


    }
}
``` 
##### Задача
Задача повышенной сложности

На числовой прямой даны два отрезка, заданных парами целых чисел: a1,b1 b a2,b2. Напишите программу, которая находит их пересечение.

Если пересечение - отрезок, необходимо вывести два числа (границы отрезка), если единственная точка - единственное число (точку), если пересечения нет - вывести фразу "Пересечения нет" (без кавычек). 

Sample Input 1:

2 5
6 10
Sample Output 1:

Пересечения нет
Sample Input 2:

2 5
4 10
Sample Output 2:

4 5
##### Решение
![alt](/img/%D1%80%D0%B8%D1%81%D1%83%D0%BD%D0%BE%D0%BA%20a1-b1%2Ca2-b2.jpg "a1-b1, a2-b2")
сканер, 4 инта, (a1,b1) и (a2,b2) по картинке сравниваем различные вариации пересечений.
```
import java.util.Scanner;

class Example {
    public static void main(String[] args) {
        Scanner c = new Scanner(System.in);
        int a1 = c.nextInt(), b1 = c.nextInt(), a2 = c.nextInt(),  b2 = c.nextInt();


        if (((a2 - b1) * (b2 - a1)) <= 0) {
            if (((a2 - b1) * (b2 - a1)) == 0) { // d[jl1
            if (a2 == b1) {
                System.out.println(b1);
            }
            if (b2 == a1) {
                System.out.println(b2);
            }
        }
        if (a1 >= a2 && b1 <= b2) { // вхол 2
            System.out.println(a1 + " " + b1);
        }

        if (a2 > a1 && b2 < b1) { // вход 3
            System.out.println(a2 + " " + b2);
        }
            if (a1 < a2 && a2 < b1 && b1 < b2) { // вход 4
                System.out.println(a2 + " " + b1);
            }
            if (a2 < a1 && a1 < b2 && b2 < b1) { // вход 5
                System.out.println(a1 + " " + b2);
            }
    }else {
            System.out.println("Пересечения нет");
        }
}}
```
Альтернативное решение:        
через Math.max и Math.min  .
```
import java.util.Scanner;

class MyProgram {
    public static void main(String[] args) {
    Scanner in = new Scanner(System.in);
        int a1 = in.nextInt();
        int b1 = in.nextInt();
        int a2 = in.nextInt();
        int b2 = in.nextInt();
        int a = Math.max(a1, a2);
        int b = Math.min(b1, b2);
         if (b < a) {
             System.out.println("Пересечения нет");
         } else if (b == a) {
             System.out.println(b);
         } else {
             System.out.println(a+" "+b);
         }
    }
}

```
##### Задача
На вход подаётся три целых числа. Выведите максимальное чётное из них. Если чётных чисел нет, выведите "Чётных чисел нет".

Sample Input:

5 10 15
Sample Output:

10
##### Решение
Сканер 3 инта, проверка на 3 не чётных числа, если 2 то выводим через Мath.max.
```
import java.util.Scanner;
public class Main {
    private final static Scanner scanner = new Scanner(System.in);

    public static void main(String[] args) {
        int a = scanner.nextInt();
        int b = scanner.nextInt();
        int c = scanner.nextInt();
        if (a % 2 != 0 && b % 2 != 0 && c % 2 != 0) {
            System.out.println("Чётных чисел нет");
        } else if (a % 2 == 0 && b % 2 != 0 && c % 2 != 0) {
            System.out.println(a);
        } else if (a % 2 != 0 && b % 2 == 0 && c % 2 != 0) {
            System.out.println(b);
        } else if (a % 2 != 0 && b % 2 != 0 && c % 2 == 0) {
            System.out.println(c);
        } else if (a % 2 == 0 && b % 2 != 0 && c % 2 == 0) {
            System.out.println(Math.max(a,c));
        } else if (a % 2 != 0 && b % 2 == 0 && c % 2 == 0) {
            System.out.println(Math.max(b, c));
        } else if (a % 2 == 0 && b % 2 == 0 && c % 2 != 0) { System.out.println(Math.max(a,b)); 
        } else {
            System.out.println(Math.max(Math.max(a,b),c));
        } 
    }
}
```
---
#### 3.4 Оператор Switch

##### Задача 
Доработайте программу так, чтобы она вывела на печать фразу We're the champions! 

Sample Input:

Sample Output:

We're the champions!
```
class MyNumber {
    public static void main(String[] args) {
        int x = 10; 
        ______ (_) _    

            case 10:
                System.out.print("We're the champions!");

            def____
                System.out.print("We're lost ((");
        }           
    }
}
```
##### Решение
Switch (x) {}, закрыть кейс break;, default: (любое другое значение).
```
class MyNumber {
    public static void main(String[] args) {
        int x = 10;
        switch (x) {

            case 10:
                System.out.print("We're the champions!");
                break;

        default:
        System.out.print("We're lost ((");
    }
}
}
```
##### Задача 
Реализуйте простой справочник по командам Java. На вход подаётся команда, по которой необходима справка (ограничимся тремя командами). В соответствии с этим выведите текст:

Ввод: System.out.println()

Вывод: Это команда вывода на печать

Ввод: if

Вывод: Это условный оператор

Ввод: else

Вывод: Это альтернативная конструкция условного оператора 


Если введено что-либо другое, выведите фразу "Раздел в разработке" (без кавычек).

Sample Input:

System.out.println()
Sample Output:

Это команда вывода на печать
##### Решение
Сканер, в условие свитч, стринг а, и в каждом кейсе скопипастили условия задания. 
```
import java.util.Scanner;

class MyNumber {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String a = sc.nextLine();
        switch (a) {

            case "System.out.println()":
                System.out.print("Это команда вывода на печать");
                break;

            case "if":
                System.out.print("Это условный оператор");
                break;

            case "else":
                System.out.print("Это альтернативная конструкция условного оператора");
                break;
                
        default:
        System.out.print("Раздел в разработке");
    }
}
}
```
---
#### 3.5 Тест

##### Задача 

На вход подаётся  целое число. Выведите "YES", если введено трёхзначное положительное число, а в противном случае - "NO".  

Sample Input 1:

125
Sample Output 1:

YES
Sample Input 2:

1
Sample Output 2:

NO
##### Решение
Cканер int, через тернарный, если >= 10 yes, else no.
```
import java.util.Scanner;

class MyTest {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int a = sc.nextInt();
        System.out.println((a >=100 && a <= 999)?"YES":"NO");
    }
}
```
Альтернативное через ленг и свитч:
```
import java.util.Scanner;
class MyProggg {
   public static void main(String[] args) {
       Scanner sc = new Scanner(System.in);
       String a=sc.nextLine();
        sc.close();
       switch (a.length()){
           case 3:
               System.out.println ("YES");
               break;
           default: System.out.println ("NO");
         }
    
   }
}
```

##### Задача 
На вход подается строка, а затем слово. Выведите true, если слово содержится в строке, и false - если нет, без учёта регистров.

Sample Input:

abracadabra
Cadabra
Sample Output:

true
##### Решение
Переводи в нижний регистр оба стринга и контаинс.
```
import java.util.Scanner;
class MyTest {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String a = sc.nextLine(), b = sc.nextLine();
        System.out.println(a.toLowerCase().contains(b.toLowerCase()));
    }
}
```
##### Задача 
На вход подаётся целое трёхзначное число, а затем цифра. Выведите true, если эта цифра является средней в числе (разряд десятков), и false - если нет. Если введённое число не является трёхзначным, выведите "error".

Sample Input:

123 2
Sample Output:

true
##### Решение
Считываем 2 числа, переводим в стринг, переводи в чар средний символ первого стринга и второй стринг. Далее проверка на то что 1 число от 100 до 999, и проверка на схожесть чаров.
```
import java.util.*;
class Example1{
    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        int a=sc.nextInt();
        int b=sc.nextInt();
        a = Math.abs(a);
        b = Math.abs(b);
        String num1=Integer.toString(a);
        String num2=Integer.toString(b);
        char c=num1.charAt(1);
        char d=num2.charAt(0);
        if(a > 99 && a < 1000){
            if (c == d){
                System.out.println("true");
            }
            else{
                System.out.println("false");
            }
        }
        else{
            System.out.println("error");
        }
    }
}
```
Альтернатива:   
без стрингов и чар, более матиматически верное.
```
import java.util.Scanner;

class Example {
	public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int num = Math.abs(sc.nextInt()), x = Math.abs(sc.nextInt());
        sc.close();
        
        int result = (num / 10) % 10;
        
        if(num > 99 && num < 1000) {
            System.out.println(x == result ? "true" : "false");
        }else {
            System.out.println("error");
        }
    }
}
```
##### Задача 
На вход подаётся два числа - a и b. Выведите знак отношения между числами: один символ "<", если a < b, ">", если a > b и "=", если a=b. 

Sample Input 1:

8 11
Sample Output 1:

<
Sample Input 2:

10 5
Sample Output 2:
\>
##### Решение
doble, else if.
```
import java.util.Scanner;
class MyTest {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        double a = sc.nextDouble(), b = sc.nextDouble();
        if (a<b){
            System.out.println("<");
        } else if (a>b) {
            System.out.println(">");
        } else if (a==b){
            System.out.println("=");
        }
    }
}
```
Альтернативное решение:
через тернарный, кратко.
```
import java.util.Scanner;
class Example {
	public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        double a = sc.nextDouble(), b = sc.nextDouble();
        System.out.print(a < b? '<': a > b? '>': '=');
    }
}
```
##### Задача 
Выведите время года по введённому номеру месяца. Если введён ошибочный номер месяца, выведите "error".

Sample Input:

1
Sample Output:

Зима
##### Решение
Через switch каждый вариант выписан.
```
import java.util.*;
class Example1{
    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        int a =sc.nextInt();

        switch (a){
            case 1 :
                System.out.println("Зима");
                break;
            case 2 :
                System.out.println("Зима");
                break;
            case 3 :
                System.out.println("Весна");
                break;
            case 4 :
                System.out.println("Весна");
                break;
            case 5 :
                System.out.println("Весна");
                break;
            case 6 :
                System.out.println("Лето");
                break;
            case 7 :
                System.out.println("Лето");
                break;
            case 8 :
                System.out.println("Лето");
                break;
            case 9 :
                System.out.println("Осень");
                break;
            case 10 :
                System.out.println("Осень");
                break;
            case 11 :
                System.out.println("Осень");
                break;
                 case 12 :
                System.out.println("Зима");
                break;
            default:
                System.out.println("error");

        }



    }
}
```
Альтернативна:
через switch, более правильно.
```
import java.util.*;
class Example {
	public static void main(String[] args) {
    Scanner sc = new Scanner(System.in);
        int a = sc.nextInt();
        switch (a) {
            case 1:
            case 2:
            case 12:
                System.out.print("Зима");
                break;
            case 3:
            case 4:
            case 5:
                System.out.print("Весна");
                break;
            case 6:
            case 7:
            case 8:
                System.out.print("Лето");
                break;
            case 9:
            case 10:
            case 11:
                System.out.print("Осень");
                break;
            default:
                System.out.print("error");
        }
    }
}
```
Альтернатива:
более элегантно через тернарный.
```
import java.util.Scanner;
class Example {
	public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int a = sc.nextInt();
        if ((a<1)||(a>12)) {
            System.out.println("error");
        } else {
            System.out.println(a < 3? "Зима": a < 6? "Весна": a < 9? "Лето":  a < 12? "Осень":"Зима");
        }
    }
}
```
##### Задача 
На вход подаются координаты точки x, y. Определите, попадает ли точка в заштрихованную область.
![alt](/img/%D0%9E%D0%B1%D0%BB%D0%B0%D1%81%D1%82%D1%8C.png)
Выведите "Yes", если попадает, и "No" - в противном случае.

Примечание. Считать, что граница принадлежит заштрихованной области.

Sample Input:

-0.5
0.5
Sample Output:

Yes
##### Решение
Сканер два дабла, и всего 2 варианта на выбор.
```
import java.util.*;
class Example1{
    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        double x =sc.nextDouble();
        double y =sc.nextDouble();

        if (x >= 0 && y <= 2-x*x && y >=0 || x < 0 && y >= x && y <=2-x*x) {
            System.out.println("Yes");
        } else {
            System.out.println("No");
        }
    }
}
```
##### Задача 
Богатейшие люди Земли решили создать тайное мировое правительство  ̶и̶ ̶у̶п̶р̶а̶в̶л̶я̶т̶ь̶ ̶п̶л̶а̶н̶е̶т̶о̶й̶,̶ ̶н̶е̶ ̶п̶р̶и̶в̶л̶е̶к̶а̶я̶ ̶в̶н̶и̶м̶а̶н̶и̶я̶ ̶с̶а̶н̶и̶т̶а̶р̶о̶в̶. В кабинет совещаний могут войти только те, кто указан в специальном списке: Джефф Безос, Илон Маск,  Марк Цукерберг, Билл Гейтс. Чтобы получить допуск, нужно сказать фразу-приветствие. Если фраза-приветствие содержит имя из списка, проход разрешается. Если же нет - проход блокируется.

На ввод подаётся фраза-приветствие. Выведите "Добро пожаловать!", если имя есть в списке, и "Здесь никого нет, Вы ошиблись дверью" - если нет.

Примечание. Буква "ё".

Sample Input 1:

Это я, Билл Гейтс
Sample Output 1:

Добро пожаловать!
Sample Input 2:

Открывай, Абрамович пришёл!
Sample Output 2:

Здесь никого нет, Вы ошиблись дверью
##### Решение
Довольно простое задание.
```
import java.util.*;
class Example1{
    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        String a =sc.nextLine(); sc.close();
        String b = "Джефф Безос", c = "Илон Маск", d = "Марк Цукерберг", f = "Билл Гейтс";
        System.out.println((a.contains(b) || a.contains(c) || a.contains(d) || a.contains(f)) ? "Добро пожаловать!":"Здесь никого нет, Вы ошиблись дверью");
    }
}
```
##### Задача 
На вход подаётся слово. Выведите словами количество букв в этом слове. Если букв больше пяти - выведите "Длинное слово". 

Sample Input:

в
Sample Output:

Одна буква
##### Решение
Через свитч, ищем ленг стринга сканера.
```
import java.util.*;
class Example1{
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String a = sc.nextLine();
        int b = a.length();

        switch (b) {

            case 0:
                System.out.println("Ноль букв");
                break;
            case 1:
                System.out.println("Одна буква");
                break;
            case 2:
                System.out.println("Две буквы");
                break;
            case 3:
                System.out.println("Три буквы");
                break;
            case 4:
                System.out.println("Четыре буквы");
                break;
            case 5:
                System.out.println("Пять букв");
                break;
            default:
                System.out.println("Длинное слово");
        }


    }
}
```
Альтернатива:    
Сокращённый свитч.
```
import java.util.Scanner;
class Example {
	public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
        String w = input.next();
        input.close();
        switch (w.length()) {
            case 1: System.out.print("Одна буква"); break;
            case 2: System.out.print("Две буквы"); break;
            case 3: System.out.print("Три буквы"); break;
            case 4: System.out.print("Четыре буквы"); break;
            case 5: System.out.print("Пять букв"); break;
            default: System.out.print("Длинное слово");
}}}
```
---
### 4 Циклы     

#### 4.1 While

##### Задача 
На вход подаётся натуральное число n. Выведите на печать числа от единицы до введённого числа включительно, каждое на новой строке.

Sample Input:

5
Sample Output:

1
2
3
4
5
##### Решение
Инт со сканера, инт равный 1 точка отчёта, цикл while в условие точка отчёта польше или равно инту со сканера в теле саут точка отчета инкремент точка отчёта.
```
import java.util.Scanner;
class MyNumber {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int a = sc.nextInt();
        int b = 1;
        while (b <= a){
            System.out.println(b);
            b++;
        }
    }
}
```
##### Задача 
На ввод подаётся натуральное число n. Выведите на печать в возрастающем порядке через пробел квадраты натуральных чисел, если эти квадраты не превышают n.

Sample Input:

30
Sample Output:

1 4 9 16 25
##### Решение
Сканер считывает число и заводит в переменную а, i точка отчёта равна 1, rezult = 1 это инт в который будет выводиться по указаным правилам Math.pow(i,2) во второй степени.Вайл в условии результат меньше или равно a .В теле вайла i++ то есть 1 во второй степени, 2 во второй и т.д.
```
import java.util.Scanner;
class MyNumber {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int a = sc.nextInt();
        int i = 1;
        int rezult = 1;
        while (rezult <= a){
            i++;
            System.out.print(rezult+" ");
            rezult = (int) Math.pow(i,2);
        }
    }
}
```
Альтернативное решение:    
Более краткое.
В n число со сканера(30), а - точка отчёта равная единице, Условие вайл перемножаеться точка отчёта a меньше или равно n. Тело{ саут точка перемножаеться a инкремент} , потом 2 перемножаеться проходит через условие и также в сауте.
```
import java.util.*;
class MyNumber {
    public static void main(String[] args) {
        int n = new Scanner(System.in).nextInt(), a = 1;
        while (a * a <= n){
            System.out.print(a * a + " ");
            a++;
        }
    }
}
```
##### Задача 
Считайте со ввода последовательность целых чисел. Последовательность оканчивается числом 0.

Выведите на печать сумму введённых чисел.

Sample Input:

1 2 3 4 5 0
Sample Output:

15
##### Решение
Импортируем сканер, создаём 2 переменные рез = 0 и а = (без разницы) в цикле в неё будут поступать данные со сканера. Вайл условие (a=сканер) не равное нулю. В теле каждое цисло введённое кроме нуля плюсуеться в rez. При окончание цикла саут рез.
```
import java.util.*;
class MyNumber {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int rez = 0;
        int a = 1;
        while ((a=sc.nextInt()) != 0){
        rez +=a;
        }
        System.out.print(rez);
    }
}
```
Альтернативное решение: 
Всё в цикле.
```
import java.util.Scanner;
class MyNumber {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
        int sum = 0, n;
        while ((sum+=n=input.nextInt())*n!=0);
        input.close();
        System.out.print(sum);
}}
```

##### Задача
На вход подаётся последовательность слов. Посчитайте общее количество введённых слов.

Примечание. Так как маркер конца последовательности в этой задаче отсутствует, будет удобно воспользоваться методом hasNext(). Найдите самостоятельно, как он работает.

Sample Input:

Java
Python
C++
Go
PHP
Sample Output:

5
##### Решение
Пока не будет введена пустая строка, счётчик не остановиться и саут не пройдёт.
```
import java.util.Scanner;
class MyNumber {
    public static void main(String[] args) {
        Scanner in=new Scanner(System.in);

        int x=0;

        while ( in.nextLine().isEmpty() == false) {x++;}

        System.out.print(x);
    }
}
```
Альтернативное решение ( которое прошло на степике)
В идее саут не выводиться.
```
import java.util.Scanner;
class MyNumber {
    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);
        int count = 0;
        while (sc.hasNext()) {
            String word = sc.next();
            count++;
        }
        System.out.print(count);
    }}
```
##### Задача
Завершите программу таким образом, чтобы она вывела числа от 1 до 5, каждое на новой строке.

Sample Input:

Sample Output:

1
2
3
4
5
```
class MyTest {
    public static void main(String[] args) {
        int x = 1;
        do {
            System.out.println(x);
            x++;
        } 
    }
}
```
##### Решение
После закрытия do, пишем while x<=5.
```
class MyTest {
    public static void main(String[] args) {
        int x = 1;
        do {
            System.out.println(x);
            x++;
        } while (x<=5);
    }
}
```
##### Задача
На вход подаются числа, которые делятся на 11. Концом последовательности будет любое число, не делящееся на 11 (это число не входит в последовательность).

Посчитайте количество введённых чисел и сумму тех из них, которые кратны 3.

Sample Input:

11 22 33 121 99 15
Sample Output:

5
132
##### Решение
Создаём сканер, и 3 нулевых инта. a это ввод с консоли, count счетчик введёных чисел, sum это сумма чисел кратных 3. 
Далее вайл условие (Число с консоли  делиться на 11 без остатка), в тело каунт++, проверка если а делиться на 3 без остатка то, а плюсуеться в sum. sout count и sum.
```
import java.util.Scanner;
class MyTest {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int a = 0;
        int count = 0, sum = 0;

        while ((a=sc.nextInt()) % 11== 0 ){
                count++;
             if (a% 3 == 0){
                sum+= a;
            }
        }
        System.out.println(count);
        System.out.println(sum);
    }
}
```
Альтернативное решение с break и пояснениями.
```
import java.util.Scanner;                      // импорт модуля сканера

class MyTest {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);   // ввод сканера sc
        int x = sc.nextInt();                 // считать первое значение
        int count = 0;                       // переменная счетчика чисел
        int summ = 0;                       // переменная сложения 
        while (x % 11 == 0)                // цикл пока х делиться на 11
        {
            count++;                     // прибавляем к счетчику +1
            if (x % 3 == 0)             // если число делиться также на 3
            {
                summ = summ + x;      // складываем число с суммой таких чисел
            }
            x = sc.nextInt();       // вводим новое значение с консоли
            if (x % 11 != 0)       // проверяем число на делимость на 11
            {
                break;           // если не делиться останавливаем цикл
            }
        } 
        
        System.out.println(count);     // вывод результата количества чисел последовательности
        System.out.println(summ);     // вывод результата сложения чисел делящихся на 3
    }
}
```

##### Задача
На вход подаётся последовательность чисел от нуля до 10, являющихся рейтингами фильма, выставленными зрителями. Если входящее число отрицательное или больше 10, последовательность прерывается.

Посчитайте среднюю оценку фильма. 

Sample Input:

5 6 7 8 9 10 11
Sample Output:

7.5
##### Решение
Всё как и в прошлом задании только вместо интов даблы, и убираем ифы, саут сумма деленная на каунт.
```
import java.util.Scanner;
class MyTest {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        double a = 0;
        double count = 0, sum = 0;
        while ((a=sc.nextInt()) >= 0 && a<11){
            count++;sum+= a;
        }
        System.out.println(sum/count);
    }
}
```

##### Задача
На вход подаётся натуральное число. Выведите на печать составляющие его цифры в обратном порядке.

Sample Input:

12345
Sample Output:

54321
##### Решение
Сканер принимает стринг, инт б равен длинне символов стринга а (-1), по сути цикл от большего к меньшему включая 0 выводит индексы строки .
```
import java.util.Scanner;
class MyTest {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String a = sc.nextLine();
        int b = a.length() -1;
        do {
            System.out.print(a.charAt(b));
            b--;
        } while (b>=0);
    }
}
```
Альтернативные решения:
C помощью метода reserve()
```
import java.util.Scanner;
class MyNumber {
    public static void main(String[] args) {
        String num = new Scanner(System.in).nextLine();
        System.out.print(new StringBuilder(num).reverse());
    }
}
```
Через массив и цикл for.
```
import java.util.Scanner;

class MyNumber {
    public static void main(String[] args) {
        Scanner in = new Scanner(System.in);
        String str = in.nextLine();
        char[] arr = str.toCharArray();
        for(int i = arr.length - 1; i >= 0; i--) {
            System.out.print(arr[i]);
        }
    }
}
```
##### Задача
На вход подаётся строка с двумя буквами, а затем - строка, состоящая из слов. Выведите на печать все слова, которые начинаются на буквы, идущие по алфавиту между буквами с первой строки (включительно). Вывести слова необходимо в том же порядке, в котором они подаются на вход.

Sample Input:

j p
java python c++ kotlin php sql http css javascript r go
Sample Output:

java
python
kotlin
php
javascript
##### Решение
Сканер принимает 2 стринга сразу переводим их в инты CharAt, вайл принимаем слова в условии sc.hasNext(), в теле пишем стринг принимающий слова и условие вывода в данном примере (если первая буква стринга больше или равна a1 и меньше или равна b1) то выводим в саут. В примере задачки это слова начинающиеся на j,k,l,m,n,o,p .

---

### 4.2 Цикл for
##### Задача
Завершите программу таким образом, чтобы она напечатала "Отлично!" 10 раз.

Sample Input:

Sample Output:

Отлично!
Отлично!
Отлично!
Отлично!
Отлично!
Отлично!
Отлично!
Отлично!
Отлично!
Отлично!
```
class MyNumber {
    public static void main(String[] args) {
        ___ (int i = 0; i _ 10; ___) {
            System.out.println("_______");
    }
}
```
##### Решение
Прописываем цикл for, в условии  i <10, инкремент.соут отлично и закрываем тело цикла скобкой.
```
class MyNumber {
    public static void main(String[] args) {
        for (int i = 0; i < 10; i++) {
            System.out.println("Отлично!");
        }
    }}
```
##### Задача
Cколько раз выполнится цикл:

for (int i = 2; i < 50; i = i * i) {
    System.out.println(i);
}
##### Решение
Три раза, сначал i = 2, это меньше 50, дальше перемножаем, 4, 16. 16*16 больше 50, цикл заканчиваеться.
##### Задача
На вход подаётся натуральное число n. Выведите на печать в одной строке через пробел все числа от 1 до n включительно, которые одновременно без остатка делятся на 2 и на 3. Если таких чисел в диапазоне нет, выведите "Таких чисел нет".

Sample Input 1:

1
Sample Output 1:

Таких чисел нет
Sample Input 2:

20
Sample Output 2:

6 12 18
##### Решение
сканер 2 инта, первый получает цисло со сканера и отдаёт в цикл, а второй в роли счётчика. For в условие прописываем число больше или равно со сканера. проверка на кратность 2 и 3. и проверка на то что бы если нет кратных то вывод "Таких чисел нет".
```
import java.util.Scanner;
class MyNumber {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int a = sc.nextInt(), b = 0;
        for (int i = 1; i <= a; i++) {
            if (i%2==0 && i%3==0){
                b++;
                System.out.print(i+" ");
            }
        } if (b == 0){
            System.out.println("Таких чисел нет");
        }
    }}
```
Альтернативное решение:
c boolean  
```
import java.util.Scanner;

class MyProgram {
	public static void main(String[] args) {
		Scanner in = new Scanner(System.in);
        int n = in.nextInt();
        boolean flag = false;
        for (int i = 1; i <= n; i++) {
            if (i % 2 == 0 && i % 3 == 0) {
                System.out.print(i + " ");
                flag = true;
            }
        }
        if (flag != true)
            System.out.println("Таких чисел нет");
    }
}
```

##### Задача
##### Решение

##### Задача
##### Решение

##### Задача
##### Решение

##### Задача
##### Решение

##### Задача
##### Решение

##### Задача
##### Решение