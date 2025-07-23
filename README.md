D.A.K.A.P. Drinks Website

Project Overview
Welcome to the D.A.K.A.P. Drinks Website! This project is a simple, yet functional web application designed for a drink company to showcase its products. It features a clean, modern user interface and a robust backend for managing drink inventory. Users can view a list of available drinks, and administrators can add, edit, and delete drink entries through an intuitive interface.

Features
Product Catalog: Displays a list of drinks with their name, description, price, batch number, expiry date, quantity, and subtype.

CRUD Operations:

Create: Add new drink products to the inventory.

Read: View details of all existing drinks.

Update: Modify details of existing drink products.

Delete: Remove drinks from the inventory.

Multi-Page Navigation: Navigate between "Home," "Products," "About Us," and "Contact" sections within a single-page application feel.

Responsive Design: The website layout adapts to different screen sizes (mobile, tablet, desktop).

Modal Forms: Clean and user-friendly pop-up forms for adding and editing drink details, with scrollability for longer forms.

Confirmation Dialogs: Prompts for confirmation before irreversible actions like deleting a drink.

Notification Messages: Provides visual feedback for successful operations or errors.

Technologies Used
Backend:

Flask: A lightweight Python web framework.

SQLite: A file-based SQL database for storing drink information.

Flask-CORS: For handling Cross-Origin Resource Sharing, allowing the frontend to communicate with the backend.

Frontend:

HTML5: For structuring the web content.

CSS3: For styling and layout.

JavaScript (ES6+): For interactive elements and dynamic content loading.

Tailwind CSS: A utility-first CSS framework for rapid UI development.

Google Fonts (Inter): For modern and legible typography.

Project Structure
drink_company_website/
├── app.py              # Main Flask application (backend logic, API endpoints, serving HTML)
├── schema.sql          # SQL script to define and initialize the database table
├── static/             # Contains static assets (CSS, JS)
│   ├── css/
│   │   └── style.css   # Custom CSS for specific elements (e.g., modal, message box)
│   └── js/
│       └── script.js   # Frontend JavaScript for all interactions and API calls
└── templates/          # Contains HTML template files
    └── index.html      # The main single-page application HTML file

Setup Instructions
Follow these steps to get the D.A.K.A.P. Drinks Website running on your local machine.

Prerequisites
Python 3.7+

pip (Python package installer)


Install Dependencies:
Install the required Python packages using pip:

pip install Flask Flask-Cors

Initialize the Database:
The app.py script automatically initializes the database.db file and creates the drinks table based on schema.sql when it runs for the first time. If you've run it before and want a fresh database (e.g., after modifying schema.sql), you should delete the existing database.db file before running app.py.

# Optional: Delete existing database if you want a fresh start
# del database.db  # On Windows
# rm database.db   # On macOS/Linux

Run the Flask Application:
Start the Flask development server:

python app.py

You should see output indicating that the server is running, usually on http://127.0.0.1:5000.

Usage
Access the Website:
Open your web browser and navigate to:

http://127.0.0.1:5000

Navigate Pages:
Use the navigation links in the header (Home, Products, About Us, Contact) to switch between different sections of the website. The "Products" page will display your drink inventory.

Manage Drinks (Products Page):

Add New Drink: Click the "Add New Drink" button to open a modal form. Fill in the details (Name, Description, Price, Batch No., Expiry Date, Quantity, Drink Subtype) and click "Save Drink."

Edit Drink: Click the "Edit" button on any drink card to open the modal pre-filled with that drink's current information. Make your changes and click "Save Drink."

Delete Drink: Click the "Delete" button on a drink card. A confirmation dialog will appear. Click "Yes" to confirm deletion.


Contributors
1. WOLA AFOLABI OLUWADARASIMI ISAAC - app.py , database.db AND README 
2. TOGBE GBENGA RIGHTEOUSNESS - templates/index.html
3. DAVID EDOSA - static/Js/script.js
4. DAVID AWUNOR - schema.sql
5. AJIMA OHEJI PRAISE - static/css/style.css
