# E-commerce-store-with-flask-test

Structure: The code uses Flask for routing, Jinja2 for templating, and in-memory dictionaries for user data and cart management.
Authentication: The login-submit route handles user login and creates a session cookie. The logout route removes the session cookie. The logged_in variable keeps track of the user's login status.
Cart Functionality: The add-to-cart route handles adding items to the cart. The cart dictionary stores items in the cart.
HTML Templates: Each route uses a corresponding HTML template to display content.


## -----------------

This is a simple e-commerce store built with Flask. The project allows users to register, login, browse products, and add items to their cart. It includes basic user authentication and a simple in-memory database to store user data.

### Project Structure

The project contains the following files:

* **index.py:**  The main Flask application logic, handling routing, templating, user authentication, session management, cart management, and error handling.

### Functionality

* **Routing:** The application defines routes for the following pages:
    * `/`: Home page.
    * `/login`: Login page.
    * `/register`: Registration page.
    * `/cart`: View cart page.
    * `/add-to-cart`: Add items to cart.
    * `/login-submit`: Process login submissions.
    * `/register-submit`: Process registration submissions.
    * `/logout`: Log out the user.
* **Templating:** Uses Jinja2 templating to render HTML pages for the different routes.
* **User Authentication:** Implements basic user login and registration functionality. User data is stored in an in-memory dictionary (`users`).
* **Session Management:** Uses cookies to manage user sessions.
* **Cart Management:** Allows users to add items to their cart. Cart data is stored in an in-memory dictionary (`cart`).
* **Global `logged_in` variable:** Tracks the user's login status and is updated during login and logout.
* **Error Handling:** Provides a simple error handling mechanism for incorrect login attempts.

### Key Components

* **Flask:** The web framework used to build the application.
* **Jinja2:** The templating engine used to render HTML pages.
* **`users` dictionary:**  Stores user data (username, password, email).
* **`sessions` dictionary:** Tracks active user sessions.
* **`cart` dictionary:** Stores items in the user's shopping cart.
* **`logged_in` variable:** Tracks user login status.

### Improvements

* **Database Integration:** Currently, user data and cart information are stored in memory, which makes them volatile. Integrating a database (e.g., SQLite, PostgreSQL) would provide persistence and scalability.
* **Product Data:** The `add_to_cart` function uses placeholder product data. Replace this with actual product information from a database or external API.
* **Security:** Implement robust security measures such as password hashing, input validation, and CSRF protection.

### To Run the Application

1. Make sure you have Python and Flask installed.
2. Navigate to the directory containing the `index.py` file in your terminal.
3. Run `flask run`.
4. Access the application in your web browser at `http://127.0.0.1:5000/`.

### Further Development

* Implement a product catalog with a database or API integration.
* Add functionality for checkout and order processing.
* Enhance the user interface with better styling and design.
* Improve security measures to protect user data.

This README provides a basic overview of the project. Further documentation for specific functionalities or additional features can be added as needed. 
