---
modified: 2024-10-05T23:01:07+06:00
---

В общих чертах процесс схож с созданием предмета в Quilt.
```java
public class TestItemsAndBlocks {  
    public static Item register(Item item, String id) {  
        if (item == null) {  
            throw new IllegalArgumentException("item cannot be null");  
        }        if (id == null) {  
            throw new IllegalArgumentException("id cannot be null");  
        }        Identifier itemID = Identifier.of(DreamCraftExtras.MOD_ID, id);  
        return Registry.register(Registries.ITEM, itemID, item);  
    }  
    public static final Item TEST_ITEM = register(  
            new Item(new Item.Settings()),  
            "test_item"  
    );  
  
    public static void initialize() {  
    }}
```