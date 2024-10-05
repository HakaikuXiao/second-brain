---
modified: 2024-10-05T09:54:19+06:00
---
Создаем в основной папке класс предметов.
Далее первое что нужно сделать - зарегистрировать предмет. Регистры буквально основополагающая часть майнкрафт. Что угодно имеет регистр.

```java
public static final Item TEST_ITEM = new Item(new QuiltItemSettings());
```
Это предмет. Переменная хранящая его самого и его настройки.

```java
public static void register(ModContainer mod) {  
    Registry.register(Registries.ITEM, new Identifier(mod.metadata().id(), "test_item"), TEST_ITEM);  
}
```
А это сам регистр для нашего предмета. Он содержит идентификатор на основе id мода.
