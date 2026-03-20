    Product Inventory Management System
    📌 Project Overview

    The Product Inventory Management System is a backend web application developed using Node.js, Express.js, and MongoDB.
    It provides a secure RESTful API for managing product data with JWT-based authentication and user-specific inventory management.

    Users can register, log in, and perform CRUD operations (Create, Read, Update, Delete) on their product inventory.

    🚀 Features
    🔐 User Authentication

    User registration

    Secure login system

    Password hashing using bcrypt

    JWT token-based authentication

    📦 Product Management

    Add new products

    View all products belonging to the user

    Update product details

    Delete products from inventory

    🔒 Security

    Protected routes using middleware

    JWT verification for authorized access

    User-specific data access

    🛠️ Technologies Used

    Technology	    Purpose
    Node.js	        Backend runtime
    Express.js	    Web framework
    MongoDB	NoSQL    database
    Mongoose	MongoDB object modeling
    JWT	Authentication
    bcryptjs	Password encryption
    dotenv	Environment variable management
    Thunder Client	API testing

    📂 Project Structure
    server/
    │
    ├── src/
    │   ├── controllers/
    │   │   ├── auth.controller.js
    │   │   └── product.controller.js
    │   │
    │   ├── db/
    │   │   └── db.js
    │   │
    │   ├── middlewares/
    │   │   └── auth.middleware.js
    │   │
    │   ├── models/
    │   │   ├── User.js
    │   │   └── Product.js
    │   │
    │   ├── routes/
    │   │   ├── auth.routes.js
    │   │   └── product.routes.js
    │   │
    │   └── server.js
    │
    ├── package.json
    ├── .env
    └── README.md

    ⚙️ Installation & Setup
    1️⃣ Clone the Repository
    git clone https://github.com/salaisanthosh2007-hue/Product-Inventory-Management-System.git
    2️⃣ Navigate to Project Folder
    cd Product-Inventory-Management-System
    3️⃣ Install Dependencies
    npm install
    4️⃣ Configure Environment Variables

    Create a .env file and add:

    PORT=5000
    MONGO_URI=your_mongodb_connection_string
    JWT_SECRET=your_secret_key
    5️⃣ Run the Server
    npm start

    Server will start at:

    http://localhost:5000
    🔗 API Endpoints
    Authentication
    Register User
    POST /api/v1/auth/register
    Login User
    POST /api/v1/auth/login
    Product Management
    Create Product
    POST /api/v1/products
    Get All Products
    GET /api/v1/products
    Update Product
    PUT /api/v1/products/:id
    Delete Product
    DELETE /api/v1/products/:id
    🧪 API Testing

    APIs were tested using Thunder Client in VS Code.

    Example Request Body:

    {
    "name": "Laptop",
    "price": 55000,
    "quantity": 5,
    "description": "Gaming Laptop"
    }
    🗄️ Database

    MongoDB Atlas is used as the cloud database.

    Collections used:

    users
    products

    Relationship:

    One User → Many Products
    🎯 Target Users

    Small business owners managing product inventory

    Developers learning REST API development

    Students learning Node.js backend development

    Freelancers tracking product stock

    👩‍💻 Developed By

    Suvitha

    Backend Development Project
    Nan Mudhalvan Program

    📜 License

    This project is developed for educational purposes.