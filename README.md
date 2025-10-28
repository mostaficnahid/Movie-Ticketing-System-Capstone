Movie Ticketing System (C Capstone Project)

A robust, console-based application written entirely in C for managing movie ticket sales, theater capacity, and user bookings. This project serves as a capstone submission, demonstrating core C programming concepts, data structures, and file handling.

Overview

This Movie Ticketing System simulates the backend logic of a real-world cinema booking platform. It provides functionalities for both administrators (to manage movie listings and view sales) and users (to browse movies, book seats, and view their tickets). All data is persistently stored in local files, managed through C's file I/O operations.

Features

Admin Module:

Add new movie listings (title, genre, showtime, price).

Delete existing movie listings.

View all listed movies and their details.

Check booking status for any show (e.g., seats sold, seats available).

View total sales and revenue reports.

User Module:

View a list of all currently playing movies.

Select a movie and showtime.

View available seats in a 2D grid layout (e.g., [O] for available, [X] for booked).

Book one or more seats.

Cancel a previously booked ticket.

View booking history.

Data Persistence:

All movie listings, user credentials, and booking records are saved to text files (e.g., movies.dat, users.dat, bookings.dat).

Data is loaded from files upon application start and saved upon exit, ensuring no loss of information between sessions.

Error Handling:

Includes robust checks for invalid user input, file opening errors, and booking conflicts (e.g., trying to book an already-taken seat).

Technologies Used

Language: C (C99 standard)

Compiler: GCC (GNU Compiler Collection)

Core Concepts:

Data Structures (structs, arrays, 2D arrays for seating)

File Handling (fopen, fclose, fread, fwrite, fseek)

Pointers and Dynamic Memory Allocation (malloc, free)

Functions and Modular Programming

String Manipulation (string.h)

Conditional Logic and Loops

Prerequisites

To compile and run this project, you will need a C compiler installed on your system. The most common one is gcc.

On Linux (Debian/Ubuntu):

sudo apt update
sudo apt install build-essential


On macOS (with Homebrew):

brew install gcc


On Windows:

Install MinGW-w64 or TDM-GCC.

Alternatively, use WSL (Windows Subsystem for Linux) and follow the Linux instructions.

Compilation

Clone this repository or download the source code.

git clone [https://github.com/your-username/movie-ticketing-system.git](https://github.com/your-username/movie-ticketing-system.git)
cd movie-ticketing-system


Compile the project using gcc. Assuming your main file is main.c and you have other utility files (e.g., admin.c, user.c), you would compile them as follows:

If all code is in one file (e.g., main.c):

gcc main.c -o movie_ticket_system


If you have multiple .c files:

gcc main.c admin.c user.c utils.c -o movie_ticket_system


(Note: You may also need to link the math library if you use it: -lm)

Using the provided Makefile (if one exists):

make


How to Run

After successful compilation, an executable file named movie_ticket_system (or movie_ticket_system.exe on Windows) will be created.

Run the application from your terminal:

./movie_ticket_system


On Windows, you might run it as:

movie_ticket_system.exe


Example Usage

Upon running the application, you will be greeted with a main menu:

======================================
  MOVIE TICKET BOOKING SYSTEM
======================================
1. Admin Login
2. User Login
3. New User? Register
4. Exit
Enter your choice:


As a User: You can register, log in, view the list of movies, select one, and then choose your seats from a visual grid.

As an Admin: You can log in (using predefined credentials, e.g., admin/pass123) to access the administrative panel for managing movie listings.

Contributing

This is a capstone project, but contributions and suggestions are welcome! If you find a bug or have an idea for a new feature, please feel free to:

Fork the repository.

Create a new branch (git checkout -b feature/YourAmazingFeature).

Commit your changes (git commit -m 'Add some AmazingFeature').

Push to the branch (git push origin feature/YourAmazingFeature).

Open a Pull Request.

License

This project is licensed under the MIT License. See the LICENSE file for more details.
Author Name: Mostafic Yellahy Nahid

GitHub: mostaficnahid

LinkedIn: https://www.linkedin.com/in/mostafic-yellahy-nahid-46a0202b5/
