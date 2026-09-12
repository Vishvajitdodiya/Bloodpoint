 BloodPoint – Blood Donation Management System

BloodPoint is an Android-based **Blood Donation Management System** developed using **Java, XML, and SQLite** in Android Studio. The application is designed to make donor information management simple, organized, and efficient.

The system provides user registration and login functionality along with features for adding, viewing, editing, and deleting blood donor records.


 Project Overview

BloodPoint helps maintain blood donor information digitally instead of relying on manual records. Users can register and log in to the application and manage donor details such as:

* Donor Name
* Mobile Number
* Blood Group
* Address

The application uses a local SQLite database to store and manage user and donor information.


 Features

 User Authentication

* User Registration
* User Login
* Email and Password authentication
* Mobile number and blood group information

 Donor Management

* Add new donor
* View donor list
* Edit donor information
* Delete donor information
* Store donor name, mobile number, blood group, and address

 Database Management

* Local SQLite database
* User data storage
* Donor data storage
* Insert, Read, Update, and Delete (CRUD) operations

 User Interface

* Simple Android XML layouts
* User-friendly navigation
* RecyclerView for displaying donor records
* Blood group selection using Spinner


 Technologies Used

| Technology     | Purpose                  |
| -------------- | ------------------------ |
| Java           | Application development  |
| XML            | User interface design    |
| Android Studio | Development environment  |
| SQLite         | Local database           |
| RecyclerView   | Displaying donor records |
| Gradle         | Project build system     |


 Project Structure

```text
Bloodpoint/
│
├── app/
│   └── src/
│       └── main/
│           ├── java/
│           │   └── com/example/bloodpoint/
│           │       ├── AddDonorActivity.java
│           │       ├── DonorListActivity.java
│           │       ├── DonorAdapter.java
│           │       ├── MainActivity.java
│           │       │
│           │       ├── auth/
│           │       │   ├── LoginActivity.java
│           │       │   └── RegisterActivity.java
│           │       │
│           │       ├── database/
│           │       │   └── DBHelper.java
│           │       │
│           │       └── Model/
│           │           └── DonerModel.java
│           │
│           └── res/
│               ├── drawable/
│               ├── layout/
│               ├── mipmap/
│               ├── values/
│               └── xml/
│
└── README.md
```


 Application Flow

```text
Start Application
       ↓
     Login
       ↓
   ┌───┴────┐
   │        │
Login     Register
   │        │
   └───┬────┘
       ↓
 Main Dashboard
       ↓
 ┌─────┴─────────┐
 ↓               ↓
Add Donor    View Donors
 ↓               ↓
Save Data    Donor List
                 ↓
          ┌──────┴──────┐
          ↓             ↓
        Edit          Delete
```


 Database

BloodPoint uses **SQLite** for local data storage.

Users Table

The users table stores registered user information.

| Field      | Description        |
| ---------- | ------------------ |
| id         | Unique user ID     |
| email      | User email         |
| password   | User password      |
| mobile     | User mobile number |
| bloodGroup | User blood group   |

Donors Table

The donors table stores donor information.

| Field      | Description         |
| ---------- | ------------------- |
| id         | Unique donor ID     |
| name       | Donor name          |
| mobile     | Donor mobile number |
| bloodGroup | Donor blood group   |
| address    | Donor address       |


 CRUD Operations

The application supports complete donor record management:

* **Create** – Add a new donor
* **Read** – View stored donors
* **Update** – Edit donor details
* **Delete** – Remove donor records

These operations are managed through the `DBHelper` class.


 How to Run the Project

1. Clone or Download the Project

Download the BloodPoint project and extract the project folder.

2. Open in Android Studio

Open **Android Studio** and select:

```text
File → Open
```

Then select the `Bloodpoint` project folder.

3. Sync Gradle

Allow Android Studio to complete the Gradle synchronization.

4. Connect a Device

You can either:

* Connect an Android smartphone with USB debugging enabled, or
* Start an Android Emulator.

5. Run the Application

Click the Run ▶ button in Android Studio.

The application will start with the Login/Registration interface.


 Main Modules

1. Login Module

Allows registered users to access the application.

2. Registration Module

Allows new users to create an account by providing their required information.

3. Main Dashboard

Provides access to the major donor-management functions.

4. Add Donor Module

Allows donor information to be entered and saved in the database.

5. Donor List Module

Displays all stored donor records using RecyclerView.

6. Edit Donor Module

Allows existing donor information to be modified.

7. Delete Donor Module

Allows unwanted donor records to be removed after confirmation.


 Validation

The application performs basic validation before storing information, including:

* Empty field validation
* Blood group selection validation
* Required donor information validation
* User registration validation


 Future Enhancements

The following features can be added in future versions:

*  Search donors by blood group
*  Nearest blood bank and hospital location
*  Google Maps integration
*  Emergency blood request notifications
*  Firebase/online database synchronization
*  Push notifications
*  User profile management
*  Blood availability management
*  Improved authentication and password security


 Project Purpose

BloodPoint was developed as an academic Android application to demonstrate practical implementation of:

* Android application development
* Java programming
* XML-based UI design
* SQLite database management
* CRUD operations
* RecyclerView
* User authentication
* Object-oriented programming


 Development
Project Name:BloodPoint
Project Type:Android Application
Platform:Android
Programming Language:Java
UI:XML
Database:SQLite
IDE:Android Studio

 License

This project is developed for **educational and academic purposes**.

You are free to study and modify the source code for learning and project development.


 Conclusion

BloodPoint provides a simple digital solution for managing blood donor information. By replacing manual donor records with an Android-based system, the application makes storing, updating, and viewing donor information easier and more organized.

The project can be further expanded into a complete blood donation platform by integrating online databases, location services, emergency requests, notifications, and hospital/blood-bank services.
