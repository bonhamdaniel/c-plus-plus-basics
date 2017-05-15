TemplateBasics.cpp - uses the Standard C++ Library vector as an underlying implementation to create a Set template class that accepts only one of each type of object that is put into it. Makes a nested iterator class that supports the “end sentinel” concept. Includes test code in main(), using both the program Set template class and the Standard C++ Library set template to verify that the behaviour is correct.

- Program Purpose:
		Introduces the C++ concepts templates, iterators, nested iterators, and end sentinels.
Compile (assuming GNU C++ compiler): g++ TMA4Question3.cpp -o TMA4Question3
Execution: TMA4Question3.exe
Notes: No user input is necessary, everything for this program is hardcoded
Classes: 
		Set - template <class T> - Uses the Standard C++ Library vector as an underlying 
			 implementation, a class that accepts only one of each type of object that 
			 you put into it.
		iterator - nested in Set class, used to traverse the objects in a Set, supports
			 the "end sentinel" concept.
Variables:
		v - vector<T> - in Set, used to store the collection of objects
		s - Set& - in iterator, used to store the Set reference the iterator works on
		index - int - in iterator, used to store current position in the set while being
			manipulated by the iterator
