# Ayurvedic Medicinal Plant Conservation Platform

This repository contains the Laravel 10-based **Ayurvedic Medicinal Plant Conservation Platform**, an AI-powered web application designed to promote awareness, identification, and conservation of Sri Lanka's Ayurvedic medicinal plant heritage.

## Features

- **AI-Powered Image Recognition**: Users can upload images to identify Ayurvedic plants.
- **Comprehensive Plant Database**: Provides medicinal properties, cultural significance, and ecological status.
- **Educational Resources**: Articles, videos, and learning materials.
- **Biodiversity Tracking**: Interactive mapping to track plant species and conservation efforts.
- **Community Engagement**: Discussion forums and chatbot support.
- **Professional Consultation**: Connects users with Ayurvedic doctors and botanists.
- **Marketplace Integration**: Allows ethical trading of Ayurvedic plants.

## Technologies Used

- **Laravel 10**: PHP framework for backend development.
- **MySQL**: Database for storing plant data, user interactions, and marketplace transactions.
- **Bootstrap 5**: Frontend framework for responsive UI.
- **JavaScript, jQuery, AJAX**: Enhancing interactivity and real-time features.
- **Toastr.js**: For displaying success/error notifications.
- **Cloudinary (or Local Storage)**: For handling image uploads.
- **AI/ML Integration**: Image recognition powered by AI models (TensorFlow, OpenCV, or an API like Google Vision).

## Installation and Setup

To set up the project locally, follow these steps:

### 1. Clone the Repository
```bash
git clone https://github.com/YourUsername/ayurvedic-plant-conservation.git
cd ayurvedic-plant-conservation
```

### 2. Install Dependencies
```bash
composer install
npm install
```

### 3. Set Up Environment Variables
- Copy the `.env.example` file and rename it to `.env`.
- Update database credentials:
```env
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=ayurvedic_db
DB_USERNAME=root
DB_PASSWORD=
```

### 4. Generate Application Key
```bash
php artisan key:generate
```

### 5. Run Migrations and Seed Database
```bash
php artisan migrate --seed
```

### 6. Serve the Application
```bash
php artisan serve
```
Access the application at `http://127.0.0.1:8000`.

## Running Tests
To run unit tests using PHPUnit:
```bash
php artisan test
```

## Folder Structure
- **app/Http/Controllers**: Handles request processing.
- **app/Models**: Database models.
- **database/migrations**: Database schema.
- **resources/views**: Blade templates for UI.
- **public/uploads**: Stores uploaded plant images.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

