# E-commerce Backend API

A robust and scalable RESTful API built with Laravel for managing e-commerce operations.

## 🚀 Features

- User Authentication with JWT
- Product Management
- Order Processing
- Category Management
- User Profile Management
- Role-based Access Control
- Shopping Cart Functionality
- Payment Integration
- Order Tracking

## 🛠️ Tech Stack

- **PHP 8.x**
- **Laravel 10.x**
- **JWT Authentication**
- **MySQL**
- **RESTful API Standards**

## 📋 Prerequisites

- PHP >= 8.0
- Composer
- MySQL/SQLite
- Node.js & NPM

## ⚙️ Installation

1. Clone the repository
```sh
git clone https://github.com/ARASIF1-6/tech-titans_backend.git
cd E-commerce-Backend-Api
```

2. Install dependencies
```sh
composer install
npm install
```

3. Create environment file
```sh
cp .env.example .env
```

4. Generate application key and JWT secret
```sh
php artisan key:generate
php artisan jwt:secret
```

5. Configure your database in `.env`
```env
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=your_database_name
DB_USERNAME=your_username
DB_PASSWORD=your_password
```

6. Run migrations and seeders
```sh
php artisan migrate --seed
```

7. Start the development server
```sh
php artisan serve
```

## 🔑 API Authentication

This API uses JWT (JSON Web Tokens) for authentication. Configure your JWT settings in `config/jwt.php`.

## 📚 API Documentation

### Authentication Endpoints
- `POST /api/auth/register` - Register a new user
- `POST /api/auth/login` - User login
- `POST /api/auth/logout` - User logout
- `GET /api/auth/profile` - Get user profile

### Product Endpoints
- `GET /api/products` - Get all products
- `GET /api/products/{id}` - Get specific product
- `POST /api/products` - Create product (Admin)
- `PUT /api/products/{id}` - Update product (Admin)
- `DELETE /api/products/{id}` - Delete product (Admin)

## 🧪 Running Tests

```sh
php artisan test
```
- Your Name (@yourusername)

## 🙏 Acknowledgments

- [Laravel](https://laravel.com)
- [JWT Auth](https://github.com/tymondesigns/jwt-auth)
