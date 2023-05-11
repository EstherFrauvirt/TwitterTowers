# TwitterTowers
This program presents the user with a menu offering two options: Option 1 and Option 2. The user can continue selecting options until choosing to exit the program by selecting Option 3.

Program Architecture
The program follows an object-oriented approach with the following classes:

Abstract Class: Shape
This abstract class represents a generic shape.
It contains the following methods:
printScope(): Calculates and returns the perimeter of the shape.
set_dimensions(height, width): Sets the height and width of the shape.
run(): Abstract method that will be implemented by subclasses to provide specific functionality.
Class: Rectangle (inherits from Shape)
This class represents a rectangular tower.
It inherits from the Shape abstract class.
It implements the run() method to either print the area or perimeter of the rectangle based on the difference between its sides.
Class: Triangle (inherits from Shape)
This class represents a triangular tower.
It inherits from the Shape abstract class.
It implements the run() method to either perform a calculation or print the triangle based on the user's choice.
Main Program Flow
The user selects an option from the menu: Option 1 (Rectangular Tower), Option 2 (Triangular Tower), or Option 3 (Exit Program).
Depending on the user's choice, the program creates an instance of the corresponding class: Rectangle or Triangle.
The program prompts the user to enter the height and width of the tower.
The instance of the class receives the dimensions through the scan() method.
The program calls the run() method of the instantiated class.
The run() method performs specific actions based on the chosen option:
For Rectangle:
If the difference between the sides is greater than 5, it prints the area of the rectangle.
Otherwise, it prints the perimeter of the rectangle.
For Triangle:
If the user chooses the Triangular Calculation option, it performs the calculation and prints the result.
If the user chooses the Printing the Triangle option, it checks the conditions:
If the width is even or longer than 2 times the height, it prints a message that the triangle cannot be printed.
If the width is odd and shorter than twice the height, it prints the triangular shape according to the specified pattern.
After executing the chosen action, the program returns to the menu, and the user can select another option.
