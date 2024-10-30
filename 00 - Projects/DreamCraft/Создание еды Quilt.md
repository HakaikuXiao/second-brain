---
modified: 2024-10-05T21:33:45+06:00
---
В целом тоже что и просто предмет за исключением того что базовый класс предмета мы дополняем свойством "еда".
```java
public static final Item TEST_FOOD = new Item(new QuiltItemSettings().food(  
    new FoodComponent.Builder()  
       .hunger(50)  
       .saturationModifier(1)  
       .snack()  
       .meat()  
       .build()  
));
```
