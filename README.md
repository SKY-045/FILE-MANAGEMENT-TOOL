# FILE-MANAGEMENT-TOOL

COMPANY: CODTECH IT SOLUTION

NAME: SAURABH KUMAR

INTERN ID: CT04DF95

DOMAIN: C++

DURATION: 4 WEEKS

MENTOR: NEELA SANTOSH 

# DESCRIPTION of the File Management Tool in C++


This C++ program is a simple and interactive File Management Tool that allows a user to perform basic operations on text files. These operations include writing to a file, reading the contents of a file, and appending data to an existing file. It demonstrates the use of C++ file streams (fstream), string manipulation, and console I/O to perform these tasks efficiently.

Program Structure
The program is organized into three main functions:

writeFile(const string& filename)

readFile(const string& filename)

appendFile(const string& filename)

Each of these functions handles a specific file operation. The main() function serves as the entry point and manages user interaction by displaying a menu, taking input, and calling the appropriate function based on the user's choice.

Functionality
1. Writing to a File

The writeFile() function opens the specified file using an ofstream (output file stream) in default mode, which truncates any existing content in the file. If the file opens successfully, the user is prompted to enter a line of data, which is then written into the file. If the file fails to open (due to permission issues, missing directories, or invalid filename), an error message is displayed. After writing, the file is closed.

2. Reading from a File

The readFile() function utilizes an ifstream (input file stream) to open and read from the specified file. If the file is successfully opened, it reads the contents line by line using getline() and prints each line to the console. If the file does not exist or cannot be opened, an error message is shown. This function is helpful for viewing the contents of a file after data has been written or appended.

3. Appending to a File

The appendFile() function opens the file in append mode using ofstream with the ios::app flag. This ensures that new data is added at the end of the file without overwriting existing content. Similar to writeFile(), it takes a line of user input and appends it to the file, followed by closing the stream. This is particularly useful when the user wants to keep previous data and only add new content.

User Interaction
The main() function is responsible for the user interface. It displays a menu with three options:

Write to a file

Read from a file

Append to a file

After displaying the menu, it asks the user to enter their choice (an integer from 1 to 3). Based on the choice, the user is prompted to enter a filename (expected to end with .txt). Then, the appropriate function is called.

The program includes basic error handling to manage invalid file openings but does not include input validation for incorrect data types or formats. One potential issue is the use of cin.ignore() inside both the writeFile() and appendFile() functions. This is typically done to clear any leftover newline characters from previous input, but it could be improved or moved to a centralized place like the main() function to avoid redundancy and bugs.

Educational Value
This program is a great example of beginner-level file handling in C++. It teaches:

How to use file streams (ifstream, ofstream)

How to open files in different modes (write, read, append)

How to read and write strings with getline()

Basic input/output and conditional logic

With a few improvements—like adding input validation, looping for multiple operations, and better error reporting—the program can serve as a foundational tool in larger file-based applications.

Conclusion
Overall, this C++ file management tool is a compact and functional program demonstrating core concepts of file I/O. It provides users with a way to interact with text files through the console, allowing writing, reading, and appending operations. Its clear structure and straightforward logic make it an excellent learning project for anyone starting out with C++ file handling.

# OUTPUT

![Image](https://github.com/user-attachments/assets/52de65ca-53ec-435c-884d-ffe03ec78ed2)
