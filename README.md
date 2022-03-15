# Welcome to LB Calculator

A small calculator project which made by LingBlack.

### The advantage of LB Calculator
* Calculate quadratic equation in standard form easily
* Free and open source

### The disadvantage of LB Calculator
* The codes have lots of areas that need to improve
* Only support quadratic equation in standard form only

# API

### `LBCalculator.Quad({a, b, c, NumberType, Return})`
Formula: `ax^2 + bx + c`
`a` is the leading coefficient of the quadratic equation.

`b` is the second coefficient of the quadratic equation.

`c` is the third coefficient of the quadratic equation and the y-intercept of the parabola.

`NumberType` has two types. They're `Normal` and `Fraction`. `Normal` number type will return the integer/decimal as a result of the quadratic equation. `Fraction` number type will return the fraction as a result of the quadratic equation.

`Return` is the result that you want the function to pass. Currently, there've three types of `Return` in this module. Those're `x`, `y` and `Vertex`. Literally, `x` refers to the x-intercept of the vertex. `y` refers to the y-intercept of the vertex. `Vertex` is just the `x` and `y`.

### Example:
```lua
local RS = game:GetService("ReplicatedStorage")

-- < Modules > --
local LBCalculator = require(RS:FindFirstChild("LBCalculator"))

-- < Variables < --
local Test1, Test2 = LBCalculator.Quad({
	a = 1, 
	b = 2, 
	c = 3,
	NumberType = "Normal",
	Return = "Vertex",
})

print(Test1, Test2)
```

### Output:
```lua
-1  2
```
