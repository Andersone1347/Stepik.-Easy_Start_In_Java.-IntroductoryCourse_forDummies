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