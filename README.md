# Impledge-Fresher

# Compound Word Finder

## Overview
The Compound Word Finder program identifies the longest and second-longest compounded words from an input file containing a list of alphabetically sorted words. A compounded word is defined as a word that can be constructed by concatenating two or more shorter words from the same list.

This solution has been implemented in Java to ensure correctness, performance, and scalability for large word lists.



## Features
1. **Input File Processing**:
   - Reads alphabetically sorted word lists from input files (`Input_01.txt` or `Input_02.txt`).
   - Files are expected to be located at:
     - `C:\Users\ajayp\OneDrive\Documents\Downloads\Input_01.txt`
     - `C:\Users\ajayp\OneDrive\Documents\Downloads\Input_02.txt`

2. **Output Results**:
   - Longest compounded word.
   - Second-longest compounded word.
   - Time taken to process the file (in milliseconds).

3. **Efficient Algorithm**:
   - Uses a combination of sorting, hashing, and recursion to identify compounded words efficiently

## Setup Instructions

### Prerequisites
- **Java Development Kit (JDK)** installed on your system.

### Steps to Run
1. **Save the Source Code**:
   - Save the provided Java files (`CompoundWordFinder.java`) to your local system.
2. **Compile the Program**:
   - Open a terminal or command prompt.
   - Navigate to the directory containing `CompoundWordFinder.java`.
   - Run:
   
     javac CompoundWordFinder.java
     ```
3. **Run the Program**:
   - For Problem 1 (Input_01.txt):
     ```
     java CompoundWordFinder
     ```
   - For Problem 2 (Input_02.txt):
     Edit the file path in the source code to:
     ```
     String filePath = "C:\\Users\\ajayp\\OneDrive\\Documents\\Downloads\\Input_02.txt";
     ```
     Recompile and run the program.

---

## Program Details
### Design Decisions
1. **Sorting**:
   - Words are sorted by length to ensure shorter words are evaluated before longer words.
2. **Hash Set**:
   - Used for efficient look-up operations.
3. **Recursive Function**:
   - Checks if a word can be broken down into smaller words present in the list.
4. **Timing**:
   - The processing time is calculated using `System.currentTimeMillis()`.

### Output Example
For `Input_01.txt`:

Longest Compound Word: ratcatdogcat
Second Longest Compound Word: catsdogcats
Time taken: 5 milliseconds

For `Input_02.txt` (large list):

Longest Compound Word: ethylenediaminetetraacetates
Second Longest Compound Word: electroencephalographically
Time taken: 8000 milliseconds



## Notes
- Ensure the input files are correctly formatted and located at the specified paths.
- Performance may vary depending on the size of the input file and system resources.

