❤️ Drawing a Heart with ColabTurtle

This project demonstrates how to use ColabTurtle
, a Python graphics library, to draw a simple heart shape in red inside Google Colab.

The script moves the turtle across the canvas step by step, combining arcs and straight lines to form a heart.

🖼️ Example Output

When executed, the code produces a red heart drawn on an 800x500 canvas.

🚀 Getting Started
1. Install ColabTurtle

If you are using Google Colab, install ColabTurtle by running:

´´!pip install ColabTurtle´´

2. Import and Initialize

´´from ColabTurtle.Turtle import *

initializeTurtle(initial_speed=4, initial_window_size=(800,500))´´

You said:
 wrote a code that uses ColabTurtle to draw a heart in red. Make a markdown Readme that explains it

initializeTurtle(initial_speed=4, initial_window_size=(800,500))

color('red')
speed(10)
penup()
goto(300, 250)
pendown()

## First concave
for i in range(9):
    forward(17)
    right(20)
penup()
left(90+70)
pendown()
## Second concave
for i in range(10):
    forward(17)
    right(20)
## First Line of the triangle
right(10)
forward(120)
left(-80)
forward(120)
left(-35)
forward(17)


penup()
goto(200, 250)
pendown()
ChatGPT said:

Here’s a clean README.md draft for your heart-drawing project with ColabTurtle:

❤️ Drawing a Heart with ColabTurtle

This project demonstrates how to use ColabTurtle
, a Python graphics library, to draw a simple heart shape in red inside Google Colab.

The script moves the turtle across the canvas step by step, combining arcs and straight lines to form a heart.

🖼️ Example Output

When executed, the code produces a red heart drawn on an 800x500 canvas.

🚀 Getting Started
1. Install ColabTurtle

If you are using Google Colab, install ColabTurtle by running:

!pip install ColabTurtle

2. Import and Initialize
from ColabTurtle.Turtle import *

initializeTurtle(initial_speed=4, initial_window_size=(800,500))

📜 Code Walkthrough

´´color('red')         # Set pen color to red
speed(10)            # Increase drawing speed
penup()              # Lift pen to move without drawing
goto(300, 250)       # Move turtle to starting position
pendown()            # Start drawing
´´

Drawing the Heart

First concave arc
The loop draws the first curved lobe of the heart:

´´for i in range(9):
    forward(17)
    right(20)´´


Second concave arc
After rotating the turtle, a second arc is drawn:

´´penup()
left(90+70)
pendown()
for i in range(10):
    forward(17)
    right(20)´´


Triangle base
The straight lines complete the bottom of the heart:

´´right(10)
forward(120)
left(-80)
forward(120)
left(-35)
forward(17)


Optional repositioning
Finally, the turtle can be moved elsewhere:

´´penup()
goto(200, 250)
pendown()´´

🎯 Result

Running the full script produces a red heart shape centered in the canvas, made from two arcs at the top and a triangular base.

🧑‍💻 Author

Made with 💖 using Python and ColabTurtle.
