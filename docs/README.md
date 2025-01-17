# Solution:
## Added functions for calculating the area and perimeter of shapes: circle, rectangle, square, triangle

# Description of functions:
## Circle:
```python
import math

def area(r):
return math.pi * r * r

def perimetr(r):
return 2 * math.pi * r
```
- Importing the math library for working with pi

```python
import math
```
- The function for calculating the area takes the number **r** - the radius of the circle for further calculation of the area of ​​the circle

```python
def area(r):
```
- Returns the area of a circle


```python
return math.pi * r * r
```
- The function for calculating the perimeter of a circle takes the number **r** - the radius of the circle to calculate the perimeter of the circle

```python
def perimetr(r):
```
- The program returns the perimeter of the circle
```python
return 2 * math.pi * r
```

### Example call:
```python
import math

def area(r):
    return math.pi * r * r

def perimetr(r):
    return 2 * math.pi * r

int r = 5
print(area(r))
print(perimetr(r))
```
## Rectangle
```python
def area(a, b):
    return a * b

def perimetr(a, b):
    return 2 * (a + b)
```
- Takes two numbers: a and b - the length and width of the rectangle to calculate its area

```python
def area(a, b):
```
- Returns the area of a rectangle

```python
return a * b
```
- The function for calculating the perimeter takes two numbers: a and b - the length and width of the rectangle to calculate its perimeter
```python
def perimetr(a, b):
```
- Returns the perimeter of a rectangle
```python
return 2 * (a + b)
```
### Example call:
```python
def area(a, b):
    return a * b

def perimetr(a, b):
    return 2 * (a + b)

int a = 5
int b = 6
print(area(a, b))
print(perimetr(a, b))
```
## Square
```python
def area(a):
    return a * a

def perimetr(a):
    return 4 * a
```
- The function for calculating the area takes the number a - the side of the square to calculate its area
```python
def area(a):
```
- Returns the area of a square

```python
return a * a
```
- The function for calculating the perimeter takes the number a - the side of the square to calculate its perimeter

```python
def perimetr(a):
```
- Returns the perimetr of a square
```python
return 4 * a
```
### Example call:
```python
def area(a):
    return a * a

def perimetr(a):
    return 4 * a

int a = 10
print(area(a))
print(perimetr(a))
```
## Triangle
```python
def area(a, h):
    return a * h / 2

def perimetr(a, b, c):
    return a + b + c
```
- The function for calculating the area takes two numbers: a and h - the side and height of the triangle to calculate its area

```python
def area(a, h):
```
- Returns the area of a triangle

```python
return a * h / 2
```
- The function for calculating the perimeter takes three numbers: a, b, c - sides of the triangle
```python
def perimetr(a, b, c):
```
- Returns the perimetr of a triangle
```python
return a + b + c
```
### Example call:
```python
def area(a, h):
    return a * h / 2

def perimetr(a, b, c):
    return a + b + c

int a = 5
int b = 4
int c = 3
int h = 2
print(area(a, h))
print(perimetr(a, b, c))
```
### Unit Tests
#### Rectangle
|  Type of Operation  |      Tests Name      | Input Data |  Excepted Result  |         Result          |
|:-------------------:|:--------------------:|:----------:|:-----------------:|:-----------------------:|
|        Area         |    area_testcases    |    10 2     |        20         | $${\color{green}True}$$ |
|      Perimetr       |  perimetr_testcases  |    a 2     |     TypeError     | $${\color{green}True}$$ |            
|        Area         |    area_testcases    |   -3 10    |    ValueError     | $${\color{green}True}$$ |         

#### Triangle
| Type of Operation |      Tests Name      | Input Data | Excepted Result |         Result          |
|:-----------------:|:--------------------:|:----------:|:---------------:|:-----------------------:|
|       Area        |    area_testcases    |   7 8      |       28        | $${\color{green}True}$$ |
|     Perimetr      |  perimetr_testcases  |   a b c    |    TypeError    | $${\color{green}True}$$ |            
|     Perimetr      |  perimetr_testcases  |  -23 1 4   |   ValueError    | $${\color{green}True}$$ |    

#### Square
| Type of Operation |      Tests Name      | Input Data | Excepted Result |         Result          |
|:-----------------:|:--------------------:|:----------:|:---------------:|:-----------------------:|
|       Area        |    area_testcases    |     a      |    TypeError    | $${\color{green}True}$$ |
|     Perimetr      |  perimetr_testcases  |    100     |       400       | $${\color{green}True}$$ |            
|       Area        |    area_testcases    |     -2     |   ValueError    | $${\color{green}True}$$ |         

#### Circle
| Type of Operation |      Tests Name      | Input Data | Excepted Result |         Result          |
|:-----------------:|:--------------------:|:----------:|:---------------:|:-----------------------:|
|       Area        |    area_testcases    |     5      |     10 * pi     | $${\color{green}True}$$ |
|     Perimetr      |  perimetr_testcases  |     p      |    TypeError    | $${\color{green}True}$$ |            
|       Area        |    area_testcases    |    1000    | 1000000 * $\pi$ | $${\color{green}True}$$ |         



# Project change history with commit hashes
> commit 6f8689d1df655ec46153baf42b798d81b7a75f1a (HEAD -> main)
- | Author: Taras <nebarrow@yandex.ru>
- | Date:   Thu Nov 16 21:47:18 2023 +0300

- |    A bug in README.md has been fixed

>commit e5e2156488367bbc0afe1b270d6078bd25cbf590 (origin/main, origin/HEAD)
- | Author: Taras <nebarrow@yandex.ru>
- | Date:   Thu Nov 16 19:08:25 2023 +0300

- |    An error with markup in readme.md has been fixed


> commit e5e2156488367bbc0afe1b270d6078bd25cbf590
- | Author: Taras <nebarrow@yandex.ru>
- | Date:   Thu Nov 16 19:08:25 2023 +0300

- |    An error with markup in readme.md has been fixed

> commit d0a91108c8311bf647287e9782c3cdb2fc442bad
- | Author: Taras <nebarrow@yandex.ru>
- | Date:   Thu Nov 16 18:39:12 2023 +0300

- |    The tests.py file has been added and the README.md has been updated

> commit e9f3a1a982e7c4a33b7c02e3d0d31cb51a0dbb81
- | Author: Taras <nebarrow@yandex.ru>
- | Date:   Sat Sep 30 22:09:11 2023 +0300

- |     The docs directory appeared in the project structure, which contains documentation on the project written in markdown notation

> commit 895de6d4ac25263a47e41d7919260685826c7e5b
- | Author: Taras <nebarrow@yandex.ru>
- | Date:   Mon Sep 18 19:12:37 2023 +0300
- |
- |     была исправлена ошибка в вычислении периметра прямоугольника в файле rectangle.py.


> commit b441342a4b0460f0e1c6895932e64ee43f4d07c5
- | Author: Taras <nebarrow@yandex.ru>
- | Date:   Mon Sep 18 19:08:11 2023 +0300
- |
- |     был добавлен новый файл rectangle.py с вычислениями для фигуры Прямоугольник


> commit d078c8d9ee6155f3cb0e577d28d337b791de28e2
-  | Author: smartiqa <info@smartiqa.ru>
-  | Date:   Thu Mar 4 14:55:29 2021 +0300
-  |
-  |     L-03: Docs added
 
