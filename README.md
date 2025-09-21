E-Commerce Product Catalog

A full-stack E-Commerce Product Catalog application built with React (frontend) and Node.js/Express (backend) with MongoDB/MySQL as the database. 
Allows users to browse, filter, and manage products, with admin functionalities for CRUD operations.

Features

User registration and login 
Browse product list with images, prices, categories, and stock count
Add, edit, and delete products (admin only)
Filter products by category
Responsive UI using Tailwind CSS
API-based architecture for frontend-backend communication

Tech Stack

Frontend: React, Tailwind CSS, Axios, React Router
Backend: Node.js, Express.js
Database: MongoDB 
Authentication: JWT 
HTTP Requests: Axios

Installation

Backend Setup

cd backend
npm install
Create .env file:
DB_URI=mongodb://localhost:27017/ecommerce
PORT=5000

Start backend server:
nodemon server.js

Frontend Setup
cd frontend
npm install

Configure API base URL in .env:

REACT_APP_API_URL=http://localhost:5000
Start frontend server:
npm run dev

API Endpoints

Products

GET /api/products – Get all products
GET /api/products/:id – Get product by ID
POST /api/products – Add new product
PUT /api/products/:id – Update product by ID
DELETE /api/products/:id – Delete product by ID

Users 

POST /api/auth/register – Register new user
POST /api/auth/login – Login user
GET /api/auth/profile – Get user profile

Usage

Open the frontend on http://localhost:5173
Browse products or perform admin actions (add/edit/delete)
Filter products by category

Database Models

User: email, password, created_at
Product: name, description, price, category, countInStock, image, created_at
Category: name, description, created_at
Order (optional): user_id, products, total_price, status, created_at

Testing

postman

About

No website provided. This project demonstrates a full-stack e-commerce catalog with React and Node.js.

Resources

Readme: Yes
Activity: Track commits in GitHub
Languages: JavaScript 100%

