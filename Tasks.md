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
