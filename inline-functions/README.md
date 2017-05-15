InlineFunctions.cpp - creates a const whose value is determined at runtime by reading the time when the program starts. In a separate function, creates two arrays of 10 000 doubles. Initializes the first array with sequential integral values starting with 100, and initializes the second array with the same numbers, but in reverse order.  Loops through both arrays using a single loop, multiplying the corresponding array elements from each array together, and displays the result. Reads the time when the program completes the multiplication, then computes and displays the elapsed time. Uses inline functions.

- Program Purpose:
		Introduces the C++ concepts of inline functions, consts, the ctime library and 
		its functions, and timing the execution of a program.
Compile (assuming GNU C++ compiler): g++ TMA3Question2.cpp -o TMA3Question2
Execution: TMA3Question2.exe
Notes: No user input is necessary, everything for this program is hardcoded
Classes: 
		ExecutionTime - contains all variables/functions (defined below) necessary for the program
Variables:
		sequentialArray - double array - used in ExecutionTime class to store
					10,000 sequential values starting with 100
		reverseArray - double array - used in the ExecutionTime class to store 10,000
					numbers in reverse order from 10,099 and down
		startTime - const time_t  - used in ExecutionTime class to store the time the program begins
		endTime - time_t - used in ExecutionTime class to store the time the program completes
					its computation
