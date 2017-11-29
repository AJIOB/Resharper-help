## Рефакторинг "Выделение класса" (Extract class)

Для выделения интерфейса щелкните правой клавишей мыши по имени любого из требуемых методов и выберите `Refactor->Extract->Extract Class`

![pic1](pictures/extract_class/1.png)

Получите такое окно:

![pic1](pictures/extract_class/2.png)

В нем требуется указать имя нового класса и выбрать методы для извлечения. 

**Небольшой лайфхак:** если начать писать имя извлекаемого класса (Extracted class), то поле "Reference to extracted" заполнится автоматически в соответствии с настройками Resharper для имени поля класса.

После заполнения получаем:

![pic1](pictures/extract_class/3.png)

Нажимаем "Next", смотрим результат:

![pic1](pictures/extract_class/4.png)

