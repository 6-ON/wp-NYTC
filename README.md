# WordPress Installation Guide

This guide will provide you with a step-by-step guide on how to install WordPress on your local machine.

## Prerequisites

Before starting, you need to have the following:

-   A web server (e.g., Apache, Nginx)
-   PHP version 7.4 or higher
-   MySQL or MariaDB database
-   A text editor
-   A web browser

## Step 1: Download WordPress

Download the latest version of WordPress from the official website: [wordpress.org](https://wordpress.org/download/). Extract the downloaded zip file to your local machine.

## Step 2: Create a Database

WordPress needs a database to store all the content, so you need to create a new database. You can use a database management tool like phpMyAdmin or the MySQL command line to create a new database.

To create a new database using the MySQL command line, open the command prompt and enter the following command:


`mysql -u root -p` 

Enter your MySQL root password when prompted. Once you are logged in, enter the following command to create a new database:

`CREATE DATABASE database_name;` 

Replace `database_name` with your desired database name.

## Step 3: Configure WordPress

Copy the `wp-config-sample.php` file to `wp-config.php`. Open `wp-config.php` with a text editor and add your database details:


`define( 'DB_NAME', 'database_name' );

/** MySQL database username */
define( 'DB_USER', 'database_user' );

/** MySQL database password */
define( 'DB_PASSWORD', 'database_password' );

/** MySQL hostname */
define( 'DB_HOST', 'localhost' );` 

Replace `database_name`, `database_user`, and `database_password` with your database details.

## Step 4: Upload WordPress files

Upload the extracted WordPress files to your web server. You can use an FTP client like FileZilla or upload the files directly through cPanel.

## Step 5: Run the Installation

Open your web browser and go to your website's URL (e.g., `http://localhost/wordpress`). You should see the WordPress installation screen. Follow the on-screen instructions to complete the installation.

## Step 6: Log in to WordPress

Once the installation is complete, you can log in to WordPress by going to `http://localhost/wordpress/wp-login.php` and entering your username and password.

## Conclusion

Congratulations! You have successfully installed WordPress on your local machine. You can now start customizing your site and creating content. If you encounter any issues during the installation, refer to the WordPress documentation or seek help from the WordPress community.
