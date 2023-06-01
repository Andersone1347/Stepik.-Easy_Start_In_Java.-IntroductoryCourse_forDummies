# Stepik.-Easy_Start_In_Java.-IntroductoryCourse_forDummies

## 2 Базовые понятия.

### Структура программы на Java

Традиционно первая программа в любом курсе - это код, выводящий на экран приветствие "Hello, World!".

Давайте сделаем это ;)

 ```

class MyClass {
    public static void main(String[] args) {
        System.out.println("Hello World");
    }
}
 ```
Выглядит довольно сложно, однако сейчас нет необходимости подробно разбираться с назначением каждой команды в этом коде. Отметим только самое важное.

Программа на Java - это совокупность объектов, которые взаимодействуют через вызов друг друга. Таким образом, на практике программа состоит из большого количества файлов с расширением .java, расположенных в каталоге программы.

Каждый файл представляет собой отдельный класс. Наименование класса должно начинаться с заглавной буквы и строго совпадать с названием файла.

Если посмотреть на пример выше, то, чтобы запустить его на компьютере, а не в песочнице Степик, нужно поместить код в файл с именем MyClass.java. Так как наша программа простая, она будет состоять всего из одного класса (файла). В больших проектах классов сотни и тысячи.


