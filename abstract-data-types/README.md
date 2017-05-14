DVDRentals.cpp - introduces the C++ concepts of abstract data types, as well as the data and operations associated with the data type, through the implementation of a DVD rental system.

- Program Purpose:
		Introduces the C++ concepts of abstract data types, as well as the data and
		operations associated with the data type.
- Compile (assuming GNU C++ compiler): g++ DVDRentals.cpp -o DVDRentals
- Execution: DVDRentals.exe
- Notes: No user input is necessary, everything for this program is hardcoded
- Classes: None
- Variables:
		- title - string - used to store the title of a DVD
		- rating - string - used to store the rating of a DVD
		- length - float - used to store the length of a DVD
		- genre - string - used to store the genre of a DVD
		- type - string - used to store the type of a DVD
		- price - float - used to store the price of a DVD
		- status - string - used to store the rental status of a DVD
		- customer - string - used to store the current rental customer of a DVD
		- dueDate - string - used to store the due date for a DVD rental
		- barcode - long - used to store the barcode of a DVD
		- dvds - a 10 element array of the abstract data type DVD - used to store all
			   associated information/operations for each individual DVD
		- file - ifstream - used to store the file that will be opened which contains
			   test data for the program

Test Plan
- Normal Case 1:
		- Runs program as constituted, without any alterations
		- Should display output as required in program specification:
			First, displays data loaded from test file
			Second, tests various functions (rent() and return()) for handling
			correct and incorrect usage
			Third, displays dvd info after manipulations to show they have been
			reflected in the underlying data structure
		> Title: Addicted
		> Rating: R
		> Length: 1.75 hrs
		> Genre: Drama
		> Type: New
		> Price: $2.99
		> Status: In-stock
		> Customer: N/A
		> Due Date: N/A
		> Barcode: 48295730

		> Title: Predestination
		>Rating: R
		>Length: 1.6 hrs
		> Genre: Action
		> Type: New
		> Price: $2.99
		> Status: Rented
		> Customer: BonhamD
		> Due Date: 02/15/2015
		> Barcode: 93681304

		> Title: Fury
		> Rating: R
		> Length: 2.2 hrs
		> Genre: Action
		> Type: New
		> Price: $2.99
		> Status: In-stock
		> Customer: N/A
		> Due Date: N/A
		> Barcode: 73591279

		> Title: Lucy
		> Rating: R
		> Length: 1.5 hrs
		> Genre: Action
		> Type: New
		> Price: $2.99
		> Status: Rented
		> Customer: SmithJ
		> Due Date: 02/17/2015
		> Barcode: 98765498

		> Title: Boyhood
		> Rating: R
		> Length: 2.8 hrs
		> Genre: Drama
		> Type: New
		> Price: $2.99
		> Status: Rented
		> Customer: DoeJ
		> Due Date: 02/16/2015
		> Barcode: 78912843

		> Title: Laggies
		> Rating: R
		> Length: 1.7 hrs
		> Genre: Comedy
		> Type: New
		> Price: $2.99
		> Status: Rented
		> Customer: BrownS
		> Due Date: 02/12/2015
		> Barcode: 45678765

		> Title: Alexander
		> Rating: PG
		> Length: 1.4 hrs
		> Genre: Family
		> Type: New
		> Price: $2.99
		> Status: In-stock
		> Customer: N/A
		> Due Date: N/A
		> Barcode: 43564728

		> Title: Brave
		> Rating: PG
		> Length: 1.6 hrs
		> Genre: Family
		> Type: Standard
		> Price: $1.99
		> Status: Rented
		> Customer: BrowningK
		> Due Date: 02/19/2015
		> Barcode: 32123465

		> Title: Dracula
		> Rating: R
		> Length: 1.5 hrs
		> Genre: Action
		> Type: Standard
		> Price: $1.99
		> Status: In-stock
		> Customer: N/A
		> Due Date: N/A
		> Barcode: 87980934

		> Title: Divergent
		> Rating: PG-13
		> Length: 2.3 hrs
		> Genre: Adventure
		> Type: Standard
		> Price: $1.99
		> Status: Rented
		> Customer: HanningL
		> Due Date: 02/18/2015
		> Barcode: 65676567

		> Dracula has been rented.

		> Sorry, Divergent is not currently in-stock.

		> Brave is now in-stock.

		> Sorry, Alexander is already in-stock.

		> Title: Addicted
		> Rating: R
		> Length: 1.75 hrs
		> Genre: Drama
		> Type: New
		> Price: $2.99
		> Status: In-stock
		> Customer: N/A
		> Due Date: N/A
		> Barcode: 48295730

		> Title: Predestination
		> Rating: R
		> Length: 1.6 hrs
		> Genre: Action
		> Type: New
		> Price: $2.99
		> Status: Rented
		> Customer: BonhamD
		> Due Date: 02/15/2015
		> Barcode: 93681304

		> Title: Fury
		> Rating: R
		> Length: 2.2 hrs
		> Genre: Action
		> Type: New
		> Price: $2.99
		> Status: In-stock
		> Customer: N/A
		> Due Date: N/A
		> Barcode: 73591279

		> Title: Lucy
		> Rating: R
		> Length: 1.5 hrs
		> Genre: Action
		> Type: New
		> Price: $2.99
		> Status: Rented
		> Customer: SmithJ
		> Due Date: 02/17/2015
		> Barcode: 98765498

		> Title: Boyhood
		> Rating: R
		> Length: 2.8 hrs
		> Genre: Drama
		> Type: New
		> Price: $2.99
		> Status: Rented
		> Customer: DoeJ
		> Due Date: 02/16/2015
		> Barcode: 78912843

		> Title: Laggies
		> Rating: R
		> Length: 1.7 hrs
		> Genre: Comedy
		> Type: New
		> Price: $2.99
		> Status: Rented
		> Customer: BrownS
		> Due Date: 02/12/2015
		> Barcode: 45678765

		> Title: Alexander
		> Rating: PG
		> Length: 1.4 hrs
		> Genre: Family
		> Type: New
		> Price: $2.99
		> Status: In-stock
		> Customer: N/A
		> Due Date: N/A
		> Barcode: 43564728

		> Title: Brave
		> Rating: PG
		> Length: 1.6 hrs
		> Genre: Family
		> Type: Standard
		> Price: $1.99
		> Status: In-stock
		> Customer: N/A
		> Due Date: N/A
		> Barcode: 32123465

		> Title: Dracula
		> Rating: R
		> Length: 1.5 hrs
		> Genre: Action
		> Type: Standard
		> Price: $1.99
		> Status: Rented
		> Customer: BonhamD
		> Due Date: 02/20/2015
		> Barcode: 87980934

		> Title: Divergent
		> Rating: PG-13
		> Length: 2.3 hrs
		> Genre: Adventure
		> Type: Standard
		> Price: $1.99
		> Status: Rented
		> Customer: HanningL
		> Due Date: 02/18/2015
		> Barcode: 65676567
		**All output as expected
***As this program is completely hardcoded, there is no user input at all, there are no
further cases to test.  The above demonstrates that the program works as required.  I
saw a discussion in the course forums which stated for this type of programs simply
running the normal case was adequate.
Discussion:
		As this is an introductory assignment, much of the C++ functionality to 
		write an elegant program, with adequate error-handling, has not yet been
		introduced.  As such, this program is completely hard-coded and does not
		contain error-handling capabilities.
		The program creates an abstractdata type - DVD - which includes all the 
		relevant data and operations necessary to implement the program.
		A file of test information is read into the program to populate a 10 element
		array of DVDs.
		The information for all 10 DVDs is displayed, followed by manipulations (both
		correct and incorrect) of some of the underlying data, after which the info for
		all DVDs is redisplayed to show the data has been correctly handled.