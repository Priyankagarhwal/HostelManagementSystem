# Hostel Management System

## Introduction
Namaste! 👋 Welcome to the Hostel Management System project. This system is designed to help manage hostel bed reservations with ease. With this program, you can reserve beds, manage student information, and handle reservations efficiently.

## Features
- Reserve Beds: Easily reserve beds for students.
- Database Integration: Uses MySQL for storing hostel information.
- User-Friendly: Simple and easy-to-understand console interface.

## Prerequisites
Before you start, make sure you have the following:
- MySQL installed and running.
- MySQL C++ Connector installed.
- Windows OS (since it uses `windows.h`).

## Installation
1. **Clone the Repository:**
   ```bash
   git clone https://github.com/yourusername/HostelManagementSystem.git
   cd HostelManagementSystem
   ```

2. **Configure MySQL Database:**
   - Create a database named `mydb`.
   - Create a table named `hostel` with the following schema:
     ```sql
     CREATE TABLE hostel (
         Name VARCHAR(50),
         Bed INT,
         Fee INT
     );
     ```

3. **Update Database Credentials:**
   - Open the `main.cpp` file.
   - Update the `HOST`, `USER`, `PW`, and `DB` variables with your MySQL credentials.

4. **Compile the Code:**
   - Use a C++ compiler to compile the code. If you're using g++, the command will be something like this:
     ```bash
     g++ -o HostelManagementSystem main.cpp -lmysqlclient
     ```

## Usage
1. **Run the Program:**
   ```bash
   ./HostelManagementSystem
   ```

2. **Follow On-Screen Instructions:**
   - You will be greeted with a welcome message.
   - Choose the option to reserve a bed or exit the system.
   - If you choose to reserve a bed, enter the student's name when prompted.

## Code Explanation
The main parts of the code include:
- **Database Connection:** Connects to MySQL database using provided credentials.
- **Hostel Class:** Defines a `Hostel` class to manage hostel details.
- **Reservation System:** Provides a simple console-based interface for reserving beds.

## Sample Output
When you run the program, you will see output similar to this:
```
Welcome To Hostel Management System
***********************************
1. Reserve Bed:
2. Exit:
Enter Your Choice: 
```

## Contributing
Contributions are welcome! Please fork the repository and create a pull request with your changes. For major changes, please open an issue to discuss what you would like to change.

