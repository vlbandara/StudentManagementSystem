# Java GUI Application for Student Management System

This repository contains a simple Java GUI application that serves as a Student Management System. The application utilizes Swing for the graphical user interface and interacts with an SQL database to perform basic operations such as insertion, update, search, and deletion of student records.

## Prerequisites
To run this application, you need to have the following software installed on your system:
- Java Development Kit (JDK) 8 or higher
- MySQL or any other SQL database server

## Setting up the Database
1. Install and configure an SQL database server of your choice if you haven't already.
2. Create a new database to be used for this application.
3. Inside the database, create a table with the following schema:

   ```sql
   CREATE TABLE IF NOT EXISTS students (
       id INT PRIMARY KEY AUTO_INCREMENT,
       name VARCHAR(255),
       age INT,
       grade VARCHAR(10)
   );


Update the database connection details in the DatabaseConnection.java file located in the src directory. Modify the following variables to match your database configuration:
DB_URL: The URL of your database server.
DB_NAME: The name of the database created in the previous step.
DB_USER: The username to access the database.
DB_PASSWORD: The password for the database user.
Running the Application

Clone this repository to your local machine or download the source code as a ZIP file and extract it.
Open a terminal or command prompt and navigate to the project directory.
Compile the Java source files by executing the following command:
bash
Copy code
javac -cp ".:lib/mysql-connector-java-<version>.jar" src/*.java
Replace <version> with the appropriate version number of the MySQL Connector/J library. If you're using a different SQL database, replace the library name accordingly.
Run the application with the following command:
bash
Copy code
java -cp ".:lib/mysql-connector-java-<version>.jar:src" MainFrame
Again, replace <version> with the appropriate version number of the MySQL Connector/J library.
The application's GUI should now be displayed, allowing you to perform various operations on the student records.
Functionality

##The application provides the following features:

Insertion: Allows you to add new student records to the database by providing their name, age, and grade.
Update: Enables you to modify the details of an existing student record by selecting it from the table and entering the updated information.
Search: Lets you search for student records by name or ID. The search results are displayed in a table.
Deletion: Allows you to delete a student record by selecting it from the table.
Contributing

Contributions to this project are welcome. If you find any bugs or have suggestions for improvements, please open an issue or submit a pull request.

License

This project is licensed under the MIT License. Feel free to use and modify the code according to your needs.

Acknowledgments

This application was developed based on tutorials and examples provided by the Java Swing documentation and various online resources.

Contact

For any questions or inquiries, please feel free to reach out to me at vlbandara2000@gmail.com.
