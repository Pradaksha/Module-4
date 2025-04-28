# Exp.No:19  
## CLASS AND OBJECTS - AREA OF CIRCLE

### AIM  
To write a Python program to take the radius from the user and find the area of a circle using the class name `umbrella` and function name `rain`.

### ALGORITHM

1. Begin the program.

2. Create a class named `umbrella`.

3. Define a method `rain(self, r)` inside the class `umbrella` that accepts a radius `r` as an argument.
    
4. Inside the `rain` method:  
   - Calculate the area of a circle using the formula:  
     \[ \text{Area} = \pi \times r^2 \]  
   - Use the `math.pi` constant to get the value of π and perform the calculation.  
   - Print the result, formatted to two decimal places.
     
5. Prompt the user for an integer input to represent the radius of the circle.

6. Create an instance of the `umbrella` class and store it in the variable `u`.
   
8. Call the `rain` method of the `umbrella` class, passing the user-provided radius `r` as an argument.
   
10. Terminate the program.


### PROGRAM

```
# Reg.No-212223020020
# Name-Pradaksha V
import math
class umbrella():
    def __init__(self , radius):
        self.radius=radius
    def rain(self):
        return math.pi*(self.radius**2)
        
r=int(input())
obj=umbrella(r)
print("Area of circle:",round(obj.rain(),2))

```

### OUTPUT
![image](https://github.com/user-attachments/assets/f8814aa4-647a-4848-9e41-4d4b404d7041)

### RESULT
The program calculates the area of the circle and displays the result formatted to two decimal places.


