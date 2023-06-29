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