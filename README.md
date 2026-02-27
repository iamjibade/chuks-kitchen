# chuks-kitchen

Chuks Kitchen Web Application

## 1. Project Overview

Chuks Kitchen is a responsive food ordering web application that allows users to:

* Create an account and log in
* Browse meals
* View detailed product information
* Customize orders (protein selection, extra sides, special instructions)
* Place and manage orders

The project is built using:

* **HTML5** – Structure
* **CSS3** – Styling and layout
* **JavaScript** – Interactivity (if implemented)
* (Optional) Backend: PHP / Node.js / Firebase
* (Optional) Database: MySQL / MongoDB / Firebase Firestore

---

## 2. System Requirements

To run the project locally, the following are required:

### For Frontend Only (Static Version)

* A modern web browser (Chrome, Edge, Firefox, Safari)
* Text editor (VS Code recommended)

### For Backend Version (if applicable)

* XAMPP / WAMP (for PHP & MySQL)
  OR
* Node.js (v16 or higher)
* npm (Node Package Manager)
* Database system (MySQL / MongoDB)

---

## 3. How to Run the Project (Frontend Only Version)

### Step 1: Download or Clone the Project

Download the project folder or clone it using:

```
git clone https://github.com/your-repository-name.git
```

### Step 2: Open the Project Folder

Open the folder in VS Code or any code editor.

### Step 3: Run the Application

Simply double-click:

```
index.html
```

Or right-click → **Open with Live Server** (if using VS Code Live Server extension).

The application will open in your default browser.

---

## 4. How to Run the Project (With Backend – PHP Example)

### Step 1: Install XAMPP

Download and install XAMPP.

### Step 2: Move Project Folder

Move the project folder into:

```
xampp/htdocs/
```

Example:

```
xampp/htdocs/chuks-kitchen/
```

### Step 3: Start Apache & MySQL

Open XAMPP Control Panel and start:

* Apache
* MySQL

### Step 4: Import Database

1. Open browser
2. Go to:

```
http://localhost/phpmyadmin
```

3. Create a new database (e.g., `chuks_kitchen`)
4. Import the provided `.sql` file

### Step 5: Configure Database Connection

Edit the database connection file:

```php
$conn = new mysqli("localhost", "root", "", "chuks_kitchen");
```

### Step 6: Run the Application

Open browser and go to:

```
http://localhost/chuks-kitchen/
```

---

## 5. Folder Structure

Example structure:

```
chuks-kitchen/
│
├── index.html
├── signin.html
├── signup.html
├── Onboarding.html
├── product.html

├── css/
│   └── style.css
│

│
├── images/
│   
│
└── backend/
    ├── config.php
    ├── login.php
    ├── register.php
    └── order.php
```

---

## 6. Features Implemented

* Responsive split-screen authentication pages
* Product customization (radio buttons & checkboxes)
* Form validation
* Special instructions textarea
* Structured footer and navigation
* Price display

(Optional advanced features if added:)

* Dynamic price update
* Add to cart functionality
* Session-based login
* Database integration

---

## 7. Security Considerations

If backend is implemented:

* Passwords must be hashed using `password_hash()` (PHP) or bcrypt (Node)
* Input validation and sanitization
* Use prepared statements to prevent SQL injection
* HTTPS recommended for production

---

## 8. Deployment

To deploy online:

* Purchase domain and hosting (e.g., Hostinger, Bluehost)
* Upload files via cPanel File Manager or FTP
* Configure database in hosting environment
* Update database credentials

For Node.js:

* Deploy using platforms like:

  * Render
  * Railway
  * Vercel
  * Heroku

---

9. Future Improvements

* Payment gateway integration (Paystack / Flutterwave)
* Admin dashboard
* Order tracking
* Email notifications
* Mobile app version

