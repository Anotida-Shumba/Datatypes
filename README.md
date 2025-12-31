### Datatypes 

# Vector 2

#### The vec2 datatype provides a table that has two values, an x and a y. This table contains functions that make handling vectors easier.
#### Several metamethods have also been paired witht his table to allow for arithmatic operations with vectors.

Instantiation

```lua
    local position = Vec2.new(10, 10)
```

The spread() function returns the x and the y
```lua
function Vec2:spread()
    return self.x, self.y
end
```

Addition

