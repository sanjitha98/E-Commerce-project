# E-Commerce Product Catalog

A full-stack **E-Commerce Product Catalog** application built with **React** (frontend) and **Node.js/Express** (backend) using **MongoDB** as the database.  
This application allows users to browse, filter, and manage products, with admin functionalities for full CRUD operations.

---

## Features

- User registration and login  
- Browse products with images, prices, categories, and stock count  
- Add, edit, and delete products (admin only)  
- Filter products by category  
- Responsive UI built with **Tailwind CSS**  
- API-based frontend-backend communication  

---

## Tech Stack

- **Frontend:** React, Tailwind CSS, Axios, React Router  
- **Backend:** Node.js, Express.js  
- **Database:** MongoDB  
- **Authentication:** JWT  
- **HTTP Requests:** Axios  

---

## Installation

### 1. Backend Setup

 cd backend
 npm install

### 2.Create .env file:
  DB_URI=mongodb://localhost:27017/ecommerce
  PORT=1000

### 3.Start backend server:
  nodemon server.js

### 4.Frontend Setup
  cd frontend
  npm install

### 5.Configure API base URL in .env:
  VITE_API_URL=http://localhost:1000

### 6.Start frontend server:
  npm run dev

### API Endpoints

# 1.Products

 GET /api/products – Get all products
 GET /api/products/:id – Get product by ID
 POST /api/products – Add new product
 PUT /api/products/:id – Update product by ID
 DELETE /api/products/:id – Delete product by ID

# 2.Users 

 POST /api/auth/register – Register new user
 POST /api/auth/login – Login user
 GET /api/auth/profile – Get user profile

## Usage

 Open the frontend on http://localhost:5173
 Browse products or perform admin actions (add/edit/delete)
 Filter products by category

## Database Models

 User: email, password, created_at
 Product: name, description, price, category, countInStock, image, created_at
 Category: name, description, created_at
 Order (optional): user_id, products, total_price, status, created_at

## Testing

 Use Postman or any API client to test endpoints.

# About

 This project demonstrates a full-stack e-commerce catalog using React for frontend, Node.js/Express for backend, and MongoDB for data storage. Ideal for learning modern    web development concepts.



