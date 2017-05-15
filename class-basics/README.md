ClassBasics.cpp - creates a Text class that contains a string object to hold the text of a file. Gives it two constructors: a default constructor, and a constructor that takes a string argument that is the name of the file to open. When the second constructor is used, the file is opened and the contents of the file read into the string member object. A member function contents() returns the string so that it can be displayed. In main(), a file is opened using Text, and displays the contents.

- Program Purpose:
		Introduces the C++ concepts of classes, multiple constructors, member data and member 
		functions, and the use of a class to perform file manipulation.
- Compile (assuming GNU C++ compiler): g++ ClassBasics.cpp -o ClassBasics
- Execution: ClassBasics.exe
- Notes: No user input is necessary, everything for this program is hardcoded
- Classes: 
	- Text - contains a string variable - fileInput - which stores the file that the class
			   will manipulate.  Also contains a contents() member function, a default constructor, 
			   and a constructor that accepts a string argument (name of file to be manipulated).
- Variables:
	- fileInput - string - member data from Text class, used to store name of file the 
				class will manipulate
	- inFile - ifstream  - in Text constructor, used to open/manipulate specified file
	- line - string - in Text constructor, used to read contents of the file and store it in
			   the Text member data fileInput
	- text - instance of Text class - used to store an instance of the Text class
	- contents - string - in main, holds the contents returned by the contents() member
			   function of the Text class

Test Plan
