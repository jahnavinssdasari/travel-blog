# Travel Blog Project

## Overview
This project is a dynamic travel blog developed using HTML, CSS, PHP, and MySQL. It features a booking system that stores user details in a database and uses Swiper for interactive elements. The project is designed to be run on a local server using XAMPP.

## Features
- **Responsive Design**: Created with HTML and CSS to ensure the blog is accessible on various devices.
- **Dynamic Content**: PHP and MySQL are used to manage and display dynamic content, such as blog posts and booking details.
- **Booking System**: Users can book travel packages, and their details are stored in a MySQL database.
- **Interactive Elements**: Swiper is used to create interactive sliders and carousels.
- **JavaScript Functionality**: Enhances user experience with dynamic interactions.

## Prerequisites
- **PHP**: Ensure PHP is installed on your system.
- **XAMPP**: A local server environment to run PHP and MySQL.
- **Web Browser**: Any modern web browser to view the project.

## Installation
### Step 1: Install XAMPP
1. Download XAMPP from the [official website](https://www.apachefriends.org/index.html).
2. Install XAMPP by following the instructions for your operating system.
3. Start the Apache and MySQL modules from the XAMPP control panel.

### Step 2: Set Up the Project
1. Clone this repository to your local machine:
   ```bash
   git clone https://github.com/jahnavinssdasari/travel-blog.git
Copy the project files to the htdocs directory in your XAMPP installation folder (e.g., C:\xampp\htdocs\travel-blog).
### Step 3: Set Up the Database
Open your web browser and go to http://localhost/website.
Create a new database named travel_blog.
Import the travel_blog.sql file located in the database directory of the project into the travel_blog database. This will create the necessary tables.
### Step 4: Configure the Project
refer the code 
Open the config.php file located in the root directory of the project.

Update the database connection details to match your local setup:

php
Copy code
<?php
$servername = "localhost";
$username = "root"; // Default username for XAMPP
$password = ""; // Default password for XAMPP
$dbname = "travel_blog";

// Create connection
$conn = new mysqli($servername, $username, $password, $dbname);

// Check connection
if ($conn->connect_error) {
    die("Connection failed: " . $conn->connect_error);
}
?>
### Step 5: Run the Project
Open your web browser and navigate to http://localhost/travel-blog.
You should see the home page of the travel blog.
Project Structure
home.php: The main page of the travel blog.
about.php: A page with information about the blog.
package.php: Displays a list of packages.
book.php: The booking form for travel packages.
book_config.php: Configuration file for database connection.
images/: Contains CSS, JavaScript, and image files.
database/: Contains the SQL file for setting up the database.
### Usage
Booking System
Navigate to the booking page (http://localhost/website/book.php).
Fill out the booking form with the required details.
Submit the form to store the booking information in the database.
View the stored booking details in the database through phpMyAdmin or a dedicated admin panel if implemented.
Interactive Elements with Swiper
Swiper is used in various parts of the website to create sliders and carousels.
The Swiper configuration can be found in the relevant JavaScript files in the assets/js directory.
Live Tracking of Data
The project uses PHP to handle form submissions and interact with the MySQL database.
All interactions and data tracking can be monitored via the XAMPP control panel and phpMyAdmin.
Contributing
Contributions are welcome! Please fork the repository and submit a pull request with your changes.


We hope you enjoy using and contributing to the Travel Blog project. Feel free to explore the code, enhance features, and create a more comprehensive travel blog experience.





