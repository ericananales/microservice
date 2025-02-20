E-Commerce Microservices API
This project consists of two microservices:

User Service: Handles user registration and fetching user details.
Order Service: Manages order creation and fetching orders for a user.
Technologies
Flask
Flask-SQLAlchemy
PostgreSQL
Docker & Docker Compose
Setup
Clone the repository.
Navigate to the project directory and build containers:
bash
Copy
docker-compose up --build
Services
User Service (Port 5000):

POST /register - Register a new user.
GET /user/<id> - Get user details.
Order Service (Port 5001):

POST /user/<id>/order - Create an order for a user.
GET /user/<id>/orders - Get all orders for a user.
Docker Compose
Run all services with:

bash
Copy
docker-compose up
