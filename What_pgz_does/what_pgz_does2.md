# Pygame Zero - frantic activity behind the scenes

Pygame Zero projects use two special Python *functions* to create the graphics - ```draw()``` and ```update()```.

## Function ```draw()```

When you run your Python project using Pygame Zero, Pygame Zero looks in your code for a function called ```draw()```. If it finds this function it *automatically* runs it, without you having to *call* the function (as you would in normal Python code).

What's more Pygame Zero doesn't just run this function *once* - it **keeps** running it over and over again (as many as 60 times a second) until you kill the programme. This function is used to keep redrawing the graphics window and allows you to *animate* objects in your project. The ```draw()``` function should contain all the code that actually draws things in the graphics window.

Here is an example of a function called ```draw()``` which will display a letter A in the graphics window, with its centre at coordinates given by the variables ```x_coord``` and ```y_coord```:

```python
def draw():
    screen.draw.text('A', center=(x_coord, y_coord))
```

## Function ```update()```

At the same time that Pygame Zero looks for a function called ```draw()``` it *also* looks for a function called ```update()```. If it finds this function it will run it repeatedly just ***before*** running function ```draw()```.

Function ```update()``` should contain code to do with ***changing*** the positions or appearances of the items to be drawn on the screen. An example of an update function is:

```python
def update():
    global x_coord
    x_coord += 1
```

Each time this function is run it will increase the value of the global variable ```x_coord``` by 1. In combination with the draw function shown above it would cause the letter A to change its x coordinate each time the function runs, so it would look as if the letter was moving to the right across the graphics window.

## How to use these and other Pygame Zero functions

There are a host of special Pygame Zero functions you can use to create and move objects to make your project really exciting. You can find a list of these functions on the Pygame Zero website at

[https://pygame-zero.readthedocs.io/en/latest/builtins.html](https://pygame-zero.readthedocs.io/en/latest/builtins.html)

Some of these look rather complicated, so to get used to some of these functions have a look at the project on this github called [Letter A](../../../../LetterA/README.md) which goes through the process of making a Pygame Zero game in very simple steps.

You can look at a simple programme written to use Pygame Zero at [letterA1.py](letterA1.py)
