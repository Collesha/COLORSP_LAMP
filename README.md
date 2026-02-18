# COLORS Application

## Description
The COLORS application is a personal contact and color management system built on the LAMP stack.It allows users to register accounts, log in securely, and manage a personalized list of color entries through a dynamic web interface.

## Technologies Used
* **Operating System:** Ubuntu 20.04 (Digital Ocean Droplet).
* **Web Server:** Apache.
* **Database:** MySQL.
* **Backend:** PHP.
* **Frontend:** HTML5, CSS3, and JavaScript.

## High-Level Setup Instructions
1. **Server Environment:** Provision a LAMP droplet on Digital Ocean and configure a domain to point to the server's IP address.
2. **Database Configuration:** Create a MySQL database named `COP4331`.
    * Execute SQL scripts to generate the `Users` and `Colors` tables.
    * Create a dedicated database user (e.g., 'TheBeast') with appropriate privileges.
3. **API Implementation:** Upload the PHP files (`AddColor.php`, `Login.php`, and `SearchColors.php`) to the `/var/www/html/LAMPAPI` directory.
4. **Connection Setup:** Update the `$conn` mysqli statement in all PHP files with the correct database credentials.
5. **Frontend Deployment:** Move the `index.html`, `color.html`, and supporting `css/` and `js/` directories to the web root at `/var/www/html/`.

## How to Run and Access
* Open a web browser and navigate to your domain or server IP address (e.g., `http://[Your-IP-Address]`).
* Use the landing page to log in with your credentials.
* Once authenticated, use the interface to add new colors or search through your existing collection.

## Assumptions and Limitations
* **Assumptions:** It is assumed that the server is running a standard Apache configuration and that the database user has been granted full privileges on the `COP4331` database.
* **AI Usage:** AI helped structure the README.md based on the assignment rubric. The prompt I gave it was "Generate a readme file based on the attached document." The attached file was the "Getting started with LAMP" pdf in canvas.
