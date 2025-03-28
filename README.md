### Документация по доступным модулям и методам

### Модуль `blocks`
Содержит константы, представляющие различные блоки в Minecraft. Каждый блок также имеет числовой идентификатор (ID), который можно использовать вместо констант.

#### Доступные блоки и их ID:

| Константа               | ID  | Описание                          |
|-------------------------|-----|-----------------------------------|
| `AIR`                   | 0   | Воздух                            |
| `BEDROCK`               | 7   | Каменная порода                   |
| `BEDROCK_INVISIBLE`     | 95  | Невидимая каменная порода         |
| `BOOKSHELF`             | 47  | Книжная полка                     |
| `BRICK_BLOCK`           | 45  | Кирпичный блок                    |
| `CACTUS`                | 81  | Кактус                            |
| `CLAY`                  | 82  | Глина                             |
| `COAL_ORE`              | 16  | Угольная руда                     |
| `COBBLESTONE`           | 4   | Булыжник                          |
| `COBWEB`                | 30  | Паутина                           |
| `CRAFTING_TABLE`        | 58  | Верстак                           |
| `DIAMOND_BLOCK`         | 57  | Алмазный блок                     |
| `DIAMOND_ORE`           | 56  | Алмазная руда                     |
| `DIRT`                  | 3   | Земля                             |
| `DOOR_IRON`             | 71  | Железная дверь                    |
| `DOOR_WOOD`             | 64  | Деревянная дверь                  |
| `FARMLAND`              | 60  | Возделанная земля                 |
| `FENCE`                 | 85  | Забор                             |
| `FENCE_GATE`            | 107 | Калитка забора                    |
| `FIRE`                  | 51  | Огонь                             |
| `FLOWER_RED`            | 38  | Красный цветок                    |
| `FLOWER_YELLOW`         | 37  | Желтый цветок                     |
| `GLASS`                 | 20  | Стекло                            |
| `GLASS_PANE`            | 102 | Стеклянная панель                 |
| `GLOWSTONE_BLOCK`       | 89  | Светящийся камень                 |
| `GOLD_BLOCK`            | 41  | Золотой блок                      |
| `GOLD_ORE`              | 14  | Золотая руда                      |
| `GRASS`                 | 2   | Трава                             |
| `GRASS_TALL`            | 31  | Высокая трава                     |
| `GRAVEL`                | 13  | Гравий                            |
| `HAY_BLOCK`             | 170 | Сено                              |
| `ICE`                   | 79  | Лед                               |
| `IRON_BLOCK`            | 42  | Железный блок                     |
| `IRON_ORE`              | 15  | Железная руда                     |
| `LADDER`                | 65  | Лестница                          |
| `LAPIS_LAZULI_BLOCK`    | 22  | Блок лазурита                     |
| `LAPIS_LAZULI_ORE`      | 21  | Лазуритовая руда                  |
| `LAVA`                  | 10  | Лава                              |
| `LAVA_FLOWING`          | 10  | Текущая лава                      |
| `LAVA_STATIONARY`       | 11  | Неподвижная лава                  |
| `LEAVES`                | 18  | Листья                            |
| `MELON`                 | 103 | Арбуз                             |
| `MOSS_STONE`            | 48  | Мшистый камень                    |
| `MUSHROOM_BROWN`        | 39  | Коричневый гриб                   |
| `MUSHROOM_RED`          | 40  | Красный гриб                      |
| `OBSIDIAN`              | 49  | Обсидиан                          |
| `REDSTONE_ORE`          | 73  | Редстоуновая руда                 |
| `SAND`                  | 12  | Песок                             |
| `SANDSTONE`             | 24  | Песчаник                          |
| `SAPLING`               | 6   | Саженец                           |
| `SNOW`                  | 78  | Снег                              |
| `SNOW_BLOCK`            | 80  | Снежный блок                      |
| `STAIRS_COBBLESTONE`    | 67  | Каменные ступени                  |
| `STAIRS_WOOD`           | 53  | Деревянные ступени                |
| `STONE`                 | 1   | Камень                            |
| `STONE_BRICK`           | 98  | Каменный кирпич                   |
| `STONE_SLAB`            | 44  | Каменная плита                    |
| `STONE_SLAB_DOUBLE`     | 43  | Двойная каменная плита            |
| `SUGAR_CANE`            | 83  | Сахарный тростник                 |
| `TNT`                   | 46  | Динамит                           |
| `TORCH`                 | 50  | Факел                             |
| `WATER`                 | 9   | Вода                              |
| `WATER_FLOWING`         | 8   | Текущая вода                      |
| `WATER_STATIONARY`      | 9   | Неподвижная вода                  |
| `WOOD`                  | 17  | Дерево                            |
| `WOOD_PLANKS`           | 5   | Деревянные доски                  |
| `WOOL`                  | 35  | Шерсть                            |

