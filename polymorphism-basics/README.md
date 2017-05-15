PolymorphismBasics.cpp - creates an inheritance hierarchy of Rodent: Mouse, Gerbil, Hamster, etc. In the base class, provides methods that are common to all Rodents, and refines these in the derived classes to perform different behaviours depending on the specific type of Rodent. Rodent is created as a pure abstract base class. Creates an array of pointers (10) to Rodent, and fills it with different specific types of Rodents. Calls the base class methods, and displays the results.

- Program Purpose:
		Introduces the C++ concepts of class hierarchies, inheritance, abstract
		functions, and polymorphism.
- Compile (assuming GNU C++ compiler): g++ PolymorphismBasics.cpp -o PolymorphismBasics
- Execution: PolymorphismBasics.exe
- Notes: No user input is necessary, everything for this program is hardcoded
Classes: 
		Rodent - a pure abstract base class, which provides methods that are common to
				all subtypes of Rodents.
		Mouse - derived from Rodent, refines each class from the base class to perform
				behaviours specific to a Mouse.
		Gerbil - derived from Rodent, refines each class from the base class to perform
				behaviours specific to a Gerbil.
		Hamster - derived from Rodent, refines each class from the base class to perform
				behaviours specific to a Hamster.
Variables:
		rp[] - Rodent* - an array of Rodent pointers which is populated with the three
			   different subtypes of Rodent to demonstrate polymorphism.
