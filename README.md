# CS2420-4.1-P4-Search-solved

Download Here: [CS2420 4.1 P4 – Search solved](https://jarviscodinghub.com/assignment/4-1-p4-search-solution/)

For Custom/Original Work email jarviscodinghub@gmail.com/whatsapp +1(541)423-7793

Search Project
Purpose
The purpose of this lab is to demonstrate the speed difference between recursive and iterative binary search and sequential search. This
difference is shown if the array size is too small Therefore. you should make your array as large as possible, and still have 2 significant
digits of output Binary search is much faster than sequential search.
Tasks
• Create a Search Class
• Member variables
o array of ints
o size of the array
o Whatever else you need
• Constructor(int size) l,’ initializes a Search Object with an internal integer array of the specified size
• Destructor // destroys all data allocated by the constructor
bool SequentiaSearch(int target) // retums true f target is found in the object’s data array
bool RecursiveBinarySearch(int target) h’ returns true if target is found in the object’s data array (recursive)
bool RecursiveginarySearchHelper(int lowlndex, int highlndex, int target) //called by RecursiveginarySearchO
• bool IterativeBinarySearch(int target) // returns true if target is found in the object’s data array
• void InitSortedA”rayO
o Function to initialize the array with sorted random numbers
o call srand(O) before initializing to get the same numbers each time
Dont use a sort() function here. Rather, when initializing, insert a number a bit larger than the previous number
Arrayli] + rand() etc
• int // returns a pointer to the array of integers
• Create a non-interactive driver that runs each of these searches and times and displays the outputs.
• Create a Search object specifying a large array size say 1,000000-
• Your timing results should be at least 2 significant digits
to get at least 2 significant digits, you may have to dispo the output in micro or nano seconds (see timer section)
• Search for (using all three types of searches)
e a number at the beginning of the sorted array
a number at the middle of the sorted array
o a number at the end ofthe sorted array
a number NOT in the array (try-I)
• Do not do any printing inside the searches.
e This will giveyou incorrect timer results.
• Display the output to do each of the different searches

Sample Output
Creating a sorted array of 10000000
Finished creating a sorted array of 10000000
Searching
for a number at the start of the array
s. sequencia1Search() returned 1 in 364ns
s. IterativeBinarySearch() returned 1 in 1459ns
s. RecursiveBinarySearch() returned 1 in 1823ns
for a number in the middle of the array
Searching
s. sequencia1Search() returned 1 in 10187113ns
s. IterativeBinarySearch() returned 1 in 1094ns
s. RecursiveBinarySearch() returned 1 in 2188ns
Searching
for a number at the end of the array
Searching
s. sequenciaISearch() returned 1 in
s. IterativeBinarySearch() returned
s. RecursiveBinarySearch() returned
for a number NOT in the array
s. sequenciaISearch() returned O in
s. IterativeBinarySearch() returned
s. RecursiveBinarySearch() returned
21273508ns
I in 2188ns
1 in 3282ns
19723286ns
e in 1458ns
e in 3282ns

Random Numbers
• Random Number generation in C/C++ is defined in the header file.
• Use void to set the random number seed. The seed can be any value, but should be the same each time (so you can
duplicate your results).
• Use “int to generate a random number from C to MAXINT
• if you need a smaller random number when initializing the array, use rand() % 20 to get a random number between C and 19.
Timer
Source code for a Timer class has been provided. You should include this class in your project to time things down to the nanc-second
level. This class was written to be portable, however, Ive not tried it in a nan-Windows/non-zyBooks environment. If it does not work for
Mac or Linux. you may have to modify the source provided. All three environments should have a •high-resolution timer’
Example
Timerti;
ti.StartO; // start the timer
// do something you want to time (dont do any “cout’s” here. They take a long time…)
usIeep(521 COO); // this should sleep for around 521 milliseconds
ti.End(); // end the timer
cout “The timed event took ” ti.DurationlnNanoSeconds() ‘ns” endl;
cout “The timed event took ” ti.DurationlnMicroSeconds() ‘us” endl;
cout “The timed event took ” ti.DurationlnMilliSeconds() “ms” endl;
You only need one Timer object for this project You can Ere-start’ him by calling tiStartO again.
Modify these files
• Main.cpp
• Search.cpp
• Search.h