#### Пример использования с ID:

```python
import mc

# Установка блока земли на позицию (0, 0, 0) с использованием ID
mc.world.setBlock(0, 0, 0, 3)  # 3 - это ID блока земли (DIRT)
```

```python
import mc

# Установка блока земли на позицию (0, 0, 0)
mc.world.setBlock(0, 0, 0, mc.blocks.DIRT)
```

#### 2. Модуль `colors`
Содержит константы, представляющие цвета.

**Доступные цвета:**
- `BLACK`, `BLUE`, `BROWN`, `CYAN`, `GRAY`, `GREEN`, `LIGHT_BLUE`, `LIGHT_GRAY`, `LIME`, `MAGENTA`, `ORANGE`, `PINK`, `PURPLE`, `RED`, `WHITE`, `YELLOW`

**Пример использования:**
```python
import mc

# Установка блока шерсти красного цвета
mc.world.setBlock(0, 0, 0, mc.blocks.WOOL, mc.colors.RED)
```

#### 3. Модуль `creatures`
Содержит константы, представляющие различных существ и сущностей в Minecraft.

**Доступные существа:**
- `BAT`, `BOAT`, `CHICKEN`, `COW`, `DONKEY`, `DRAGON_FIREBALL`, `EGG`, `FIREBALL`, `HORSE`, `IRON_GOLEM`, `LIGHTNING`, `LLAMA`, `MINECART`, `MINECART_CHEST`, `MINECART_FURNACE`, `MINECART_TNT`, `MULE`, `MUSHROOM_COW`, `OCELOT`, `PARROT`, `PIG`, `POLAR_BEAR`, `PRIMED_TNT`, `RABBIT`, `SHEEP`, `SMALL_FIREBALL`, `SNOWBALL`, `SNOWMAN`, `SPLASH_POTION`, `SQUID`, `VILLAGER`, `WOLF`

**Пример использования:**
```python
import mc

# Создание коровы на позиции (10, 0, 10)
mc.world.spawnCreature(10, 0, 10, mc.creatures.COW)

mc.world.spawnCreature(10, 0, 10, "COW")
```

#### 4. Модуль `directions`
Содержит константы, представляющие направления.

**Доступные направления:**
- `BACK`, `DOWN`, `EAST`, `FORWARD`, `LEFT`, `NORTH`, `RIGHT`, `SOUTH`, `UP`, `WEST`

**Пример использования:**
```python
import mc

# Поворот игрока на север
mc.player.lookTo(mc.directions.NORTH)
# Другой способ, можно передать строку в параметр
mc.player.lookTo("NORTH")
```

# 5. Модуль `drones`
Содержит классы и функции для управления дронами.

## Основные функции

### `createDrone(x, y, z, name)`

Создает дрона с указанными координатами и именем.

- **Параметры:**
  - `x`, `y`, `z` — координаты начального положения дрона.
  - `name` — уникальное имя дрона.
- **Возвращает:** объект дрона.

**Пример:**

