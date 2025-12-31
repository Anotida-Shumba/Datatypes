### Datatypes 

# Vector 2

#### The vec2 datatype provides a table that has two values, an x and a y. This table contains functions that make handling vectors easier.
#### Several metamethods have also been paired witht his table to allow for arithmatic operations with vectors.

### Instantiation

```lua
local position = Vec2.new(10, 10)
```

### Spreading Values
```lua
function Vec2:spread()
    return self.x, self.y
end

local x, y = position.spread()
```

### Addition

```lua
local position_1 = Vec2.new(100, 100)
local position_2 = Vec2.new(300, 200)
local result = position_1 + position_2

--the result of this operation returns a Vec2 with the value [400, 300]
```

### Subtraction

```lua
local position_1 = Vec2.new(100, 100)
local position_2 = Vec2.new(300, 200)
local result = position_1 - position_2

--the result of this operation returns a Vec2 with the value [-200, -100]
```

### Multiplication

```lua
local position_1 = Vec2.new(10, 10)
local position_2 = Vec2.new(3, 2)
local result = position_1 * position_2

--the result of this operation returns a Vec2 with the value [30, 20]

--however with multiplication you can multiply the vector by a single number
local result = position_1 * 5
--the result of this operation now returns [10 * 5, 10 * 5]
```

### Division

```lua
local position_1 = Vec2.new(10, 10)
local position_2 = Vec2.new(5, 2)
local result = position_1 / position_2

--the result of this operation returns a Vec2 with the value [2, 5]

--however same as multiplication you can divide the vector by a single number
local result = position_1 / 5
--the result of this operation now returns [10 * 5, 10 * 5]
