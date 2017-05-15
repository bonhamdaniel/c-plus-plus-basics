InheritanceBasics.cpp - creates a class hierarchy for simple geometry. Starts with a Point class to hold x and y values of a point. Overloads the << operator to print point values, and the + and – operators to add and subtract point coordinates.Creates a pure abstract base class Shape, which forms the basis of shapes. The Shape class contains abstract functions to calculate area and circumference of the shape, plus provides the coordinates (Points) of a rectangle that encloses the shape (a bounding box). These are overloaded by the derived classes. Creates a display() function that displays the name of the class, and all stored information about the class (including area, circumference, and bounding box). Builds a hierarchy by creating the Shape classes Circle, Square, and Triangle. For these derived classes, default constructors, and constructors whose arguments can initialize the shapes appropriately using the correct number of Point objects are created.  In main(), creates one instance each of the following: Circle (10, -5) with a radius of 23; Square (5, -5)(-10,7)(4,23)(-6,12); and Triangle(0,0)(10,10)(-15,15). Displays the information from each object.

- Program Purpose:
		Introduces the C++ concepts of class hierarchies, inheritance, abstract
		functions, composition, and other related topics.
- Compile (assuming GNU C++ compiler): g++ InheritanceBasics.cpp -o InheritanceBasics
- Execution: InheritanceBasics.exe
- Notes: No user input is necessary, everything for this program is hardcoded
- Classes: 
		Point - holds x and y values of a point. Overloads the << operator to print 
				point values, and the + and – operators to add and subtract point 
				coordinates. 
		Shape (base class) - forms the basis of shapes. Contains abstract functions 
				to calculate area and circumference of the shape, plus provides the 
				coordinates (Points) of a rectangle that encloses the shape (a bounding 
				box). These are overloaded by the derived classes. Creates a display() 
				function that displays the name of the class, and all stored information 
				about the class (including area, circumference, and bounding box).
		Circle  (derived from Shape) - contains a default constructor and a constructor 
				whose arguments can initialize the circle appropriately using a Point 
				center and a radius.
		Square (derived from Shape) - contains a default constructor and a constructor 
				whose arguments can initialize the square appropriately using four 
				Point vertices.
		Triangle (derived from Shape) - contains a default constructor and a constructor 
				whose arguments can initialize the triangle appropriately using three 
				Point vertices.
Variables:
		x - int - Point class, used to store x-coordinate of a Point
		y - int - Point class, used to store y-coordinate of a Point
		center - Point - Circle class, used to store center Point of a circle
		radius - int - Circle class, used to store the radius of a circle
		pa - Point* - each derived Shape class, used to store bounding box of shape
		vertices1 - Point - Square/Triangle class, used to store 1st Point of a shape
		vertices2 - Point - Square/Triangle class, used to store 2nd Point of a shape
		vertices3 - Point - Square/Triangle class, used to store 3rd Point of a shape
		vertices4 - Point - Square class, used to store 4th Point of a square
		minX - int - Square/Triangle class, used to store the minimum x-coordinate 
				among the points that make up the shape, used to determine bounding 
				box
		maxX - int - Square/Triangle class, used to store the maximum x-coordinate 
				among the points that make up the shape, used to determine bounding 
				box
		minY - int - Square/Trisngle class, used to store the minimum y-coordinate 
				among the points that make up the shape, used to determine bounding 
				box
		maxY - int - Square/Triangle class, used to store the maximum x-coordinate 
				among the points that make up the shape, used to determine bounding box
		s1 - Point - Square/Triangle class, used to store the difference between the 1st
				and 2nd vertices, used in calculating circumference
		s2 - Point - Square/Triangle class, used to store the difference between the 2nd
				and 3rd vertices, used in calculating circumference
		s3 - Point - Square/Triangle class, used to store the difference between the 3rd
				and 4th vertices, used in calculating circumference
		s4 - Point - Square class, used to store the difference between the 4th
				and 1st vertices, used in calculating circumference