```python
drone = drones.createDrone(0, 0, 0, "Игорь")
print(drone.getPos())  # [0, 0, 0]
```

### `getDrone(name)`

Возвращает объект дрона по его имени.

- **Параметры:**
  - `name` — имя дрона.
- **Возвращает:** объект дрона или `None`, если дрон не найден.

**Пример:**

```python
drone = drones.getDrone("Игорь")
if drone:
    print("Дрон найден!")
else:
    print("Дрон не найден!")
```

### `list()`

Возвращает список всех активных дронов.

- **Возвращает:** массив с именами дронов.

**Пример:**

```python
drone_names = drones.list()
print(drone_names)  # ["Игорь", "Андрей"]
```

### `removeDrone(name)`

Удаляет дрона с указанным именем.

- **Параметры:**
  - `name` — имя дрона.
- **Возвращает:** `true`, если дрон удалён, иначе `false`.

**Пример:**

```python
success = drones.removeDrone("Игорь")
print(success)  # True
```

### `removeAll()`

Удаляет всех дронов.

- **Возвращает:** `true`, если все дроны удалены, иначе `false`.

**Пример:**

```python
success = drones.removeAll()
print(success)  # True
```

---

## Методы дрона

### Перемещение и поворот

#### `moveForward(distance)`

Перемещает дрона вперёд на указанное количество блоков.

**Пример:**

```python
drone.moveForward(5)
```

#### `move(direction, distance)`

Перемещает дрона в указанном направлении.

**Пример:**

```python
drone.move("NORTH", 3)
```

#### `lookTo(direction)`

Поворачивает дрона в указанном направлении.

**Пример:**

```python
drone.lookTo("EAST")
```

#### `turn(pitch, yaw)`

Поворачивает дрона на указанные углы.

**Пример:**

```python
drone.turn(30, 90)
```

#### `turnLeft()` и `turnRight()`

Поворачивает дрона на 90 градусов.

**Пример:**

```python
drone.turnLeft()
drone.turnRight()
```

---

### Взаимодействие с блоками

#### `breakBlock()`

Разрушает блок перед дроном.

**Пример:**

```python
success = drone.breakBlock()
print(success)  # True
```

#### `placeBlock(type)`

Устанавливает блок перед дроном.

**Пример:**

```python
drone.placeBlock("stone")
```

#### `getBlockInFront()`

Возвращает тип блока перед дроном.

**Пример:**

```python
block = drone.getBlockInFront()
print(block)  # "stone"
```

---

### Инвентарь

#### `getInventory()`

Возвращает содержимое инвентаря дрона.

**Пример:**

```python
inventory = drone.getInventory()
print(inventory)
```

#### `inventoryContains(item)`

Проверяет наличие предмета в инвентаре.

**Пример:**

```python
has_item = drone.inventoryContains("stone")
print(has_item)  # True
```

#### `pickItem([material])`

Подбирает предмет в инвентарь.

**Пример:**

```python
drone.pickItem(["stone"])
```

#### `dropItem(material, amount)`

Выбрасывает предмет из инвентаря.

**Пример:**

```python
drone.dropItem("stone", 1)
```

---

### Другие методы

#### `getPos()`

Возвращает текущие координаты дрона.

**Пример:**

```python
pos = drone.getPos()
print(pos)  # [x, y, z]
```

#### `destroy()`

Уничтожает дрона.

**Пример:**

```python
drone.destroy()
```

#### `shootArrow()`

Стреляет из лука.

**Пример:**

```python
drone.shootArrow()
```

---

## Пример использования

```python
# Создание дрона
drone = drones.createDrone(0, 0, 0, "Игорь")

# Перемещение и поворот
drone.moveForward(5)
drone.turnRight()

# Взаимодействие с блоками
drone.placeBlock("stone")
block_type = drone.getBlockInFront()
print(block_type)

# Работа с инвентарём
drone.pickItem(["stone"])
drone.dropItem("stone", 1)

# Уничтожение дрона
drone.destroy()
```


