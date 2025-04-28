🛒 Order Management System
This project builds a simple and expandable system for managing orders. It connects a React-based frontend to a Node.js backend. PostgreSQL stores all important data, Redis speeds up frequently needed queries, and RabbitMQ handles tasks like processing orders in the background.

✨ Main Features
Place Orders: Users can easily select a product and place an order.

Handle Orders: Orders are processed in the background using RabbitMQ, so the system stays fast.

Quick Data Access: Redis is used to quickly get saved data.

Save Information: PostgreSQL is used to store details about products and orders.

Easy Frontend: A clean and simple React website for users.


🏗️ How the System Works
The system is made up of different parts that work together:
Frontend (React): Where users place orders and see products.
Backend (Node.js + Express): Handles the main logic and talks to the database and cache.
Database (PostgreSQL): Stores all the product and order information safely.
Cache (Redis): Stores frequently used data so it loads faster.
Message Queue (RabbitMQ): Helps process orders in the background without slowing down the app.


⚙️ System Requirements
Node.js
PostgreSQL
Redis
RabbitMQ
Docker and Docker Compose


🚀 Setup Instructions
1. Set Up Environment Variables
Create a .env file in the root directory and configure the following variables:
POSTGRES_DB=db_name
POSTGRES_USER=user_name
POSTGRES_PASSWORD=db_pass


🚢 Launch Services using Docker Compose
docker-compose up --build 


🌐 Access Points
Frontend: http://localhost:3000
Backend API: http://localhost:5000
RabbitMQ Dashboard: http://localhost:15672


📡API Routes
1. Get List of Products
2. Create a New Order
3. Get Orders by Product ID


🎨 Design Choices 
React: For making a user-friendly and dynamic website.
Node.js + Express: To handle backend logic easily and quickly.
PostgreSQL: To safely store all the data.
Redis: To make the app faster by caching data.
RabbitMQ: To manage order processing smoothly without slowing down the system.



