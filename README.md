# **Project Title: 5.2-lab-Program-Painting a wall**

This is a project to write  Python code to determine the cost of the painting a wall.

## **Getting Started**

These instructions will install Pycharm on your local machine for experimentation.

### **Prerequisites**

Python requires Pycharm 2020.1.1 to run, with no additional packages. This URL to download and install the Pycharm.

```
[Pycharm](https://www.jetbrains.com/pycharm/download/#section=windows)
```

**Running**

Once downloaded you can run the program by:

```
Click on the next several times and then install.
```
Click on the Pycharm icon to open the program.
Right click on "file" to Great new project.
Right click on the project that you just did then 'new' then choose 'Python file'.

**copy and past the following codes:**

```
python 5.2program Painting a wall-lab.py 
```
import math

# Dictionary of paint colors and cost per gallon
paint_colors = {
   'red': 35,
   'blue': 25,
   'green': 23
}

# FIXME (1): Prompt user to input wall's width
# Calculate and output wall area
wall_height = int(input('Enter wall height (feet):\n'))
wall_width = int(input('Enter wall width (feet):\n'))
wall_area = wall_height * wall_width
print('Wall area:', wall_area,'square feet')
   
# FIXME (2): Calculate and output the amount of paint in gallons needed to paint the wall
gallon = 350
paint_needed = wall_area / 350
print('Paint needed: ''{:.2f}'.format(paint_needed),'gallons')
# FIXME (3): Calculate and output the number of 1 gallon cans needed to paint the wall, rounded up to nearest integer
cans_needed = math.ceil(paint_needed)
print('Cans needed:', cans_needed,'can(s)')
print()
# FIXME (4): Calculate and output the total cost of paint can needed depending on color
print('Choose a color to paint the wall:')


userColor = input()
if userColor in paint_colors:
    price = paint_colors[userColor]
    totalPrice = price * cans_needed
    print('Cost of purchasing', userColor, 'paint: $%d' % totalPrice)

## **Thanks**
