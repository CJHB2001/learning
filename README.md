# Ayur Essence AI Base Web Application
A comprehensive Ayurvedic web application built using Laravel 10.

# Images

<div align="center">
  <table>
    <tr>
      <td><img src="/Documents/Images/HomePage1.png" width="300" alt="Home Page"></td>
      <td><img src="/Documents/Images/HomePage2.png" width="300" alt="Admin Driver Login"></td>
      <td><img src="/Documents/Images/BookingPage.png" width="300" alt="Admin Dashboard"></td>
    </tr>
    <tr>
      <td><img src="/Documents/Images/AdminDasboard.png" width="300" alt="Driver Dashboard"></td>
        <td><img src="/Documents/Images/AdminDashboard2.png" width="300" alt="Driver Dashboard"></td>
        <td><img src="/Documents/Images/BookingAdmin.png" width="300" alt="Driver Dashboard"></td>
    </tr>
      <tr>
      <td><img src="/Documents/Images/AdminDriverLoin.png" width="300" alt="Driver Dashboard"></td>
        <td><img src="/Documents/Images/d1.png" width="300" alt="Driver Dashboard"></td>
        <td><img src="/Documents/Images/d2.png" width="300" alt="Driver Dashboard"></td>
    </tr>
  </table>
</div>


## Features
### Admin Features
- **View Recent Orders** – Monitor and track recent customer orders.
- **Generate Reports** – Generate reports related to orders, users, and other system activities.
- **View and Reply to Queries** – Access and respond to customer queries.
- **View Customer Messages** – Read messages sent by customers.
- **Manage Ayurvedic Data** – Add, update, and delete information related to:
  - Ayurvedic Plants
  - Ayurvedic Doctors
  - Ayurvedic Treatments
  - Plant Diseases
  - Ayurvedic Hospitals
  - Blog Posts
  - Gallery
  - Services
  - Users
- **Admin Authentication** – Login and Logout functionality with password verification and error handling.

### Customer Features
- **Register & Login** – Create an account and access the system securely.
- **Make an Online Order** – Place orders for Ayurvedic products or services.
- **View Ayurvedic Information** – Browse details about:
  - Ayurvedic Plants
  - Ayurvedic Doctors
  - Ayurvedic Treatments
  - Plant Diseases
  - Ayurvedic Hospitals
- **Submit Queries, Reviews, Subscriptions, and Messages** – Send queries and provide feedback.
- **View Order History** – Check past orders.
- **Make a Payment** – Complete online payments.
- **Search Ayurvedic Doctors and Plants** – Find specific Ayurvedic plants or doctors.
- **AI-Based Plant Identification** – Upload a plant image for AI-based identification.
- **Logout** – Securely log out of the system.

## Installation
1. Clone the project:
   ```bash
   git clone < https://github.com/madhuekanayake/AyurEssence>
   ```
2. Navigate to the project's root directory:
   ```bash
   cd ayur-essence
   ```
3. Create `.env` file:
   ```bash
   cp .env.example .env
   ```
4. Install dependencies:
   ```bash
   composer install
   ```
5. Set application key:
   ```bash
   php artisan key:generate 
   ```
6. Run migrations and seed data:
   ```bash
   php artisan migrate
   
   ```
7. Start the Laravel development server:
   ```bash
   php artisan serve
   ```
## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