# 6. Модуль `entity`
Содержит методы для работы с сущностями.

**Доступные методы:**
- `getDirection()`
- `getPitch()`
- `getPos()`
- `getRotation()`
- `sendCommand()`
- `setPos()`
- `setVelocity()`

**Пример использования:**
```python
import mc

# Получение позиции сущности
pos = mc.entity.getPos()
print(pos)
```

#### 7. Модуль `items`
Содержит константы, представляющие различные предметы.

**Доступные предметы:**
- `BONE_MEAL`, `CARROT`, `COAL`, `DIAMOND`, `EGG`, `EMERALD`, `GOLD_INGOT`, `IRON_INGOT`, `POTATO`, `REDSTONE`, `REEDS`, `WHEAT`, `WHEAT_SEEDS`

**Пример использования:**
```python
import mc

# Выдача алмаза игроку
mc.player.sendCommand(f"give @p {mc.items.DIAMOND}")
```

#### 8. Модуль `particles`
Содержит константы, представляющие различные частицы.

**Доступные частицы:**
- `CRIT_MAGIC`, `DRIP_WATER`, `ENCHANTMENT_TABLE`, `FLAME`, `HEART`, `NOTE`, `REDSTONE`, `VILLAGER_ANGRY`, `VILLAGER_HAPPY`

**Пример использования:**
```python
import mc

# Создание частиц огня на позиции (0, 0, 0)
mc.world.sendCommand(f"particle {mc.particles.FLAME} 0 0 0")
```

#### 9. Модуль `player`
Содержит методы для управления игроком.

**Доступные методы:**
- `getDirection()`
- `getPitch()`
- `getPos()`
- `getRotation()`
- `lookTo()`
- `move()`
- `sendCommand()`
- `setPos()`
- `turnLeft()`
- `turnRight()`

**Пример использования:**
```python
import mc

# Перемещение игрока вперед
mc.player.move(mc.directions.FORWARD)
```

#### 10. Модуль `rails`
Содержит константы, представляющие различные типы рельсов.

**Доступные рельсы:**
- `ASCENDING_EAST`, `ASCENDING_NORTH`, `ASCENDING_SOUTH`, `ASCENDING_WEST`, `EAST_WEST`, `NORTH_EAST`, `NORTH_SOUTH`, `NORTH_WEST`, `SOUTH_EAST`, `SOUTH_WEST`

**Пример использования:**
```python
import mc

# Установка рельсов на позицию (0, 0, 0)
mc.world.setBlock(0, 0, 0, mc.blocks.RAIL, mc.rails.EAST_WEST)
```

#### 11. Модуль `util`
Содержит вспомогательные функции.

**Доступные методы:**
- `postToChat()`
- `sendCommand()`

**Пример использования:**
```python
import mc

# Отправка сообщения в чат
mc.util.postToChat("Привет, Minecraft!")
```

#### 12. Модуль `weather`
Содержит константы, представляющие различные погодные условия.

**Доступные погодные условия:**
- `CLEAR`, `DOWNFALL`

**Пример использования:**
```python
import mc

# Установка ясной погоды
mc.world.setWeather(mc.weather.CLEAR)
```

#### 13. Модуль `world`
Содержит методы для управления миром.

**Доступные методы:**
- `buildArc()`
- `buildColumn()`
- `buildHome()`
- `buildSphere()`
- `buildWall()`
- `getBlock()`
- `getBlockData()`
- `getBlocks()`
- `getHeight()`
- `getPlayerId()`
- `getPlayerIds()`
- `sendCommand()`
- `setBlock()`
- `setBlocks()`
- `setCuboid()`
- `setTime()`
- `setWeather()`
- `spawnCreature()`

**Пример использования:**
```python
import mc

# Установка блока земли на позицию (0, 0, 0)
mc.world.setBlock(0, 0, 0, mc.blocks.DIRT)
```
