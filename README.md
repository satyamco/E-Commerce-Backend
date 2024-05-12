---

# E-Commerce Backend

The "E-Commerce Backend" is a backend application for managing the data and operations of an e-commerce website.

## Features

- **Product Management**: Add, update, delete, and retrieve products.
- **Category Management**: Manage product categories.
- **User Authentication**: Secure user authentication and authorization.
- **Order Management**: Track and manage customer orders.

## Installation

To set up the "E-Commerce Backend" locally, follow these steps:

1. Clone the repository:

   ```bash
   git clone https://github.com/satyamco/E-Commerce-Backend.git
   ```

2. Navigate into the project directory:

   ```bash
   cd E-Commerce-Backend
   ```

3. Install dependencies:

   ```bash
   npm install
   ```

4. Set up the database:
   - Create a `.env` file in the project root directory.

     ```
     PORT=5000
     MONGO_URI=mongodb://127.0.0.1:27017
     JWT_SECRET=your jwt secret
     ```


5. Start the server:

   ```bash
   npm start
   ```

## Usage

### API Endpoints

- **Products**:
  - `GET /api/products`: Retrieve all products.
  - `GET /api/products/:id`: Retrieve a specific product.
  - `POST /api/products`: Add a new product.
  - `PUT /api/products/:id`: Update a product.
  - `DELETE /api/products/:id`: Delete a product.
  - `POST /api/products/top`: get top Products.
  - `POST /api/products/new`: get new Products.

- **Categories**:
  - `GET /api/categories`: Retrieve all categories.
  - `GET /api/categories/:id`: Retrieve a specific category.
  - `POST /api/categories`: Add a new category.
  - `PUT /api/categories/:id`: Update a category.
  - `DELETE /api/categories/:id`: Delete a category.

- **Users**:
  - `POST /api/users/register`: Register a new user.
  - `POST /api/users/login`: User login.
  - `POST /api/users/logout`: User logout.
  - `GET /api/users/profile`: get current user profile.
  - `PUT /api/users/profile`: update current user profile.

- **Orders**:
  - `GET /api/orders/mine`: Retrieve all orders.
  - `GET /api/orders/:id`: Retrieve a specific order.
  - `GET /api/orders./:id`:get order by Id.
  - `POST /api/orders`: Place a new order.

## Contributing

Contributions to the "E-Commerce Backend" are welcome!
