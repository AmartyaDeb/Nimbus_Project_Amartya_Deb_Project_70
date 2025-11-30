# Nimbus_Project_Amartya_Deb_Project_70
School Fee Management System
Project Objective

The School Fee Management System helps educational instituions manage student fee records efficiently. This system enables administrators to:

Add new students and their fee details

Print fee reciepts for students

Apply penalty fees for late payments

View revenue summaries by course

The system also ensures that data persists between runs, saving student information to a file and allowing it to be loaded back when the program restarts. It tracks the fees paid, balances, and applies penalties as needed, making it a useful tool for managng school finances.

Development Steps
1. Project Setup

The first step was to define a Student structure that holds important information like the student's roll number, name, course, and fee details.

Functions were created to manange student records, such as adding a new student, printing their fee receipt, and applying late fees.

2. Input/Output Functionality

Developed user prompts for collecting information such as the student’s name, course, and fee details.

Initially used scanf for input, but later switched to fgets for string inputs like the name and course name to handle spaces and avoid issues with input buffering.

3. Data Persistence

A major part of the development was adding functionality to save and load student data to and from a binary file. This allows the system to keep records even after the program exits.

4. Late Penalty Fee

Implemented a late penalty fee that automatically applies a 5% fee on the outstanding balance for any student who has not paid their full fee by the time the penalty function is run.

5. Revenue Summary

Added a feature to display a revenue summary. This shows the total amount of fees collected and breaks it down by course.

6. Testing and Refining

After implementing the basic functionality, I ran tests to make sure that the system handles user input correctly, saves data reliably, and calculates balances and penalties as expected.

One important fix was ensuring that input functions like fgets worked smoothly for strings like names and courses by clearing the input buffer correctly after reading numeric inputs.

Output Screenshots

The system outputs various messages depending on the user's choices. Here are some of the types of outputs you can expect:

Main Menu: The user is presented with a list of options to choose from, such as adding a new student or displaying a fee receipt.

Adding a New Student: The program will ask for details like the student’s roll number, full name, course, and total fee, then save the data for future use.

Fee Receipt: After entering student data, you can print a detailed receipt that includes the student's name, course, total fee, amount paid, and outstanding balance.

Revenue Summary: The program can display a summary of the total revenue collected and how it breaks down by course.

Usage Instructions
1. Compiling the Code

To compile the program, run the following command in your terminal:

gcc -o fee_management_system fee_management_system.c

2. Running the Program

Once the program is compiled, you can run it with:

./fee_management_system

3. Using the Menu

The program presents a menu of options, and you can choose one by entering the corresponding number:

Add New Student: Allows you to input a new student’s details and save them.random aaah

Print Fee Receipt: Prints a fee receipt for each student, showing their fee details.

Apply Late Penalty Fee: Adds a penalty fee to students who still have an outstanding balance.

Display Revenue Summary by Course: Shows how much revenue has been collected and breaks it down by course.

Exit: Saves all student data to a file and exits the program.

4. Saving and Loading Data

The program automatically saves student data to a file (student_data.dat) when you exit.

On startup, it loads any previously saved data so you don’t lose your progress.

Conclusion

The School Fee Management System provides an efficient way to manage student fee records. It allows administrators to track fees, handle late penalties, and view detailed revenue summaries. By saving and loading data from a file, the system ensures that all information is retained between program runs.
