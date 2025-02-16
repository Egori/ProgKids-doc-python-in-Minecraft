### Документация по доступным модулям и методам

#### 1. Модуль `blocks`
Содержит константы, представляющие различные блоки в Minecraft.

**Доступные блоки:**
- `AIR`, `BED`, `BEDROCK`, `BEDROCK_INVISIBLE`, `BOOKSHELF`, `BRICK_BLOCK`, `CACTUS`, `CHEST`, `CLAY`, `COAL_ORE`, `COBBLESTONE`, `COBWEB`, `CRAFTING_TABLE`, `DIAMOND_BLOCK`, `DIAMOND_ORE`, `DIRT`, `DOOR_IRON`, `DOOR_WOOD`, `FARMLAND`, `FENCE`, `FENCE_GATE`, `FIRE`, `FLOWER_RED`, `FLOWER_YELLOW`, `FURNACE_ACTIVE`, `FURNACE_INACTIVE`, `GLASS`, `GLASS_PANE`, `GLOWSTONE_BLOCK`, `GOLD_BLOCK`, `GOLD_ORE`, `GRASS`, `GRASS_TALL`, `GRAVEL`, `HAY_BLOCK`, `ICE`, `IRON_BLOCK`, `IRON_ORE`, `LADDER`, `LAPIS_LAZULI_BLOCK`, `LAPIS_LAZULI_ORE`, `LAVA`, `LAVA_FLOWING`, `LAVA_STATIONARY`, `LEAVES`, `MELON`, `MOSS_STONE`, `MUSHROOM_BROWN`, `MUSHROOM_RED`, `OBSIDIAN`, `REDSTONE_ORE`, `SAND`, `SANDSTONE`, `SAPLING`, `SNOW`, `SNOW_BLOCK`, `STAIRS_COBBLESTONE`, `STAIRS_WOOD`, `STONE`, `STONE_BRICK`, `STONE_SLAB`, `STONE_SLAB_DOUBLE`, `SUGAR_CANE`, `TNT`, `TORCH`, `WATER`, `WATER_FLOWING`, `WATER_STATIONARY`, `WOOD`, `WOOD_PLANKS`, `WOOL`

**Пример использования:**
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
```

#### 4. Модуль `directions`
Содержит константы, представляющие направления.

**Доступные направления:**
- `BACK`, `DOWN`, `EAST`, `FORWARD`, `LEFT`, `NORTH`, `RIGHT`, `SOUTH`, `UP`, `WEST`

**Пример использования:**
```python
import mc

# Поворот игрока на север
mc.player.turnRight(mc.directions.NORTH)
```

#### 5. Модуль `drones`
Содержит классы и функции для управления дронами.

**Доступные методы:**
- `Drone` (класс)
- `createDrone()`
- `getDrone()`
- `list()`
- `removeAll()`
- `removeDrone()`
- `sendCommand()`

**Пример использования:**
```python
import mc

# Создание дрона и перемещение его вперед
drone = mc.drones.createDrone()
drone.move(mc.directions.FORWARD)
```

#### 6. Модуль `entity`
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
