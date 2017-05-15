DynamicStorage.cpp - introduces the C++ concepts of dynamic creation of storage, deleting that storage, and shows the required memory for different types.

- Program Purpose:
		Introduces the C++ concepts of dynamic creation of storage, deleting that
		storage, and shows the required memory for the different types
- Compile (assuming GNU C++ compiler): g++ DynamicStorage.cpp -o DynamicStorage
- Execution: DynamicStorage.exe
- Notes: No user input is necessary, everything for this program is hardcoded
- Classes: None
- Variables:
		- size - int - used to store a single int value that is the size for the arrays
		- ip - int* - used to store a pointer to a single int value
		- lp - long* - used to store a pointer to a single long value
		- ca - char* - used to store a pointer to a char array with 100 elements
		- fa - float* - used to store a pointer to a float array with 100 elements

Test Plan
- Normal Case 1:
		- Runs program as constituted, without any alterations
		- Should display output as required in program specification
		> int @ <5772088> = <59>
		> long @ <5772136> = <123456>
		> charArray[0] @ <5770984> = <a>
		> charArray[1] @ <5770985> = <b>
		> charArray[2] @ <5770986> = <c>
		> charArray[3] @ <5770987> = <d>
		> charArray[4] @ <5770988> = <e>
		> charArray[5] @ <5770989> = <f>
		> charArray[6] @ <5770990> = <g>
		> charArray[7] @ <5770991> = <h>
		> charArray[8] @ <5770992> = <i>
		> charArray[9] @ <5770993> = <j>
		> charArray[10] @ <5770994> = <k>
		> charArray[11] @ <5770995> = <l>
		> charArray[12] @ <5770996> = <m>
		> charArray[13] @ <5770997> = <n>
		> charArray[14] @ <5770998> = <o>
		> charArray[15] @ <5770999> = <p>
		> charArray[16] @ <5771000> = <q>
		> charArray[17] @ <5771001> = <r>
		> charArray[18] @ <5771002> = <s>
		> charArray[19] @ <5771003> = <t>
		> charArray[20] @ <5771004> = <u>
		> charArray[21] @ <5771005> = <v>
		> charArray[22] @ <5771006> = <w>
		> charArray[23] @ <5771007> = <x>
		> charArray[24] @ <5771008> = <y>
		> charArray[25] @ <5771009> = <z>
		> charArray[26] @ <5771010> = <A>
		> charArray[27] @ <5771011> = <B>
		> charArray[28] @ <5771012> = <C>
		> charArray[29] @ <5771013> = <D>
		> charArray[30] @ <5771014> = <E>
		> charArray[31] @ <5771015> = <F>
		> charArray[32] @ <5771016> = <G>
		> charArray[33] @ <5771017> = <H>
		> charArray[34] @ <5771018> = <I>
		> charArray[35] @ <5771019> = <J>
		> charArray[36] @ <5771020> = <K>
		> charArray[37] @ <5771021> = <L>
		> charArray[38] @ <5771022> = <M>
		> charArray[39] @ <5771023> = <N>
		> charArray[40] @ <5771024> = <O>
		> charArray[41] @ <5771025> = <P>
		> charArray[42] @ <5771026> = <Q>
		> charArray[43] @ <5771027> = <R>
		> charArray[44] @ <5771028> = <S>
		> charArray[45] @ <5771029> = <T>
		> charArray[46] @ <5771030> = <U>
		> charArray[47] @ <5771031> = <V>
		> charArray[48] @ <5771032> = <W>
		> charArray[49] @ <5771033> = <X>
		> charArray[50] @ <5771034> = <Y>
		> charArray[51] @ <5771035> = <Z>
		> charArray[52] @ <5771036> = <a>
		> charArray[53] @ <5771037> = <b>
		> charArray[54] @ <5771038> = <c>
		> charArray[55] @ <5771039> = <d>
		> charArray[56] @ <5771040> = <e>
		> charArray[57] @ <5771041> = <f>
		> charArray[58] @ <5771042> = <g>
		> charArray[59] @ <5771043> = <h>
		> charArray[60] @ <5771044> = <i>
		> charArray[61] @ <5771045> = <j>
		> charArray[62] @ <5771046> = <k>
		> charArray[63] @ <5771047> = <l>
		> charArray[64] @ <5771048> = <m>
		> charArray[65] @ <5771049> = <n>
		> charArray[66] @ <5771050> = <o>
		> charArray[67] @ <5771051> = <p>
		> charArray[68] @ <5771052> = <q>
		> charArray[69] @ <5771053> = <r>
		> charArray[70] @ <5771054> = <s>
		> charArray[71] @ <5771055> = <t>
		> charArray[72] @ <5771056> = <u>
		> charArray[73] @ <5771057> = <v>
		> charArray[74] @ <5771058> = <w>
		> charArray[75] @ <5771059> = <x>
		> charArray[76] @ <5771060> = <y>
		> charArray[77] @ <5771061> = <z>
		> charArray[78] @ <5771062> = <A>
		> charArray[79] @ <5771063> = <B>
		> charArray[80] @ <5771064> = <C>
		> charArray[81] @ <5771065> = <D>
		> charArray[82] @ <5771066> = <E>
		> charArray[83] @ <5771067> = <F>
		> charArray[84] @ <5771068> = <G>
		> charArray[85] @ <5771069> = <H>
		> charArray[86] @ <5771070> = <I>
		> charArray[87] @ <5771071> = <J>
		> charArray[88] @ <5771072> = <K>
		> charArray[89] @ <5771073> = <L>
		> charArray[90] @ <5771074> = <M>
		> charArray[91] @ <5771075> = <N>
		> charArray[92] @ <5771076> = <O>
		> charArray[93] @ <5771077> = <P>
		> charArray[94] @ <5771078> = <Q>
		> charArray[95] @ <5771079> = <R>
		> charArray[96] @ <5771080> = <S>
		> charArray[97] @ <5771081> = <T>
		> charArray[98] @ <5771082> = <U>
		> charArray[99] @ <5771083> = <V>
		> floatArray[0]  @ <5771096> = <101>
		> floatArray[1]  @ <5771100> = <102>
		> floatArray[2]  @ <5771104> = <103>
		> floatArray[3]  @ <5771108> = <104>
		> floatArray[4]  @ <5771112> = <105>
		> floatArray[5]  @ <5771116> = <106>
		> floatArray[6]  @ <5771120> = <107>
		> floatArray[7]  @ <5771124> = <108>
		> floatArray[8]  @ <5771128> = <109>
		> floatArray[9]  @ <5771132> = <110>
		> floatArray[10]  @ <5771136> = <111>
		> floatArray[11]  @ <5771140> = <112>
		> floatArray[12]  @ <5771144> = <113>
		> floatArray[13]  @ <5771148> = <114>
		> floatArray[14]  @ <5771152> = <115>
		> floatArray[15]  @ <5771156> = <116>
		> floatArray[16]  @ <5771160> = <117>
		> floatArray[17]  @ <5771164> = <118>
		> floatArray[18]  @ <5771168> = <119>
		> floatArray[19]  @ <5771172> = <120>
		> floatArray[20]  @ <5771176> = <121>
		> floatArray[21]  @ <5771180> = <122>
		> floatArray[22]  @ <5771184> = <123>
		> floatArray[23]  @ <5771188> = <124>
		> floatArray[24]  @ <5771192> = <125>
		> floatArray[25]  @ <5771196> = <126>
		> floatArray[26]  @ <5771200> = <127>
		> floatArray[27]  @ <5771204> = <128>
		> floatArray[28]  @ <5771208> = <129>
		> floatArray[29]  @ <5771212> = <130>
		> floatArray[30]  @ <5771216> = <131>
		> floatArray[31]  @ <5771220> = <132>
		> floatArray[32]  @ <5771224> = <133>
		> floatArray[33]  @ <5771228> = <134>
		> floatArray[34]  @ <5771232> = <135>
		> floatArray[35]  @ <5771236> = <136>
		> floatArray[36]  @ <5771240> = <137>
		> floatArray[37]  @ <5771244> = <138>
		> floatArray[38]  @ <5771248> = <139>
		> floatArray[39]  @ <5771252> = <140>
		> floatArray[40]  @ <5771256> = <141>
		> floatArray[41]  @ <5771260> = <142>
		> floatArray[42]  @ <5771264> = <143>
		> floatArray[43]  @ <5771268> = <144>
		> floatArray[44]  @ <5771272> = <145>
		> floatArray[45]  @ <5771276> = <146>
		> floatArray[46]  @ <5771280> = <147>
		> floatArray[47]  @ <5771284> = <148>
		> floatArray[48]  @ <5771288> = <149>
		> floatArray[49]  @ <5771292> = <150>
		> floatArray[50]  @ <5771296> = <151>
		> floatArray[51]  @ <5771300> = <152>
		> floatArray[52]  @ <5771304> = <153>
		> floatArray[53]  @ <5771308> = <154>
		> floatArray[54]  @ <5771312> = <155>
		> floatArray[55]  @ <5771316> = <156>
		> floatArray[56]  @ <5771320> = <157>
		> floatArray[57]  @ <5771324> = <158>
		> floatArray[58]  @ <5771328> = <159>
		> floatArray[59]  @ <5771332> = <160>
		> floatArray[60]  @ <5771336> = <161>
		> floatArray[61]  @ <5771340> = <162>
		> floatArray[62]  @ <5771344> = <163>
		> floatArray[63]  @ <5771348> = <164>
		> floatArray[64]  @ <5771352> = <165>
		> floatArray[65]  @ <5771356> = <166>
		> floatArray[66]  @ <5771360> = <167>
		> floatArray[67]  @ <5771364> = <168>
		> floatArray[68]  @ <5771368> = <169>
		> floatArray[69]  @ <5771372> = <170>
		> floatArray[70]  @ <5771376> = <171>
		> floatArray[71]  @ <5771380> = <172>
		> floatArray[72]  @ <5771384> = <173>
		> floatArray[73]  @ <5771388> = <174>
		> floatArray[74]  @ <5771392> = <175>
		> floatArray[75]  @ <5771396> = <176>
		> floatArray[76]  @ <5771400> = <177>
		> floatArray[77]  @ <5771404> = <178>
		> floatArray[78]  @ <5771408> = <179>
		> floatArray[79]  @ <5771412> = <180>
		> floatArray[80]  @ <5771416> = <181>
		> floatArray[81]  @ <5771420> = <182>
		> floatArray[82]  @ <5771424> = <183>
		> floatArray[83]  @ <5771428> = <184>
		> floatArray[84]  @ <5771432> = <185>
		> floatArray[85]  @ <5771436> = <186>
		> floatArray[86]  @ <5771440> = <187>
		> floatArray[87]  @ <5771444> = <188>
		> floatArray[88]  @ <5771448> = <189>
		> floatArray[89]  @ <5771452> = <190>
		> floatArray[90]  @ <5771456> = <191>
		> floatArray[91]  @ <5771460> = <192>
		> floatArray[92]  @ <5771464> = <193>
		> floatArray[93]  @ <5771468> = <194>
		> floatArray[94]  @ <5771472> = <195>
		> floatArray[95]  @ <5771476> = <196>
		> floatArray[96]  @ <5771480> = <197>
		> floatArray[97]  @ <5771484> = <198>
		> floatArray[98]  @ <5771488> = <199>
		> floatArray[99]  @ <5771492> = <200>
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
		The program creates an int, a long, an array of 100 chars, and an array of
		100 floats and displays the address and value for each data element.
		The char array is fileed with alternating copies of the lowercase and
		uppercase alphabet, while the float array contains sequential numbers from
		101 to 200.
		After all required information has been displayed, all data is deleted.
