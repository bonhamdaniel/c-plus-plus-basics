OperatorOverloading.cpp - creates a simple class (DoStuff) containing an int, and overloads the operator+ as a member function. Also, provides a print() member function that takes an ostream& as an argument and prints to that ostream&. Adds a binary operator- and operator+ to the class as member functions. Allows use of the objects in complex expressions such as a + b – c. Adds the operator++ and operator--, both prefix and postfix versions. Overloads the << operator to provide the same functionality as the print() member function.

- Program Purpose:
		Introduces the C++ concept of operator overloading.
- Compile (assuming GNU C++ compiler): g++ TMA3Question3.cpp -o TMA3Question3
Execution: TMA3Question3.exe
Notes: No user input is necessary, everything for this program is hardcoded
Classes: 
		DoStuff - contains all necessary elements to fulfill the program description
Variables:
		i - int - used to store the int that is operated on by all the member functions
