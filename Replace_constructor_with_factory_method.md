## Рефакторинг "Замена конструктора фабричным методом" (Replace constructor with factory method)

Исходный код:

![pic1](pictures/replace_constructor_with_factory_method/1.png)

Для замены конструктора фабричным методом щелкните правой клавишей мыши по имени требуемого конструктора в классе и выберите `Refactor->Convert->Constructor to Factory Method...`

![pic1](pictures/replace_constructor_with_factory_method/2.png)

Получите такое окно:

![pic1](pictures/replace_constructor_with_factory_method/3.png)

В нем набираем имя фабричного метода, который будет скрывать требуемый констуктор. Также можно выбрать класс, в котором этот метод нужно разместить. По умолчанию выбирается корректное имя (в соответствии с codestyle-ом языка C#), но имя метода совпадает с именем конструктора. 

Для примера дадим методу имя `Class1Factory`:

![pic1](pictures/replace_constructor_with_factory_method/4.png)

Жмем "Next" и получаем следующий код:

![pic1](pictures/replace_constructor_with_factory_method/5.png)

В данном коде требуемый конструктор переведен в категорию `private` и появился статический метод, который занимается вызовом этого конструктора и возвращением созданного объекта

P.S. Если не изменить целевой класс или имя метода в окне генерации метода, появится ошибка, которая говорит, что это имя доступно только для конструкторов и деструкторов, но при этом все равно создаст метод с требуемым именем, если нажать "Next".

![pic1](pictures/replace_constructor_with_factory_method/6.png)