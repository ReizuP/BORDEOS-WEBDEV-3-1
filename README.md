For Web Development - PUP-SPC 3-1

Installation Steps
Clone or download the repository

git clone <repository-url>

Or download and extract the ZIP file.


Move to your web server directory

XAMPP: C:\xampp\htdocs\web-app (Windows) or /opt/lampp/htdocs/web-app (Linux)
WAMP: C:\wamp64\www\web-app
MAMP: /Applications/MAMP/htdocs/web-app
Other: Your web server's document root
Configure database connection

Edit misc/database.php and update these values to match your setup:

$db_server = "localhost"; 
$db_user = "root"; //your username
$db_pass = 'root'; // your password
$db_name = 'vivace_db';
Create the database

Open phpMyAdmin or MySQL command line and create a new database:

CREATE DATABASE vivace_db;
Import the database schema located in C:\XAMPP\htdocs\Vivace\dumpsqlfile\VIVACE4.sql

Option A - Using phpMyAdmin:

Open phpMyAdmin (usually at http://localhost/phpmyadmin)
Select the webdemo database
Click "Import" tab
Choose file: dumpsqlfile\VIVACE4.sql
Click "Go"
Option B - Using MySQL command line:

mysql -u root -p webdemo < dumpsqlfile\VIVACE4.sql
Access the application

Open your browser and navigate to:

Homepage: http://localhost/BORDEOS-WEBDEV-3-1/index.php
Products: http://localhost/BORDEOS-WEBDEV-3-1/products.php
(Adjust the URL based on where you placed the project)

Create your account

Click "Sign Up" and create your own user account to start using the application.
