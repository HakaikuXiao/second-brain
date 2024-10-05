---
modified: 2024-10-05T10:43:09+06:00
---
Все еще похоже на создание предмета, но кроме этого еще и включает создание блока(что довольно логично).

```java
public class DCETestBlock {  
    public static final Block TEST_BLOCK = new Block(QuiltBlockSettings.create());  
  
    public static void register(ModContainer mod) {  
       Registry.register(Registries.BLOCK, new Identifier(mod.metadata().id(), "test_block"), TEST_BLOCK);  
       Registry.register(Registries.ITEM, new Identifier(mod.metadata().id(), "test_block"),  
          new BlockItem(TEST_BLOCK, new QuiltItemSettings()));  
  
    }}
```