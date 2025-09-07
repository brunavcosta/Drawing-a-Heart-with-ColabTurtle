# ❤️ Drawing a Heart with ColabTurtle

This project demonstrates how to use **[ColabTurtle](https://pypi.org/project/ColabTurtle/)**, a Python graphics library, to draw a simple heart shape in red inside Google Colab.  

Two different versions of the heart are included:
- **Version 1:** A heart built with arcs and straight lines (triangle base).
- **Version 2:** A smoother heart shape built from arcs.

The script moves the turtle across the canvas step by step, combining arcs and straight lines to form a heart.

---

## 🖼️ Example Output

When executed, the code produces a **red heart** drawn on an `800x500` canvas.  

---

## 🚀 Getting Started

### 1. Install ColabTurtle  
If you are using **Google Colab**, install ColabTurtle by running:

```python
!pip install ColabTurtle
```
### 2. Import and Initialize
```python
from ColabTurtle.Turtle import *

initializeTurtle(initial_speed=4, initial_window_size=(800,500))
```

##📜 Code Walkthrough
##🔹 Version 1 – Triangle-based Heart
```python
color('red')         # Set pen color to red
speed(10)            # Increase drawing speed
penup()              # Lift pen to move without drawing
goto(300, 250)       # Move turtle to starting position
pendown()            # Start drawing

# First concave arc
for i in range(9):
    forward(17)
    right(20)

penup()
left(90+70)
pendown()

# Second concave arc
for i in range(10):
    forward(17)
    right(20)

# Triangle base
right(10)
forward(120)
left(-80)
forward(120)
left(-35)
forward(17)

# Optional repositioning
penup()
goto(200, 250)
pendown()
```
##🔹 Version 2 – Smooth Arc Heart
```python
initializeTurtle(initial_speed=4, initial_window_size=(800,500))

color('red')
speed(10)
penup()
goto(400, 250) # Start near the center
pendown()

# Adjust initial angle for 90 degrees rotation to the right
left(140 - 90) # Rotate 140 degrees to start, then add 90 degrees more

forward(111.65) # Adjust length for a better shape
for i in range(200):
    right(1)
    forward(1)

left(120)
for i in range(200):
    right(1)
    forward(1)

forward(111.65) # Adjust length

penup()
goto(400, 250) # Return to center
pendown()
```
## 🎯 Result

- Version 1 creates a stylized heart with a triangular bottom.

- Version 2 creates a smoother and rounder heart using arcs.

Both hearts are drawn in red on the 800x500 canvas.

## 🧑‍💻 Author

Made with 💖 using Python and ColabTurtle.
